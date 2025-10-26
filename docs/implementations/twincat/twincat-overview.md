# TwinCAT Implementation Overview

This page lists all source code files of the exemplary TwinCAT implementation of the Automation Service Choreography Framework.

!!! danger "Disclaimer"

    The source code provided here is intended solely for illustration and to improve the comprehensibility of the mechanisms, concepts, and approaches described in the dissertation. It is explicitly not designed as production-ready or usable software library and should not be used in productive environments or safety-critical applications.  

    For further details, please refer to the license: [Link to license](../../license.md)


## Active Choreography Participant - Implementation

| Name | Link | Description |
|------|------|-------------|
| ASCF_ParticipantManager | [ASCF_ParticipantManager.TcPOU](../../../Part_4_ExampleCode/TwinCAT/ASCF_ParticipantManager.TcPOU) | Core participant manager for choreography coordination |
| MTPChoreographyParticipantManager | [MTPChoreographyParticipantManager.TcDUT](../../../Part_4_ExampleCode/TwinCAT/MTPChoreographyParticipantManager.TcDUT) | MTP-specific choreography participant data structure |





### Configurable Communication (OPC UA Client/Server)

#### Main Function Blocks

| Name | Link | Description |
|------|------|-------------|
| ASCF_OpcUaClientServerManager | [ASCF_OpcUaClientServerManager.TcPOU](../../../Part_4_ExampleCode/TwinCAT/ASCF_OpcUaClientServerManager.TcPOU) | OPC UA client-server communication manager |
| MTPOpcUaClientServerManager | [MTPOpcUaClientServerManager.TcDUT](../../../Part_4_ExampleCode/TwinCAT/MTPOpcUaClientServerManager.TcDUT) | MTP OPC UA client-server data structure |

#### Internal Implementation

