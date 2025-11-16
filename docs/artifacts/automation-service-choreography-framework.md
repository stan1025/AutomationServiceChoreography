# Artifact - Automation Service Choreography Framework

## Artifact Factsheet

!!! highlight ""

    | Fact Sheet | |
    | :--- | :--- |
    | **Name** | Automation Service Choreography Framework |
    | **Artifact Type** | Framework |
    | **Target Users** | System Architects, Software Architects, PLC Programmers |
    | **Objective** | Development of the *Automation Service Choreography Framework* to present the components necessary for developing and implementing automation services. It describes individual components as sub-artifacts and illustrates their mutual dependencies. The goal is to provide a comprehensive representation of all individual components as an entry point for future developers and users of automation service choreographies. |

## Relevant Publications




## Artifact Description

The *Automation Service Choreography Framework* provides the development framework that encompasses the required components of the described concept and presents relationships following a top-down approach. The framework consists of one architectural pattern and eight design patterns, organized into the four content areas named *System Architecture*, *Participants*, *Information Processing* and *Information Provisioning*. Its visualized within the following figure. 

![Automation Service Choreography Framework Overview](./Abbildung_Framework_Overview.drawio.png)
*Figure: Automation Service Choreography Framework and its Components*


## Artifact Building Blocks

### Choreography-enabled System Architecture

It represents the architectural pattern of this concept. it Introduces the resulting system architecture and shows the impact of choreographed automation services on service-based automation systems and their central orchestration in the Process Orchestration Layer.

### Active Choreography Participant

It represents the central building block as design patterns implementing automation service choreographies. It defines the components, relationships, and tasks of an active choreography participant with capabilities for information transfer and processing. 

### Passive Choreography Participant

It represents an extending building block of the Active Participant as design pattern. It enables the integration of legacy systems through decentralized orchestration by an active choreography participant. 

### External Lead

It represents a second extending building block by introducting a design pattern for the implementation of a special automation service. It introduces an automation service that plays an essential role in orchestrating choreographed functions when no available service can assume the leader role. 

### Configurable Logic

It represents an implementation related design pattern which specifies the core of information processing and enables influence on native control programs and configurable behavior based on internal and external information.

### Configurable Communication

It represents an abstract design pattern defining the foundation for configurable communication indepentend of the used communication technologies. A analysis of different communication pattern and their usable technologies extends this artifact.

### Configurable Communication with OPC UA Client/Server

It represents a technology-specific design pattern for the configurable communication using OPC UA Client/Server mechanisms. Base of this pattern represents the PLC Open OPC UA Client Function Block specification. 

### Configurable Communication with OPC UA Publish/Subscribe

It represents a technology-specific design pattern for the configurable communication using OPC UA Publish/Subscribe. It is possible to implement with this kind of communication technology one-to-many communication based on the push principle. 

### Configurable Communication with OPC UA Field Exchange

It represents a technology-specific design pattern for the configurable communication using OPC UA Field Exchange. It represents an alternative OPC UA mechanism which is itself already for the use of configurable communication. 


## Artifact Decisions

### Dual Target Audience

The framework is designed to cater to two distinct target audiences: system architects and software architects/PLC programmers. For system architects, it provides a "System View" that focuses on the *System Architecture* and *Participants* content areas. For software architects and PLC programmers, a more detailed "Software View" is offered, which extends the "System View" by also including the *Information Processing* and *Information Provisioning* areas.

### Modular Building Block System

Software components for configurable logic and communication are treated separately to enable flexible combination of multiple communication technologies. This supports targeted equipment of choreography participants with suitable communication mechanisms based on system strategy requirements.


## Artifact Application

### For System Architects

System architects use the *Choreography-enabled System Architecture* pattern as their entry point to design modular production systems with choreographed automation services. They are responsible for defining the framework conditions for software architects and PLC programmers, which involves considering the system-wide implications and design options for the choreography patterns.

### For Software Architects/PLC Programmers

Software architects and PLC programmers use the participant design patterns as their entry point. They are responsible for implementing the software components from the *Information Processing* and *Information Provisioning* areas. This allows for the flexible selection and combination of communication technologies, enabling the runtime composition of distributed functions based on system design requirements.












