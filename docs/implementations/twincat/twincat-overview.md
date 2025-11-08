# TwinCAT Implementation Overview

This page lists all source code files of the exemplary TwinCAT implementation of the Automation Service Choreography Framework.

!!! danger "Disclaimer"

    The source code provided here is intended solely for illustration and to improve the comprehensibility of the mechanisms, concepts, and approaches described in the dissertation. It is explicitly not designed as production-ready or usable software library and should not be used in productive environments or safety-critical applications.  

    For further details, please refer to the license: <a href="../../license.md" target="_blank">Link to license</a>


## Active Choreography Participant - Implementation

| Name | Link | Description |
|------|------|-------------|
| ASCF_ParticipantManager | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/ASCF_ParticipantManager.TcPOU" target="_blank">View</a> | Core participant manager for choreography coordination |
| MTPChoreographyParticipantManager | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/MTPChoreographyParticipantManager.TcDUT" target="_blank">View</a> | MTP-specific choreography participant data structure |





### Configurable Communication (OPC UA Client/Server)

#### Main Function Blocks

| Name | Link | Description |
|------|------|-------------|
| ASCF_OpcUaClientServerManager | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/ASCF_OpcUaClientServerManager.TcPOU" target="_blank">View</a> | OPC UA client-server communication manager |
| MTPOpcUaClientServerManager | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/MTPOpcUaClientServerManager.TcDUT" target="_blank">View</a> | MTP OPC UA client-server data structure |

#### Internal Implementation

