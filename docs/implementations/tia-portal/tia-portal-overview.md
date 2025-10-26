# TIA Portal Implementation Overview

This page lists all source code files of the exemplary TIA Portal implementation of the Automation Service Choreography Framework.

!!! danger "Disclaimer"

    The source code provided here is intended solely for illustration and to improve the comprehensibility of the mechanisms, concepts, and approaches described in the dissertation. It is explicitly not designed as production-ready or usable software library and should not be used in productive environments or safety-critical applications.  

    For further details, please refer to the license: [Link to license](../../license.md)

## Source Code Files

| Filename | Link | Description |
|----------|------|-------------|
| ASCF_ParticipantManager.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Base/ASCF_ParticipantManager.scl) | Base manager for choreography participants |
| MTPChoreographyParticipantManager.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/MTPChoreographyParticipantManager.scl) | MTP-based choreography participant manager |




### Configurable Communication (OPC UA Client/Server)

#### Main Function Blocks

| Filename | Link | Description |
|----------|------|-------------|
| ASCF_OpcUaClientServerManager.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/ASCF_OpcUaClientServerManager.scl) | OPC UA Client/Server communication manager |
| MTPOpcUaClientServerManager.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/MTPOpcUaClientServerManager.scl) | MTP OPC UA communication manager |

#### Internal Implementation

| Filename | Link | Description |
|----------|------|-------------|
| _ASCF_CC_OPCUACS_EnumConnectionHandleStates.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Communication/_ASCF_CC_OPCUACS_EnumConnectionHandleStates.scl) | Enumeration for connection handle states |
| _ASCF_CC_OPCUACS_ScheduleAlgorithmType1.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Communication/_ASCF_CC_OPCUACS_ScheduleAlgorithmType1.scl) | Scheduling algorithm type 1 |
| _ASCF_CC_OPCUACS_ScheduleAlgorithmType2.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Communication/_ASCF_CC_OPCUACS_ScheduleAlgorithmType2.scl) | Scheduling algorithm type 2 |
| ASCF_CC_OPCUACS_ConnectionConfig.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Communication/ASCF_CC_OPCUACS_ConnectionConfig.scl) | Connection configuration for OPC UA |
| ASCF_CC_OPCUACS_ConnectionHandle.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Communication/ASCF_CC_OPCUACS_ConnectionHandle.scl) | Connection handle for OPC UA |
| ASCF_CC_OPCUACS_ConnectionInterface.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Communication/ASCF_CC_OPCUACS_ConnectionInterface.scl) | Connection interface |
| ASCF_CC_OPCUACS_Connections.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Communication/ASCF_CC_OPCUACS_Connections.scl) | Connection management |
| ASCF_CC_OPCUACS_Connections_clean.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Communication/ASCF_CC_OPCUACS_Connections_clean.scl) | Clean connection implementation |
| ASCF_CC_OPCUACS_ConnectionStatus.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Communication/ASCF_CC_OPCUACS_ConnectionStatus.scl) | Connection status |
| ASCF_CC_OPCUACS_Constants.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Communication/ASCF_CC_OPCUACS_Constants.scl) | Constants for OPC UA communication |
| ASCF_CC_OPCUACS_EnumErrors.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Communication/ASCF_CC_OPCUACS_EnumErrors.scl) | Error codes for OPC UA |
| ASCF_CC_OPCUACS_QuerySchedule.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Communication/ASCF_CC_OPCUACS_QuerySchedule.scl) | Schedule query functionality |
| ASCF_CC_OPCUACS_Reader.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Communication/ASCF_CC_OPCUACS_Reader.scl) | OPC UA reader functionality |
| ASCF_CC_OPCUACS_ReaderConfig.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Communication/ASCF_CC_OPCUACS_ReaderConfig.scl) | Reader configuration |
| ASCF_CC_OPCUACS_ReaderStatus.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Communication/ASCF_CC_OPCUACS_ReaderStatus.scl) | Reader status |
| ASCF_CC_OPCUACS_ScheduleData.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Communication/ASCF_CC_OPCUACS_ScheduleData.scl) | Schedule data |
| ASCF_CC_OPCUACS_ScheduleDataType1.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Communication/ASCF_CC_OPCUACS_ScheduleDataType1.scl) | Schedule data type 1 |
| ASCF_CC_OPCUACS_ScheduleDataType2.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Communication/ASCF_CC_OPCUACS_ScheduleDataType2.scl) | Schedule data type 2 |
| ASCF_CC_OPCUACS_Scheduler.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Communication/ASCF_CC_OPCUACS_Scheduler.scl) | Communication scheduler |
| ASCF_CC_OPCUACS_Writer.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Communication/ASCF_CC_OPCUACS_Writer.scl) | OPC UA writer functionality |
| ASCF_CC_OPCUACS_WriterConfig.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Communication/ASCF_CC_OPCUACS_WriterConfig.scl) | Writer configuration |
| ASCF_CC_OPCUACS_WriterStatus.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Communication/ASCF_CC_OPCUACS_WriterStatus.scl) | Writer status |

### Configurable Logic

#### Main Function Blocks

| Filename | Link | Description |
|----------|------|-------------|
| ASCF_ConfigurableLogic.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/ASCF_ConfigurableLogic.scl) | Main function block for configurable logic functions |

#### Internal Implementation - Arithmetic Operations

