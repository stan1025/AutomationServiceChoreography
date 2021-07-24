# :mortar_board: AUTOMATION SERVICE CHOREOGRAPHY

[:rewind:back](../README.md)


Editing Status: :construction: (under construction))

Last Modification: 25.07.2021

---


## :three: Software Pattern - Configurable Communication


**Name**  
*Name of the PLC Programming Pattern*

Value Registry Pattern

---

**Purpose**  
*Purpose of the PLC Programming Pattern*

This pattern includes the ability for a free configurable PEA-to-PEA communication based on OPC UA Client-Server structure. The Client-Interface is configurable via the own OPC UA Server. According to this, a vendor-independent configurable PEA-to-PEA communication can be realized.


---

**Motivation**  
*Reason to use the pattern*

If your PLC programm requires a communication interface, where to count of partners or the distribtion of intformation is not known at the time of design, this pattern shall be applied. It enables to change the communication interfaces that the pre-tested and verified PLC program must not be re-compiled or re-loaded.

---

**Applicability**  
*Describes the usage context of the pattern*

This pattern is used in the context of configurable data exchange between OPC UA servers of other systems and the integrated OPC UA client of the implementing system.

---

**Structure**  
*Describes the structure of the pattern*

![Software Pattern - Configurable Communication](pattern_config_communication.png)


---

**Actors**  
*Introduce the involved software entities*

This pattern consists of two defined types of actors, where the *ConnectionManager* exist once and the *Reader* entity exist as often as needed.

The *ConnectionManager* consists a list of *ConnectionHandle*. The length of the list is equal to the maximum count of parallel OPC UA connections. For each possible connection a *ConnectionConfig* is available, which is used to setup the connection partner. The connection configuration as well as the prepared block call list follows the specifications of OPC UA Client Blocks for IEC 61131-3, specified by PLC Open.

The *Reader* is a generic function block which can be configured in that way, that it can read REAL, DINT, BOOL, STRING or SERVICE information. The list of exchanged information base on the specifications from VDI/VDE/NAMUR 2658-4. Each *Reader* shall be related to one of the connection handles in the list. 

---

**Interaction**  
*Describes the interaction between the entities*

From the code point of view, the *ConnectionManager* contains a list of *ConnectionHandle* that is used to connect all the instantiated *Reader* blocks within the program. All the interaction between *ConnectionManager* and *Reader* is done via this list-variable.

Due to the relation of the *HandleIndex* of the *Reader* and the concrete connection, identified via this *HandleIndex*, the *ConnectionManager* establishs the list of related Readers after initializing the communication. This self configuration mechanism reduce the implementation effort. 

In the case of higher number of related Readers, a scheduling shall be neccesary. This scheduling is done by the *CommunicationManager*. It sends over the *ConnectionHandle* the command to read the configured data and after finishing this, the *CommunicationManager* pushs the token to read to one of the next Readers. 

---

**Consequences**  
*Pros and Cons of the pattern*

The advantage of this pattern is the ability to realize a configurable communication interface based on an open communication standard and without any vendor-specific configuration interfaces. Due to the configurability the already tested and verified PLC program containing this pattern, it must now be recompiled and reloaded for configuration changes. 

The disadvantage is the higher footprint of memory and processor capacities. 

The increased adaptability for information exchange comes at the cost of memory and performance.

---

**Implementation**  
*Hints for implementation of the pattern*

The exemplary TIA Portal source code will be published soon.

---

**Cross References**  
*References to other related patterns*

PLC Open OPC UA Client Blocks [Link](https://plcopen.org/downloads/plcopen-opc-ua-client-function-blocks-iec-61131-3-version-11)

---