| Name | Link | Description |
|------|------|-------------|
| ASCF_CC_OPCUACS_ConnectionConfig | [Configurable Communication/ASCF_CC_OPCUACS_ConnectionConfig.TcDUT](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_ConnectionConfig.TcDUT) | OPC UA connection configuration |
| ASCF_CC_OPCUACS_ConnectionHandle | [Configurable Communication/ASCF_CC_OPCUACS_ConnectionHandle.TcDUT](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_ConnectionHandle.TcDUT) | OPC UA connection handle |
| ASCF_CC_OPCUACS_ConnectionInterface | [Configurable Communication/ASCF_CC_OPCUACS_ConnectionInterface.TcDUT](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_ConnectionInterface.TcDUT) | OPC UA connection interface |
| ASCF_CC_OPCUACS_Connections | [Configurable Communication/ASCF_CC_OPCUACS_Connections.TcPOU](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_Connections.TcPOU) | OPC UA connections manager |
| ASCF_CC_OPCUACS_ConnectionStatus | [Configurable Communication/ASCF_CC_OPCUACS_ConnectionStatus.TcDUT](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_ConnectionStatus.TcDUT) | OPC UA connection status |
| ASCF_CC_OPCUACS_Constants | [Configurable Communication/ASCF_CC_OPCUACS_Constants.TcDUT](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_Constants.TcDUT) | OPC UA constants |
| ASCF_CC_OPCUACS_EnumConnectionHandleStates | [Configurable Communication/ASCF_CC_OPCUACS_EnumConnectionHandleStates.TcDUT](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_EnumConnectionHandleStates.TcDUT) | Connection handle state enumeration |
| ASCF_CC_OPCUACS_EnumErrors | [Configurable Communication/ASCF_CC_OPCUACS_EnumErrors.TcDUT](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_EnumErrors.TcDUT) | OPC UA error enumeration |
| ASCF_CC_OPCUACS_QuerySchedule | [Configurable Communication/ASCF_CC_OPCUACS_QuerySchedule.TcPOU](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_QuerySchedule.TcPOU) | Query schedule function |
| ASCF_CC_OPCUACS_Reader | [Configurable Communication/ASCF_CC_OPCUACS_Reader.TcPOU](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_Reader.TcPOU) | OPC UA reader function |
| ASCF_CC_OPCUACS_ReaderConfig | [Configurable Communication/ASCF_CC_OPCUACS_ReaderConfig.TcDUT](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_ReaderConfig.TcDUT) | Reader configuration |
| ASCF_CC_OPCUACS_ReaderStatus | [Configurable Communication/ASCF_CC_OPCUACS_ReaderStatus.TcDUT](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_ReaderStatus.TcDUT) | Reader status |
| ASCF_CC_OPCUACS_Reader_Interface | [Configurable Communication/ASCF_CC_OPCUACS_Reader_Interface.TcDUT](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_Reader_Interface.TcDUT) | Reader interface |
| ASCF_CC_OPCUACS_Reader_Internals | [Configurable Communication/ASCF_CC_OPCUACS_Reader_Internals.TcDUT](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_Reader_Internals.TcDUT) | Reader internal data |
| ASCF_CC_OPCUACS_Reader_Temp | [Configurable Communication/ASCF_CC_OPCUACS_Reader_Temp.TcDUT](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_Reader_Temp.TcDUT) | Reader temporary data |
| ASCF_CC_OPCUACS_Reader_Temp_Bool | [Configurable Communication/ASCF_CC_OPCUACS_Reader_Temp_Bool.TcDUT](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_Reader_Temp_Bool.TcDUT) | Boolean reader temporary data |
| ASCF_CC_OPCUACS_Reader_Temp_Dint | [Configurable Communication/ASCF_CC_OPCUACS_Reader_Temp_Dint.TcDUT](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_Reader_Temp_Dint.TcDUT) | Double integer reader temporary data |
| ASCF_CC_OPCUACS_Reader_Temp_Dword | [Configurable Communication/ASCF_CC_OPCUACS_Reader_Temp_Dword.TcDUT](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_Reader_Temp_Dword.TcDUT) | Double word reader temporary data |
| ASCF_CC_OPCUACS_Reader_Temp_Real | [Configurable Communication/ASCF_CC_OPCUACS_Reader_Temp_Real.TcDUT](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_Reader_Temp_Real.TcDUT) | Real reader temporary data |
| ASCF_CC_OPCUACS_Reader_Temp_String | [Configurable Communication/ASCF_CC_OPCUACS_Reader_Temp_String.TcDUT](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_Reader_Temp_String.TcDUT) | String reader temporary data |
| ASCF_CC_OPCUACS_ScheduleAlgorithmType1 | [Configurable Communication/ASCF_CC_OPCUACS_ScheduleAlgorithmType1.TcPOU](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_ScheduleAlgorithmType1.TcPOU) | Schedule algorithm type 1 |
| ASCF_CC_OPCUACS_ScheduleAlgorithmType2 | [Configurable Communication/ASCF_CC_OPCUACS_ScheduleAlgorithmType2.TcPOU](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_ScheduleAlgorithmType2.TcPOU) | Schedule algorithm type 2 |
| ASCF_CC_OPCUACS_ScheduleData | [Configurable Communication/ASCF_CC_OPCUACS_ScheduleData.TcDUT](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_ScheduleData.TcDUT) | Schedule data structure |
| ASCF_CC_OPCUACS_ScheduleDataType1 | [Configurable Communication/ASCF_CC_OPCUACS_ScheduleDataType1.TcDUT](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_ScheduleDataType1.TcDUT) | Schedule data type 1 |
| ASCF_CC_OPCUACS_ScheduleDataType2 | [Configurable Communication/ASCF_CC_OPCUACS_ScheduleDataType2.TcDUT](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_ScheduleDataType2.TcDUT) | Schedule data type 2 |
| ASCF_CC_OPCUACS_Scheduler | [Configurable Communication/ASCF_CC_OPCUACS_Scheduler.TcPOU](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_Scheduler.TcPOU) | OPC UA scheduler |
| ASCF_CC_OPCUACS_Writer | [Configurable Communication/ASCF_CC_OPCUACS_Writer.TcPOU](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_Writer.TcPOU) | OPC UA writer function |
| ASCF_CC_OPCUACS_WriterConfig | [Configurable Communication/ASCF_CC_OPCUACS_WriterConfig.TcDUT](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_WriterConfig.TcDUT) | Writer configuration |
| ASCF_CC_OPCUACS_WriterStatus | [Configurable Communication/ASCF_CC_OPCUACS_WriterStatus.TcDUT](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_WriterStatus.TcDUT) | Writer status |
| ASCF_CC_OPCUACS_Writer_Interface | [Configurable Communication/ASCF_CC_OPCUACS_Writer_Interface.TcDUT](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_Writer_Interface.TcDUT) | Writer interface |
| ASCF_CC_OPCUACS_Writer_Internals | [Configurable Communication/ASCF_CC_OPCUACS_Writer_Internals.TcDUT](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_Writer_Internals.TcDUT) | Writer internal data |
| ASCF_CC_OPCUACS_Writer_Temp | [Configurable Communication/ASCF_CC_OPCUACS_Writer_Temp.TcDUT](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_Writer_Temp.TcDUT) | Writer temporary data |
| ASCF_CC_OPCUACS_Writer_Temp_Bool | [Configurable Communication/ASCF_CC_OPCUACS_Writer_Temp_Bool.TcDUT](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_Writer_Temp_Bool.TcDUT) | Boolean writer temporary data |
| ASCF_CC_OPCUACS_Writer_Temp_Dint | [Configurable Communication/ASCF_CC_OPCUACS_Writer_Temp_Dint.TcDUT](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_Writer_Temp_Dint.TcDUT) | Double integer writer temporary data |
| ASCF_CC_OPCUACS_Writer_Temp_Dword | [Configurable Communication/ASCF_CC_OPCUACS_Writer_Temp_Dword.TcDUT](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_Writer_Temp_Dword.TcDUT) | Double word writer temporary data |
| ASCF_CC_OPCUACS_Writer_Temp_Real | [Configurable Communication/ASCF_CC_OPCUACS_Writer_Temp_Real.TcDUT](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_Writer_Temp_Real.TcDUT) | Real writer temporary data |
| ASCF_CC_OPCUACS_Writer_Temp_String | [Configurable Communication/ASCF_CC_OPCUACS_Writer_Temp_String.TcDUT](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Communication/ASCF_CC_OPCUACS_Writer_Temp_String.TcDUT) | String writer temporary data |

