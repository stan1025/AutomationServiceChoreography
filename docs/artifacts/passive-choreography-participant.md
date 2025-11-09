# Artifact - Passive Choreography Participant

## Artifact Description

!!! highlight ""

    | Fact Sheet | |
    | :--- | :--- |
    | **Name** | Passive Choreography Participant |
    | **Artifact Type** | Design Pattern |
    | **Target Users** | System Architects, Software Architects, PLC Programmers |
    | **Objective** | This artifact describes the necessary components and approaches to integrate non-choreography-capable equipment into a choreography using another active choreography participant as a decentralized orchestrator. This enables existing equipment to be used in choreographies while preserving investment protection. |

## Relevant Publications






## Artifact Description


The *Passive Choreography Participant* design pattern describes the conceptual building blocks for integrating non-choreography-capable legacy equipment into a choreography. This capability is of great importance for manufacturing companies in terms of investment protection. The integration of the passive participant is performed by the active participant. The active choreography participant serves as a decentralized orchestrator for the non-choreography-capable equipment and can be integrated into a choreography on behalf of the non-choreography-capable equipment.

## Artifact Technological Conditions


## Artifact Building Blocks

The *Passive Choreography Participant* design pattern consists of the actual passive participant and its control system, as well as an assigned active choreography participant, as shown in the figure below.

![Software architecture of an active choreography participant for integrating a passive choreography participant](./Inhalt/07_Vorstellung_der_Artefakte/Entwurfsmuster_PassiverTeilnehmer/Abbildung_PassiverTeilnehmer_Schema.drawio.png)

### Passive Choreography Participant - Native Program

The native program (orange area) represents the part of a control program that provides the automated functions of the modular unit, similar to the active participant case.

### Passive Choreography Participant - Passive Communication

The passive communication (lower blue area) represents a communication interface that takes a passive role within information transmission. An example would be an OPC UA Server in the underlying control system. This component provides information from the native program part and forwards information from passive communication back to the native control software.

### Active Choreography Participant - Configurable Communication

The configurable communication (upper blue area) provides the components for incoming and outgoing active communication from the assigned active choreography participant. In this case, the active choreography participant must have an active role in information transmission, for example an OPC UA Client, enabling it to actively push information to the passive participant and actively pull information from the passive participant.

### Active Choreography Participant - Configurable Logic

The configurable logic (green area) represents the component for configurable information processing. The configurable logic uses information from itself, from other active choreography participants, and from the passive choreography participant.


## Artifact Decisions


### Assumptions Regarding Legacy Equipment Interfaces

Evaluation at Merck revealed a conceptual gap regarding the integration of legacy equipment. A temperature control FEA could not be integrated because it had an unchangeable embedded controller and could not be made choreography-capable.

The selection of suitable communication technologies depends on the legacy system. The abstract *Configurable Communication* design pattern provides a flexible foundation for implementing available technologies analogously.

No restriction to MTP or OPC UA can be made. Solutions must be designed flexibly and technology-agnostic. Software architects and PLC programmers must be prepared and supported to successfully integrate non-standardized legacy systems.

### Static vs. Dynamic Integration

Two fundamental approaches exist for integrating legacy equipment:

**Static Integration:** Requires interfaces and communication technologies to be considered during development of choreography-capable systems. This is technically feasible but limits adaptability, as only equipment with previously known and prepared characteristics can be integrated.

**Dynamic Integration:** Possible by combining decentralized orchestration with the capabilities of an active choreography participant. Flexibility with different interfaces can be realized through the *Configurable Logic* design pattern by linking command and state variables of the legacy system with other choreography participants as needed.

Dynamic integration is preferred for legacy equipment integration. The combination of decentralized orchestration with active choreography participant capabilities and the *Configurable Logic* design pattern allows flexible interface linking and adaptation to different legacy systems.

## Artifact Implementation Details


For integrating a passive choreography participant into a choreography, an active choreography participant becomes its decentralized orchestrator, incorporating its functions into the circle of other active choreography participants.

The configurable logic and communication of an active choreography participant enable the integration of a passive participant. Data is transferred via pull communication to the active participant's input list, where behavioral rules for the passive participant are configured via the logic list. Results are then sent back via push communication through the output list.

The active choreography participant requires additional communication functions, particularly supporting the communication technology that the passive choreography participant supports. Technology-independently, this means an active choreography participant must provide the respective active communication side of a passive choreography participant to be integrated.

Communication failure between the orchestrating active choreography participant and its passive choreography participant leads to loss of controllability of the passive participant, requiring case-specific evaluation for exception handling.


## Artifact Application


Three execution variants are available for applying this design pattern:

### Variant 1 - Integrated Variant

![Integrated decentralized orchestration in a "normal" PEA](./Inhalt/07_Vorstellung_der_Artefakte/Entwurfsmuster_PassiverTeilnehmer/Abbildung_PassiverTeilnehmer_Integriert.drawio.png)

The *Integrated Variant* extends existing PEAs, FEAs, or COMPs with decentralized orchestrator functions for passive choreography participants. An active choreography participant can become a decentralized orchestrator for legacy equipment.

**Advantages:** Utilizes existing control systems
**Disadvantages:** Additional load on limited resources for communication and logic; communication technology must be considered during engineering

### Variant 2 - Standalone Variant

![Standalone decentralized orchestration in a proxy PEA](./Inhalt/07_Vorstellung_der_Artefakte/Entwurfsmuster_PassiverTeilnehmer/Abbildung_PassiverTeilnehmer_standalone.drawio.png)

The *Standalone Variant* uses a separately developed active choreography participant (proxy PEA) that contains the communication technology required for integrating legacy equipment alongside basic functions. This must be configurable for reuse with specific technologies.

**Advantages:** Relieves other choreography participants; easy retrofitting without interventions in existing equipment
**Disadvantages:** Additional system resource requirements and associated operating costs

### Variant 3 - Type-Specific Variant

![Type-specific decentralized orchestration in a proxy PEA](./Inhalt/07_Vorstellung_der_Artefakte/Entwurfsmuster_PassiverTeilnehmer/Abbildung_PassiverTeilnehmer_specific.drawio.png)

The *Type-Specific Variant* corresponds to the *Standalone Variant* but forgoes a configurable communication interface for the legacy equipment to be integrated. It is used when certain communication technologies or their implementation in control systems do not allow configurability. The communication technology is statically implemented for a specific type of legacy equipment.

**Advantages:** Extended selection of communication technologies that become usable despite static implementation
**Disadvantages:** Fixed to concrete legacy equipment, though flexibility toward choreography is retained

## Artifact Pros/Cons