| Name | Link | Description |
|------|------|-------------|
| ASCF_CC_OPCUACS_ConnectionConfig | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_ConnectionConfig.TcDUT" target="_blank">View</a> | OPC UA connection configuration |
| ASCF_CC_OPCUACS_ConnectionHandle | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_ConnectionHandle.TcDUT" target="_blank">View</a> | OPC UA connection handle |
| ASCF_CC_OPCUACS_ConnectionInterface | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_ConnectionInterface.TcDUT" target="_blank">View</a> | OPC UA connection interface |
| ASCF_CC_OPCUACS_Connections | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_Connections.TcPOU" target="_blank">View</a> | OPC UA connections manager |
| ASCF_CC_OPCUACS_ConnectionStatus | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_ConnectionStatus.TcDUT" target="_blank">View</a> | OPC UA connection status |
| ASCF_CC_OPCUACS_Constants | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_Constants.TcDUT" target="_blank">View</a> | OPC UA constants |
| ASCF_CC_OPCUACS_EnumConnectionHandleStates | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_EnumConnectionHandleStates.TcDUT" target="_blank">View</a> | Connection handle state enumeration |
| ASCF_CC_OPCUACS_EnumErrors | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_EnumErrors.TcDUT" target="_blank">View</a> | OPC UA error enumeration |
| ASCF_CC_OPCUACS_QuerySchedule | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_QuerySchedule.TcPOU" target="_blank">View</a> | Query schedule function |
| ASCF_CC_OPCUACS_Reader | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_Reader.TcPOU" target="_blank">View</a> | OPC UA reader function |
| ASCF_CC_OPCUACS_ReaderConfig | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_ReaderConfig.TcDUT" target="_blank">View</a> | Reader configuration |
| ASCF_CC_OPCUACS_ReaderStatus | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_ReaderStatus.TcDUT" target="_blank">View</a> | Reader status |
| ASCF_CC_OPCUACS_Reader_Interface | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_Reader_Interface.TcDUT" target="_blank">View</a> | Reader interface |
| ASCF_CC_OPCUACS_Reader_Internals | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_Reader_Internals.TcDUT" target="_blank">View</a> | Reader internal data |
| ASCF_CC_OPCUACS_Reader_Temp | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_Reader_Temp.TcDUT" target="_blank">View</a> | Reader temporary data |
| ASCF_CC_OPCUACS_Reader_Temp_Bool | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_Reader_Temp_Bool.TcDUT" target="_blank">View</a> | Boolean reader temporary data |
| ASCF_CC_OPCUACS_Reader_Temp_Dint | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_Reader_Temp_Dint.TcDUT" target="_blank">View</a> | Double integer reader temporary data |
| ASCF_CC_OPCUACS_Reader_Temp_Dword | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_Reader_Temp_Dword.TcDUT" target="_blank">View</a> | Double word reader temporary data |
| ASCF_CC_OPCUACS_Reader_Temp_Real | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_Reader_Temp_Real.TcDUT" target="_blank">View</a> | Real reader temporary data |
| ASCF_CC_OPCUACS_Reader_Temp_String | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_Reader_Temp_String.TcDUT" target="_blank">View</a> | String reader temporary data |
| ASCF_CC_OPCUACS_ScheduleAlgorithmType1 | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_ScheduleAlgorithmType1.TcPOU" target="_blank">View</a> | Schedule algorithm type 1 |
| ASCF_CC_OPCUACS_ScheduleAlgorithmType2 | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_ScheduleAlgorithmType2.TcPOU" target="_blank">View</a> | Schedule algorithm type 2 |
| ASCF_CC_OPCUACS_ScheduleData | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_ScheduleData.TcDUT" target="_blank">View</a> | Schedule data structure |
| ASCF_CC_OPCUACS_ScheduleDataType1 | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_ScheduleDataType1.TcDUT" target="_blank">View</a> | Schedule data type 1 |
| ASCF_CC_OPCUACS_ScheduleDataType2 | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_ScheduleDataType2.TcDUT" target="_blank">View</a> | Schedule data type 2 |
| ASCF_CC_OPCUACS_Scheduler | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_Scheduler.TcPOU" target="_blank">View</a> | OPC UA scheduler |
| ASCF_CC_OPCUACS_Writer | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_Writer.TcPOU" target="_blank">View</a> | OPC UA writer function |
| ASCF_CC_OPCUACS_WriterConfig | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_WriterConfig.TcDUT" target="_blank">View</a> | Writer configuration |
| ASCF_CC_OPCUACS_WriterStatus | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_WriterStatus.TcDUT" target="_blank">View</a> | Writer status |
| ASCF_CC_OPCUACS_Writer_Interface | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_Writer_Interface.TcDUT" target="_blank">View</a> | Writer interface |
| ASCF_CC_OPCUACS_Writer_Internals | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_Writer_Internals.TcDUT" target="_blank">View</a> | Writer internal data |
| ASCF_CC_OPCUACS_Writer_Temp | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_Writer_Temp.TcDUT" target="_blank">View</a> | Writer temporary data |
| ASCF_CC_OPCUACS_Writer_Temp_Bool | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_Writer_Temp_Bool.TcDUT" target="_blank">View</a> | Boolean writer temporary data |
| ASCF_CC_OPCUACS_Writer_Temp_Dint | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_Writer_Temp_Dint.TcDUT" target="_blank">View</a> | Double integer writer temporary data |
| ASCF_CC_OPCUACS_Writer_Temp_Dword | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_Writer_Temp_Dword.TcDUT" target="_blank">View</a> | Double word writer temporary data |
| ASCF_CC_OPCUACS_Writer_Temp_Real | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_Writer_Temp_Real.TcDUT" target="_blank">View</a> | Real writer temporary data |
| ASCF_CC_OPCUACS_Writer_Temp_String | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_Writer_Temp_String.TcDUT" target="_blank">View</a> | String writer temporary data |

### Configurable Logic

#### Main Function Blocks

| Name | Link | Description |
|------|------|-------------|
| ASCF_ConfigurableLogic | <a href="./https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Logic/ASCF_ConfigurableLogic.TcPOU" target="_blank">View</a> | Main configurable logic manager |


#### Internal Implementation - Arithmetic Operations

| Name | Link | Description |
|------|------|-------------|
| ASCF_CL_10_ADD | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Logic/ASCF_CL_10_ADD.TcPOU" target="_blank">View</a> | Addition operation |
| ASCF_CL_11_SUB | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Logic/ASCF_CL_11_SUB.TcPOU" target="_blank">View</a> | Subtraction operation |
| ASCF_CL_12_MUL | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Logic/ASCF_CL_12_MUL.TcPOU" target="_blank">View</a> | Multiplication operation |
| ASCF_CL_13_DIV | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Logic/ASCF_CL_13_DIV.TcPOU" target="_blank">View</a> | Division operation |
| ASCF_CL_14_MOD | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Logic/ASCF_CL_14_MOD.TcPOU" target="_blank">View</a> | Modulo operation |