### Configurable Logic

#### Main Function Blocks

| Name | Link | Description |
|------|------|-------------|
| ASCF_ConfigurableLogic | [Configurable Logic/ASCF_ConfigurableLogic.TcPOU](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Logic/ASCF_ConfigurableLogic.TcPOU) | Main configurable logic manager |


#### Internal Implementation - Arithmetic Operations

| Name | Link | Description |
|------|------|-------------|
| ASCF_CL_10_ADD | [Configurable Logic/ASCF_CL_10_ADD.TcPOU](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Logic/ASCF_CL_10_ADD.TcPOU) | Addition operation |
| ASCF_CL_11_SUB | [Configurable Logic/ASCF_CL_11_SUB.TcPOU](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Logic/ASCF_CL_11_SUB.TcPOU) | Subtraction operation |
| ASCF_CL_12_MUL | [Configurable Logic/ASCF_CL_12_MUL.TcPOU](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Logic/ASCF_CL_12_MUL.TcPOU) | Multiplication operation |
| ASCF_CL_13_DIV | [Configurable Logic/ASCF_CL_13_DIV.TcPOU](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Logic/ASCF_CL_13_DIV.TcPOU) | Division operation |
| ASCF_CL_14_MOD | [Configurable Logic/ASCF_CL_14_MOD.TcPOU](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Logic/ASCF_CL_14_MOD.TcPOU) | Modulo operation |

