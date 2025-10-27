# TIA Portal Implementation Overview

This page lists all source code files of the exemplary TIA Portal implementation of the Automation Service Choreography Framework.

!!! danger "Disclaimer"

    The source code provided here is intended solely for illustration and to improve the comprehensibility of the mechanisms, concepts, and approaches described in the dissertation. It is explicitly not designed as production-ready or usable software library and should not be used in productive environments or safety-critical applications.  

    For further details, please refer to the license: <a href="../../license.md" target="_blank">Link to license</a>




## Source Code Files

| Filename | Link | Description |
|----------|------|-------------|
| ASCF_ParticipantManager.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Base/ASCF_ParticipantManager.scl" target="_blank">View</a> | Base manager for choreography participants |
| MTPChoreographyParticipantManager.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/MTPChoreographyParticipantManager.scl" target="_blank">View</a> | MTP-based choreography participant manager |




### Configurable Communication (OPC UA Client/Server)

#### Main Function Blocks

| Filename | Link | Description |
|----------|------|-------------|
| ASCF_OpcUaClientServerManager.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/ASCF_OpcUaClientServerManager.scl" target="_blank">View</a> | OPC UA Client/Server communication manager |
| MTPOpcUaClientServerManager.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/MTPOpcUaClientServerManager.scl" target="_blank">View</a> | MTP OPC UA communication manager |

#### Internal Implementation

| Filename | Link | Description |
|----------|------|-------------|
| _ASCF_CC_OPCUACS_EnumConnectionHandleStates.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Communication/_ASCF_CC_OPCUACS_EnumConnectionHandleStates.scl" target="_blank">View</a> | Enumeration for connection handle states |
| _ASCF_CC_OPCUACS_ScheduleAlgorithmType1.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Communication/_ASCF_CC_OPCUACS_ScheduleAlgorithmType1.scl" target="_blank">View</a> | Scheduling algorithm type 1 |
| _ASCF_CC_OPCUACS_ScheduleAlgorithmType2.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Communication/_ASCF_CC_OPCUACS_ScheduleAlgorithmType2.scl" target="_blank">View</a> | Scheduling algorithm type 2 |
| ASCF_CC_OPCUACS_ConnectionConfig.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Communication/ASCF_CC_OPCUACS_ConnectionConfig.scl" target="_blank">View</a> | Connection configuration for OPC UA |
| ASCF_CC_OPCUACS_ConnectionHandle.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Communication/ASCF_CC_OPCUACS_ConnectionHandle.scl" target="_blank">View</a> | Connection handle for OPC UA |
| ASCF_CC_OPCUACS_ConnectionInterface.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Communication/ASCF_CC_OPCUACS_ConnectionInterface.scl" target="_blank">View</a> | Connection interface |
| ASCF_CC_OPCUACS_Connections.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Communication/ASCF_CC_OPCUACS_Connections.scl" target="_blank">View</a> | Connection management |
| ASCF_CC_OPCUACS_Connections_clean.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Communication/ASCF_CC_OPCUACS_Connections_clean.scl" target="_blank">View</a> | Clean connection implementation |
| ASCF_CC_OPCUACS_ConnectionStatus.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Communication/ASCF_CC_OPCUACS_ConnectionStatus.scl" target="_blank">View</a> | Connection status |
| ASCF_CC_OPCUACS_Constants.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Communication/ASCF_CC_OPCUACS_Constants.scl" target="_blank">View</a> | Constants for OPC UA communication |
| ASCF_CC_OPCUACS_EnumErrors.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Communication/ASCF_CC_OPCUACS_EnumErrors.scl" target="_blank">View</a> | Error codes for OPC UA |
| ASCF_CC_OPCUACS_QuerySchedule.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Communication/ASCF_CC_OPCUACS_QuerySchedule.scl" target="_blank">View</a> | Schedule query functionality |
| ASCF_CC_OPCUACS_Reader.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Communication/ASCF_CC_OPCUACS_Reader.scl" target="_blank">View</a> | OPC UA reader functionality |
| ASCF_CC_OPCUACS_ReaderConfig.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Communication/ASCF_CC_OPCUACS_ReaderConfig.scl" target="_blank">View</a> | Reader configuration |
| ASCF_CC_OPCUACS_ReaderStatus.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Communication/ASCF_CC_OPCUACS_ReaderStatus.scl" target="_blank">View</a> | Reader status |
| ASCF_CC_OPCUACS_ScheduleData.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Communication/ASCF_CC_OPCUACS_ScheduleData.scl" target="_blank">View</a> | Schedule data |
| ASCF_CC_OPCUACS_ScheduleDataType1.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Communication/ASCF_CC_OPCUACS_ScheduleDataType1.scl" target="_blank">View</a> | Schedule data type 1 |
| ASCF_CC_OPCUACS_ScheduleDataType2.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Communication/ASCF_CC_OPCUACS_ScheduleDataType2.scl" target="_blank">View</a> | Schedule data type 2 |
| ASCF_CC_OPCUACS_Scheduler.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Communication/ASCF_CC_OPCUACS_Scheduler.scl" target="_blank">View</a> | Communication scheduler |
| ASCF_CC_OPCUACS_Writer.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Communication/ASCF_CC_OPCUACS_Writer.scl" target="_blank">View</a> | OPC UA writer functionality |
| ASCF_CC_OPCUACS_WriterConfig.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Communication/ASCF_CC_OPCUACS_WriterConfig.scl" target="_blank">View</a> | Writer configuration |
| ASCF_CC_OPCUACS_WriterStatus.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Communication/ASCF_CC_OPCUACS_WriterStatus.scl" target="_blank">View</a> | Writer status |