#### Internal Implementation - Logical Operations

| Name | Link | Description |
|------|------|-------------|
| ASCF_CL_30_NOT | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Logic/ASCF_CL_30_NOT.TcPOU" target="_blank">View</a> | Logical NOT operation |
| ASCF_CL_31_AND | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Logic/ASCF_CL_31_AND.TcPOU" target="_blank">View</a> | Logical AND operation |
| ASCF_CL_32_OR | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Logic/ASCF_CL_32_OR.TcPOU" target="_blank">View</a> | Logical OR operation |
| ASCF_CL_33_NAND | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Logic/ASCF_CL_33_NAND.TcPOU" target="_blank">View</a> | Logical NAND operation |
| ASCF_CL_34_NOR | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Logic/ASCF_CL_34_NOR.TcPOU" target="_blank">View</a> | Logical NOR operation |
| ASCF_CL_35_XOR | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Logic/ASCF_CL_35_XOR.TcPOU" target="_blank">View</a> | Logical XOR operation |
| ASCF_CL_36_XNOR | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Logic/ASCF_CL_36_XNOR.TcPOU" target="_blank">View</a> | Logical XNOR operation |

#### Internal Implementation - Comparison Operations

| Name | Link | Description |
|------|------|-------------|
| ASCF_CL_37_FE | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Logic/ASCF_CL_37_FE.TcPOU" target="_blank">View</a> | Falling edge detection |
| ASCF_CL_38_RE | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Logic/ASCF_CL_38_RE.TcPOU" target="_blank">View</a> | Rising edge detection |
| ASCF_CL_50_EE | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Logic/ASCF_CL_50_EE.TcPOU" target="_blank">View</a> | Equal comparison |
| ASCF_CL_51_NE | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Logic/ASCF_CL_51_NE.TcPOU" target="_blank">View</a> | Not equal comparison |
| ASCF_CL_52_GT | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Logic/ASCF_CL_52_GT.TcPOU" target="_blank">View</a> | Greater than comparison |
| ASCF_CL_53_GTE | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Logic/ASCF_CL_53_GTE.TcPOU" target="_blank">View</a> | Greater than or equal comparison |
| ASCF_CL_54_LT | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Logic/ASCF_CL_54_LT.TcPOU" target="_blank">View</a> | Less than comparison |
| ASCF_CL_55_LTE | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Logic/ASCF_CL_55_LTE.TcPOU" target="_blank">View</a> | Less than or equal comparison |
| ASCF_CL_56_EE_BIT | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Logic/ASCF_CL_56_EE_BIT.TcPOU" target="_blank">View</a> | Bitwise equal comparison |

#### Internal Implementation - Control Structures

| Name | Link | Description |
|------|------|-------------|
| ASCF_CL_100_IF1 | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Logic/ASCF_CL_100_IF1.TcPOU" target="_blank">View</a> | Conditional logic function IF1 |
| ASCF_CL_101_IF2 | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Logic/ASCF_CL_101_IF2.TcPOU" target="_blank">View</a> | Conditional logic function IF2 |
| ASCF_CL_102_IF3 | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Logic/ASCF_CL_102_IF3.TcPOU" target="_blank">View</a> | Conditional logic function IF3 |
| ASCF_CL_103_IF4 | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Logic/ASCF_CL_103_IF4.TcPOU" target="_blank">View</a> | Conditional logic function IF4 |
| ASCF_CL_104_IF5 | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Logic/ASCF_CL_104_IF5.TcPOU" target="_blank">View</a> | Conditional logic function IF5 |
| ASCF_CL_105_IF6 | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Logic/ASCF_CL_105_IF6.TcPOU" target="_blank">View</a> | Conditional logic function IF6 |
| ASCF_CL_106_IF7 | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Logic/ASCF_CL_106_IF7.TcPOU" target="_blank">View</a> | Conditional logic function IF7 |
| ASCF_CL_107_IF8 | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Logic/ASCF_CL_107_IF8.TcPOU" target="_blank">View</a> | Conditional logic function IF8 |
| ASCF_CL_108_IF9 | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Logic/ASCF_CL_108_IF9.TcPOU" target="_blank">View</a> | Conditional logic function IF9 |