#### Internal Implementation - Logical Operations

| Name | Link | Description |
|------|------|-------------|
| ASCF_CL_30_NOT | [Configurable Logic/ASCF_CL_30_NOT.TcPOU](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Logic/ASCF_CL_30_NOT.TcPOU) | Logical NOT operation |
| ASCF_CL_31_AND | [Configurable Logic/ASCF_CL_31_AND.TcPOU](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Logic/ASCF_CL_31_AND.TcPOU) | Logical AND operation |
| ASCF_CL_32_OR | [Configurable Logic/ASCF_CL_32_OR.TcPOU](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Logic/ASCF_CL_32_OR.TcPOU) | Logical OR operation |
| ASCF_CL_33_NAND | [Configurable Logic/ASCF_CL_33_NAND.TcPOU](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Logic/ASCF_CL_33_NAND.TcPOU) | Logical NAND operation |
| ASCF_CL_34_NOR | [Configurable Logic/ASCF_CL_34_NOR.TcPOU](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Logic/ASCF_CL_34_NOR.TcPOU) | Logical NOR operation |
| ASCF_CL_35_XOR | [Configurable Logic/ASCF_CL_35_XOR.TcPOU](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Logic/ASCF_CL_35_XOR.TcPOU) | Logical XOR operation |
| ASCF_CL_36_XNOR | [Configurable Logic/ASCF_CL_36_XNOR.TcPOU](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Logic/ASCF_CL_36_XNOR.TcPOU) | Logical XNOR operation |

#### Internal Implementation - Comparison Operations

| Name | Link | Description |
|------|------|-------------|
| ASCF_CL_37_FE | [Configurable Logic/ASCF_CL_37_FE.TcPOU](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Logic/ASCF_CL_37_FE.TcPOU) | Falling edge detection |
| ASCF_CL_38_RE | [Configurable Logic/ASCF_CL_38_RE.TcPOU](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Logic/ASCF_CL_38_RE.TcPOU) | Rising edge detection |
| ASCF_CL_50_EE | [Configurable Logic/ASCF_CL_50_EE.TcPOU](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Logic/ASCF_CL_50_EE.TcPOU) | Equal comparison |
| ASCF_CL_51_NE | [Configurable Logic/ASCF_CL_51_NE.TcPOU](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Logic/ASCF_CL_51_NE.TcPOU) | Not equal comparison |
| ASCF_CL_52_GT | [Configurable Logic/ASCF_CL_52_GT.TcPOU](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Logic/ASCF_CL_52_GT.TcPOU) | Greater than comparison |
| ASCF_CL_53_GTE | [Configurable Logic/ASCF_CL_53_GTE.TcPOU](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Logic/ASCF_CL_53_GTE.TcPOU) | Greater than or equal comparison |
| ASCF_CL_54_LT | [Configurable Logic/ASCF_CL_54_LT.TcPOU](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Logic/ASCF_CL_54_LT.TcPOU) | Less than comparison |
| ASCF_CL_55_LTE | [Configurable Logic/ASCF_CL_55_LTE.TcPOU](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Logic/ASCF_CL_55_LTE.TcPOU) | Less than or equal comparison |
| ASCF_CL_56_EE_BIT | [Configurable Logic/ASCF_CL_56_EE_BIT.TcPOU](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Logic/ASCF_CL_56_EE_BIT.TcPOU) | Bitwise equal comparison |

#### Internal Implementation - Control Structures