### Configurable Logic

#### Main Function Blocks

| Filename | Link | Description |
|----------|------|-------------|
| ASCF_ConfigurableLogic.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/ASCF_ConfigurableLogic.scl" target="_blank">View</a> | Main function block for configurable logic functions |

#### Internal Implementation - Arithmetic Operations

| Filename | Link | Description |
|----------|------|-------------|
| ASCF_CL_10_ADD.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_10_ADD.scl" target="_blank">View</a> | Addition |
| ASCF_CL_11_SUB.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_11_SUB.scl" target="_blank">View</a> | Subtraction |
| ASCF_CL_12_MUL.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_12_MUL.scl" target="_blank">View</a> | Multiplication |
| ASCF_CL_13_DIV.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_13_DIV.scl" target="_blank">View</a> | Division |
| ASCF_CL_14_MOD.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_14_MOD.scl" target="_blank">View</a> | Modulo |

#### Internal Implementation - Logical Operations

| Filename | Link | Description |
|----------|------|-------------|
| ASCF_CL_30_NOT.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_30_NOT.scl" target="_blank">View</a> | Logical NOT |
| ASCF_CL_31_AND.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_31_AND.scl" target="_blank">View</a> | Logical AND |
| ASCF_CL_32_OR.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_32_OR.scl" target="_blank">View</a> | Logical OR |
| ASCF_CL_33_NAND.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_33_NAND.scl" target="_blank">View</a> | Logical NAND |
| ASCF_CL_34_NOR.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_34_NOR.scl" target="_blank">View</a> | Logical NOR |
| ASCF_CL_35_XOR.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_35_XOR.scl" target="_blank">View</a> | Logical XOR |
| ASCF_CL_36_XNOR.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_36_XNOR.scl" target="_blank">View</a> | Logical XNOR |
| ASCF_CL_37_FE.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_37_FE.scl" target="_blank">View</a> | Falling edge |
| ASCF_CL_38_RE.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_38_RE.scl" target="_blank">View</a> | Rising edge |

#### Internal Implementation - Comparison Operations

| Filename | Link | Description |
|----------|------|-------------|
| ASCF_CL_50_EE.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_50_EE.scl" target="_blank">View</a> | Equality |
| ASCF_CL_51_NE.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_51_NE.scl" target="_blank">View</a> | Not equal |
| ASCF_CL_52_GT.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_52_GT.scl" target="_blank">View</a> | Greater than |
| ASCF_CL_53_GTE.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_53_GTE.scl" target="_blank">View</a> | Greater than or equal |
| ASCF_CL_54_LT.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_54_LT.scl" target="_blank">View</a> | Less than |
| ASCF_CL_55_LTE.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_55_LTE.scl" target="_blank">View</a> | Less than or equal |
| ASCF_CL_56_EE_BIT.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_56_EE_BIT.scl" target="_blank">View</a> | Bit equality |