#### Internal Implementation - Data Types and Enumerations

| Name | Link | Description |
|------|------|-------------|
| ASCF_CL_ArgumentType | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Logic/ASCF_CL_ArgumentType.TcDUT" target="_blank">View</a> | Argument type definition |
| ASCF_CL_EnumErrors | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Logic/ASCF_CL_EnumErrors.TcDUT" target="_blank">View</a> | Configurable logic error enumeration |
| ASCF_CL_EnumFunctionTypes | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Logic/ASCF_CL_EnumFunctionTypes.TcDUT" target="_blank">View</a> | Function type enumeration |
| ASCF_CL_EnumSourceTypes | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Logic/ASCF_CL_EnumSourceTypes.TcDUT" target="_blank">View</a> | Source type enumeration |
| ASCF_CL_FunctionType | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Logic/ASCF_CL_FunctionType.TcDUT" target="_blank">View</a> | Function type definition |
| ASCF_CL_FunctionTypeConfig | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Logic/ASCF_CL_FunctionTypeConfig.TcDUT" target="_blank">View</a> | Function type configuration |
| ASCF_CL_OutputType | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Logic/ASCF_CL_OutputType.TcDUT" target="_blank">View</a> | Output type definition |
| ASCF_CL_OutputTypeConfig | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Configurable%20Logic/ASCF_CL_OutputTypeConfig.TcDUT" target="_blank">View</a> | Output type configuration |


### Base Components and Utilities

| Name | Link | Description |
|------|------|-------------|
| ASCF_CalcWQC | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Base/ASCF_CalcWQC.TcPOU" target="_blank">View</a> | Quality code calculation function |
| ASCF_EnumErrors | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Base/ASCF_EnumErrors.TcDUT" target="_blank">View</a> | Error code enumeration |
| ASCF_EnumUnionTypes | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Base/ASCF_EnumUnionTypes.TcDUT" target="_blank">View</a> | Union type enumeration |
| ASCF_GetValueOutputList | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Base/ASCF_GetValueOutputList.TcPOU" target="_blank">View</a> | Generic value output list retrieval |
| ASCF_GetVBoolOutputList | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Base/ASCF_GetVBoolOutputList.TcPOU" target="_blank">View</a> | Boolean value output list retrieval |
| ASCF_GetVDIntOutputList | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Base/ASCF_GetVDIntOutputList.TcPOU" target="_blank">View</a> | Double integer value output list retrieval |
| ASCF_GetVDWordOutputList | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Base/ASCF_GetVDWordOutputList.TcPOU" target="_blank">View</a> | Double word value output list retrieval |
| ASCF_GetVRealOutputList | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Base/ASCF_GetVRealOutputList.TcPOU" target="_blank">View</a> | Real value output list retrieval |
| ASCF_GetVStringOutputList | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Base/ASCF_GetVStringOutputList.TcPOU" target="_blank">View</a> | String value output list retrieval |
| ASCF_QualityCodes | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Base/ASCF_QualityCodes.TcDUT" target="_blank">View</a> | Quality code definitions |
| ASCF_State_Internals | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Base/ASCF_State_Internals.TcDUT" target="_blank">View</a> | Internal state data structure |
| ASCF_UnionType | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Base/ASCF_UnionType.TcDUT" target="_blank">View</a> | Union type data structure |
| ASCF_WriteValue | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Base/ASCF_WriteValue.TcPOU" target="_blank">View</a> | Value writing function |
| CreateDTL | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Utils/CreateDTL.TcPOU" target="_blank">View</a> | Date and time creation utility |
| DeltaDTL | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Utils/DeltaDTL.TcPOU" target="_blank">View</a> | Date and time delta calculation |
| DTL | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Utils/DTL.TcDUT" target="_blank">View</a> | Date and time data structure |
| DTL_to_TIME | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Utils/DTL_to_TIME.TcPOU" target="_blank">View</a> | Date-time to time conversion |
| SYS_TIME_Store_DTL | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/TwinCAT/Utils/SYS_TIME_Store_DTL.TcPOU" target="_blank">View</a> | System time storage utility |