| Name | Link | Description |
|------|------|-------------|
| ASCF_CL_100_IF1 | [Configurable Logic/ASCF_CL_100_IF1.TcPOU](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Logic/ASCF_CL_100_IF1.TcPOU) | Conditional logic function IF1 |
| ASCF_CL_101_IF2 | [Configurable Logic/ASCF_CL_101_IF2.TcPOU](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Logic/ASCF_CL_101_IF2.TcPOU) | Conditional logic function IF2 |
| ASCF_CL_102_IF3 | [Configurable Logic/ASCF_CL_102_IF3.TcPOU](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Logic/ASCF_CL_102_IF3.TcPOU) | Conditional logic function IF3 |
| ASCF_CL_103_IF4 | [Configurable Logic/ASCF_CL_103_IF4.TcPOU](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Logic/ASCF_CL_103_IF4.TcPOU) | Conditional logic function IF4 |
| ASCF_CL_104_IF5 | [Configurable Logic/ASCF_CL_104_IF5.TcPOU](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Logic/ASCF_CL_104_IF5.TcPOU) | Conditional logic function IF5 |
| ASCF_CL_105_IF6 | [Configurable Logic/ASCF_CL_105_IF6.TcPOU](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Logic/ASCF_CL_105_IF6.TcPOU) | Conditional logic function IF6 |
| ASCF_CL_106_IF7 | [Configurable Logic/ASCF_CL_106_IF7.TcPOU](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Logic/ASCF_CL_106_IF7.TcPOU) | Conditional logic function IF7 |
| ASCF_CL_107_IF8 | [Configurable Logic/ASCF_CL_107_IF8.TcPOU](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Logic/ASCF_CL_107_IF8.TcPOU) | Conditional logic function IF8 |
| ASCF_CL_108_IF9 | [Configurable Logic/ASCF_CL_108_IF9.TcPOU](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Logic/ASCF_CL_108_IF9.TcPOU) | Conditional logic function IF9 |

#### Internal Implementation - Data Types and Enumerations

| Name | Link | Description |
|------|------|-------------|
| ASCF_CL_ArgumentType | [Configurable Logic/ASCF_CL_ArgumentType.TcDUT](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Logic/ASCF_CL_ArgumentType.TcDUT) | Argument type definition |
| ASCF_CL_EnumErrors | [Configurable Logic/ASCF_CL_EnumErrors.TcDUT](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Logic/ASCF_CL_EnumErrors.TcDUT) | Configurable logic error enumeration |
| ASCF_CL_EnumFunctionTypes | [Configurable Logic/ASCF_CL_EnumFunctionTypes.TcDUT](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Logic/ASCF_CL_EnumFunctionTypes.TcDUT) | Function type enumeration |
| ASCF_CL_EnumSourceTypes | [Configurable Logic/ASCF_CL_EnumSourceTypes.TcDUT](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Logic/ASCF_CL_EnumSourceTypes.TcDUT) | Source type enumeration |
| ASCF_CL_FunctionType | [Configurable Logic/ASCF_CL_FunctionType.TcDUT](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Logic/ASCF_CL_FunctionType.TcDUT) | Function type definition |
| ASCF_CL_FunctionTypeConfig | [Configurable Logic/ASCF_CL_FunctionTypeConfig.TcDUT](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Logic/ASCF_CL_FunctionTypeConfig.TcDUT) | Function type configuration |
| ASCF_CL_OutputType | [Configurable Logic/ASCF_CL_OutputType.TcDUT](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Logic/ASCF_CL_OutputType.TcDUT) | Output type definition |
| ASCF_CL_OutputTypeConfig | [Configurable Logic/ASCF_CL_OutputTypeConfig.TcDUT](../../../Part_4_ExampleCode/TwinCAT/Configurable%20Logic/ASCF_CL_OutputTypeConfig.TcDUT) | Output type configuration |


### Base Components and Utilities