#### Internal Implementation - Control Structures

| Filename | Link | Description |
|----------|------|-------------|
| ASCF_CL_100_IF1.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_100_IF1.scl" target="_blank">View</a> | IF condition type 1 |
| ASCF_CL_101_IF2.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_101_IF2.scl" target="_blank">View</a> | IF condition type 2 |
| ASCF_CL_102_IF3.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_102_IF3.scl" target="_blank">View</a> | IF condition type 3 |
| ASCF_CL_103_IF4.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_103_IF4.scl" target="_blank">View</a> | IF condition type 4 |
| ASCF_CL_104_IF5.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_104_IF5.scl" target="_blank">View</a> | IF condition type 5 |
| ASCF_CL_105_IF6.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_105_IF6.scl" target="_blank">View</a> | IF condition type 6 |
| ASCF_CL_106_IF7.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_106_IF7.scl" target="_blank">View</a> | IF condition type 7 |
| ASCF_CL_107_IF8.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_107_IF8.scl" target="_blank">View</a> | IF condition type 8 |
| ASCF_CL_108_IF9.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_108_IF9.scl" target="_blank">View</a> | IF condition type 9 |

#### Internal Implementation - Data Types and Enumerations

| Filename | Link | Description |
|----------|------|-------------|
| ASCF_CL_ArgumentType.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_ArgumentType.scl" target="_blank">View</a> | Argument type definition |
| ASCF_CL_EnumErrors.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_EnumErrors.scl" target="_blank">View</a> | Error codes for configurable logic |
| ASCF_CL_EnumFunctionTypes.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_EnumFunctionTypes.scl" target="_blank">View</a> | Function type enumeration |
| ASCF_CL_EnumSourceTypes.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_EnumSourceTypes.scl" target="_blank">View</a> | Source type enumeration |
| ASCF_CL_FunctionType.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_FunctionType.scl" target="_blank">View</a> | Function type definition |
| ASCF_CL_FunctionTypeConfig.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_FunctionTypeConfig.scl" target="_blank">View</a> | Function type configuration |
| ASCF_CL_OutputType.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_OutputType.scl" target="_blank">View</a> | Output type definition |





### External Leader Implementation

| Filename | Link | Description |
|----------|------|-------------|
| ASCF_ExternalLeader.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/ASCF_ExternalLeader.scl" target="_blank">View</a> | External leadership logic for choreography participants |


### Base Components and Utilities

| Filename | Link | Description |
|----------|------|-------------|
| ASCF_CalcWQC.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Base/ASCF_CalcWQC.scl" target="_blank">View</a> | Calculation of value quality codes |
| ASCF_EnumUnionTypes.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Base/ASCF_EnumUnionTypes.scl" target="_blank">View</a> | Enumeration types for union data structures |
| ASCF_GetValueOutputList.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Base/ASCF_GetValueOutputList.scl" target="_blank">View</a> | Helper function for value output lists |
| ASCF_GetVBoolOutputList.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Base/ASCF_GetVBoolOutputList.scl" target="_blank">View</a> | Extract boolean values from output lists |
| ASCF_GetVDIntOutputList.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Base/ASCF_GetVDIntOutputList.scl" target="_blank">View</a> | Extract DInt values from output lists |
| ASCF_GetVDWordOutputList.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Base/ASCF_GetVDWordOutputList.scl" target="_blank">View</a> | Extract DWord values from output lists |
| ASCF_GetVRealOutputList.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Base/ASCF_GetVRealOutputList.scl" target="_blank">View</a> | Extract Real values from output lists |
| ASCF_GetVStringOutputList.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Base/ASCF_GetVStringOutputList.scl" target="_blank">View</a> | Extract String values from output lists |
| ASCF_QualityCodes.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Base/ASCF_QualityCodes.scl" target="_blank">View</a> | Quality code definitions |
| ASCF_UnionType.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Base/ASCF_UnionType.scl" target="_blank">View</a> | Union data type for various value types |
| ASCF_WriteValue.scl | <a href="https://github.com/stan1025/AutomationServiceChoreography/tree/master/Part_4_ExampleCode/TIA-Portal/Base/ASCF_WriteValue.scl" target="_blank">View</a> | Helper function for writing values |