| Filename | Link | Description |
|----------|------|-------------|
| ASCF_CL_10_ADD.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_10_ADD.scl) | Addition |
| ASCF_CL_11_SUB.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_11_SUB.scl) | Subtraction |
| ASCF_CL_12_MUL.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_12_MUL.scl) | Multiplication |
| ASCF_CL_13_DIV.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_13_DIV.scl) | Division |
| ASCF_CL_14_MOD.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_14_MOD.scl) | Modulo |

#### Internal Implementation - Logical Operations

| Filename | Link | Description |
|----------|------|-------------|
| ASCF_CL_30_NOT.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_30_NOT.scl) | Logical NOT |
| ASCF_CL_31_AND.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_31_AND.scl) | Logical AND |
| ASCF_CL_32_OR.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_32_OR.scl) | Logical OR |
| ASCF_CL_33_NAND.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_33_NAND.scl) | Logical NAND |
| ASCF_CL_34_NOR.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_34_NOR.scl) | Logical NOR |
| ASCF_CL_35_XOR.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_35_XOR.scl) | Logical XOR |
| ASCF_CL_36_XNOR.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_36_XNOR.scl) | Logical XNOR |
| ASCF_CL_37_FE.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_37_FE.scl) | Falling edge |
| ASCF_CL_38_RE.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_38_RE.scl) | Rising edge |

#### Internal Implementation - Comparison Operations

| Filename | Link | Description |
|----------|------|-------------|
| ASCF_CL_50_EE.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_50_EE.scl) | Equality |
| ASCF_CL_51_NE.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_51_NE.scl) | Not equal |
| ASCF_CL_52_GT.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_52_GT.scl) | Greater than |
| ASCF_CL_53_GTE.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_53_GTE.scl) | Greater than or equal |
| ASCF_CL_54_LT.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_54_LT.scl) | Less than |
| ASCF_CL_55_LTE.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_55_LTE.scl) | Less than or equal |
| ASCF_CL_56_EE_BIT.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_56_EE_BIT.scl) | Bit equality |

#### Internal Implementation - Control Structures

| Filename | Link | Description |
|----------|------|-------------|
| ASCF_CL_100_IF1.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_100_IF1.scl) | IF condition type 1 |
| ASCF_CL_101_IF2.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_101_IF2.scl) | IF condition type 2 |
| ASCF_CL_102_IF3.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_102_IF3.scl) | IF condition type 3 |
| ASCF_CL_103_IF4.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_103_IF4.scl) | IF condition type 4 |
| ASCF_CL_104_IF5.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_104_IF5.scl) | IF condition type 5 |
| ASCF_CL_105_IF6.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_105_IF6.scl) | IF condition type 6 |
| ASCF_CL_106_IF7.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_106_IF7.scl) | IF condition type 7 |
| ASCF_CL_107_IF8.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_107_IF8.scl) | IF condition type 8 |
| ASCF_CL_108_IF9.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_108_IF9.scl) | IF condition type 9 |

#### Internal Implementation - Data Types and Enumerations

| Filename | Link | Description |
|----------|------|-------------|
| ASCF_CL_ArgumentType.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_ArgumentType.scl) | Argument type definition |
| ASCF_CL_EnumErrors.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_EnumErrors.scl) | Error codes for configurable logic |
| ASCF_CL_EnumFunctionTypes.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_EnumFunctionTypes.scl) | Function type enumeration |
| ASCF_CL_EnumSourceTypes.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_EnumSourceTypes.scl) | Source type enumeration |
| ASCF_CL_FunctionType.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_FunctionType.scl) | Function type definition |
| ASCF_CL_FunctionTypeConfig.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_FunctionTypeConfig.scl) | Function type configuration |
| ASCF_CL_OutputType.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Configurable%20Logic/ASCF_CL_OutputType.scl) | Output type definition |





### External Leader Implementation

| Filename | Link | Description |
|----------|------|-------------|

| ASCF_ExternalLeader.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/ASCF_ExternalLeader.scl) | External leadership logic for choreography participants |


### Base Components and Utilities

| Filename | Link | Description |
|----------|------|-------------|
| ASCF_CalcWQC.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Base/ASCF_CalcWQC.scl) | Calculation of value quality codes |
| ASCF_EnumUnionTypes.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Base/ASCF_EnumUnionTypes.scl) | Enumeration types for union data structures |
| ASCF_GetValueOutputList.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Base/ASCF_GetValueOutputList.scl) | Helper function for value output lists |
| ASCF_GetVBoolOutputList.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Base/ASCF_GetVBoolOutputList.scl) | Extract boolean values from output lists |
| ASCF_GetVDIntOutputList.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Base/ASCF_GetVDIntOutputList.scl) | Extract DInt values from output lists |
| ASCF_GetVDWordOutputList.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Base/ASCF_GetVDWordOutputList.scl) | Extract DWord values from output lists |
| ASCF_GetVRealOutputList.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Base/ASCF_GetVRealOutputList.scl) | Extract Real values from output lists |
| ASCF_GetVStringOutputList.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Base/ASCF_GetVStringOutputList.scl) | Extract String values from output lists |
| ASCF_QualityCodes.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Base/ASCF_QualityCodes.scl) | Quality code definitions |
| ASCF_UnionType.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Base/ASCF_UnionType.scl) | Union data type for various value types |
| ASCF_WriteValue.scl | [View Source Code](../../../Part_4_ExampleCode/TIA-Portal/Base/ASCF_WriteValue.scl) | Helper function for writing values |