| Name | Link | Description |
|------|------|-------------|
| ASCF_CalcWQC | [Base/ASCF_CalcWQC.TcPOU](../../../Part_4_ExampleCode/TwinCAT/Base/ASCF_CalcWQC.TcPOU) | Quality code calculation function |
| ASCF_EnumErrors | [Base/ASCF_EnumErrors.TcDUT](../../../Part_4_ExampleCode/TwinCAT/Base/ASCF_EnumErrors.TcDUT) | Error code enumeration |
| ASCF_EnumUnionTypes | [Base/ASCF_EnumUnionTypes.TcDUT](../../../Part_4_ExampleCode/TwinCAT/Base/ASCF_EnumUnionTypes.TcDUT) | Union type enumeration |
| ASCF_GetValueOutputList | [Base/ASCF_GetValueOutputList.TcPOU](../../../Part_4_ExampleCode/TwinCAT/Base/ASCF_GetValueOutputList.TcPOU) | Generic value output list retrieval |
| ASCF_GetVBoolOutputList | [Base/ASCF_GetVBoolOutputList.TcPOU](../../../Part_4_ExampleCode/TwinCAT/Base/ASCF_GetVBoolOutputList.TcPOU) | Boolean value output list retrieval |
| ASCF_GetVDIntOutputList | [Base/ASCF_GetVDIntOutputList.TcPOU](../../../Part_4_ExampleCode/TwinCAT/Base/ASCF_GetVDIntOutputList.TcPOU) | Double integer value output list retrieval |
| ASCF_GetVDWordOutputList | [Base/ASCF_GetVDWordOutputList.TcPOU](../../../Part_4_ExampleCode/TwinCAT/Base/ASCF_GetVDWordOutputList.TcPOU) | Double word value output list retrieval |
| ASCF_GetVRealOutputList | [Base/ASCF_GetVRealOutputList.TcPOU](../../../Part_4_ExampleCode/TwinCAT/Base/ASCF_GetVRealOutputList.TcPOU) | Real value output list retrieval |
| ASCF_GetVStringOutputList | [Base/ASCF_GetVStringOutputList.TcPOU](../../../Part_4_ExampleCode/TwinCAT/Base/ASCF_GetVStringOutputList.TcPOU) | String value output list retrieval |
| ASCF_QualityCodes | [Base/ASCF_QualityCodes.TcDUT](../../../Part_4_ExampleCode/TwinCAT/Base/ASCF_QualityCodes.TcDUT) | Quality code definitions |
| ASCF_State_Internals | [Base/ASCF_State_Internals.TcDUT](../../../Part_4_ExampleCode/TwinCAT/Base/ASCF_State_Internals.TcDUT) | Internal state data structure |
| ASCF_UnionType | [Base/ASCF_UnionType.TcDUT](../../../Part_4_ExampleCode/TwinCAT/Base/ASCF_UnionType.TcDUT) | Union type data structure |
| ASCF_WriteValue | [Base/ASCF_WriteValue.TcPOU](../../../Part_4_ExampleCode/TwinCAT/Base/ASCF_WriteValue.TcPOU) | Value writing function |
| CreateDTL | [Utils/CreateDTL.TcPOU](../../../Part_4_ExampleCode/TwinCAT/Utils/CreateDTL.TcPOU) | Date and time creation utility |
| DeltaDTL | [Utils/DeltaDTL.TcPOU](../../../Part_4_ExampleCode/TwinCAT/Utils/DeltaDTL.TcPOU) | Date and time delta calculation |
| DTL | [Utils/DTL.TcDUT](../../../Part_4_ExampleCode/TwinCAT/Utils/DTL.TcDUT) | Date and time data structure |
| DTL_to_TIME | [Utils/DTL_to_TIME.TcPOU](../../../Part_4_ExampleCode/TwinCAT/Utils/DTL_to_TIME.TcPOU) | Date-time to time conversion |
| SYS_TIME_Store_DTL | [Utils/SYS_TIME_Store_DTL.TcPOU](../../../Part_4_ExampleCode/TwinCAT/Utils/SYS_TIME_Store_DTL.TcPOU) | System time storage utility |
