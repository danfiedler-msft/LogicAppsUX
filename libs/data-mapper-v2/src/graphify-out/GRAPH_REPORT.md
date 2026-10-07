# Graph Report - src  (2026-10-07)

## Corpus Check
- 143 files · ~77,576 words
- Verdict: corpus is large enough that graph structure adds value.

## Summary
- 1473 nodes · 4683 edges · 76 communities (67 shown, 9 thin omitted)
- Extraction: 98% EXTRACTED · 2% INFERRED · 0% AMBIGUOUS · INFERRED: 74 edges (avg confidence: 0.85)
- Token cost: 0 input · 0 output

## Graph Freshness
- Built from commit: `04df5b5c`
- Run `git rev-parse HEAD` and compare to check if the graph is stale.
- Run `graphify update .` after code changes (no API cost).

## Community Hubs (Navigation)
- MapDefinitionDeserializer
- MapDefinitionSerializer.ts
- images/FunctionIcons/FunctionIcons.tsx
- images/FunctionIcons/DataType16Icons.tsx
- images/FunctionIcons/DataType24Icons.tsx
- components/functionConfigurationMenu/inputTab/inputTab.tsx
- core/state/PanelSlice.ts
- src/core/state/Store.ts
- Schema.Utils.ts
- core/state/DataMapSlice.ts
- DataMap.Utils.ts
- TrieTree
- components/common/fileDropdownTree/FileDropdownTree.tsx
- MapChecker.Utils.ts
- core/state/Store.ts
- src/components/schema/SchemaPanel.tsx
- components/test/TestPanel.tsx
- Edge.Utils.ts
- Function.Utils.ts
- components/schema/SchemaPanel.tsx
- isFunctionNode
- components/canvas/ReactFlow.tsx
- src/core/state/__test__/DataMapSlice.spec.ts
- Icon.Utils.tsx
- ThemeConect.ts
- src/components/functionConfigurationMenu/inputDropdown/InputDropdown.tsx
- components/common/reactflow/FunctionNode.tsx
- ReactFlow.Util.ts
- components/canvas/useReactflowStates.ts
- src/core/state/selectors/selectors.ts
- models/index.ts
- RootState
- src/components/functionsPanel/FunctionPanel.tsx
- src/core/state/DataMapSlice.ts
- src/components/functionConfigurationMenu/inputTab/inputTab.tsx
- DataMapperDesignerProvider.tsx
- ref_fluentui_react_icons
- src/mapHandling/__test__/MapDefinitionSerializer.spec.ts
- intl-test-helper.tsx
- utils/reactFlowTesting/NodeInspector.tsx
- DataMapDataProvider.tsx
- Svg.d.ts
- IDataMapperFileService
- isSchemaNodeExtended
- src/components/canvas/ReactFlow.tsx
- src/images/FunctionIcons/DataType16Icons.tsx
- src/images/FunctionIcons/DataType24Icons.tsx
- Connection.Utils.ts
- src/components/schema/SchemaPanelBody.tsx
- src/components/schema/tree/SchemaTreeNode.tsx
- TrieTree
- FunctionData
- ref_fluentui_react_components
- components/common/selector/__test__/FileSelector.spec.tsx
- src/components/functionConfigurationMenu/functionConfigurationPopover.tsx
- ext_logic_apps_shared_src_index_ts
- src/core/state/ModalSlice.ts
- DataMapperDesigner.tsx
- core/index.ts
- src/components/commandBar/EditorCommandBar.tsx
- components/commandBar/EditorCommandBar.tsx
- ref_react
- src/components/common/reactflow/FunctionNode.tsx
- src/components/common/selector/__test__/FileSelector.spec.tsx
- src/core/state/FunctionSlice.ts
- MapMetadataSerializer.ts
- ref_xyflow_react
- src/core/state/ErrorsSlice.ts
- getConnectedTargetSchemaNodes
- ui/hooks/useAutoLayout.ts
- images/FunctionIcons/CategoryIcons.tsx
- src/core/services/dataMapperFileService/dataMapperFileService.ts
- components/functionsPanel/FunctionPanel.tsx
- core/state/AppSlice.ts

## God Nodes (most connected - your core abstractions)
1. `FunctionData` - 60 edges
2. `isSchemaNodeExtended()` - 43 edges
3. `MapDefinitionDeserializer` - 38 edges
4. `ConnectionDictionary` - 38 edges
5. `applyConnectionValue()` - 36 edges
6. `isNodeConnection()` - 32 edges
7. `RootState` - 31 edges
8. `RootState` - 31 edges
9. `isCustomValueConnection()` - 30 edges
10. `convertSchemaToSchemaExtended()` - 30 edges

## Surprising Connections (you probably didn't know these)
- `InitialDataMapAction` --references--> `ConnectionDictionary`  [EXTRACTED]
  core/state/DataMapSlice.ts → src/models/Connection.ts
- `ExtendedRenderOptions` --references--> `RootState`  [EXTRACTED]
  src/__test__/redux-test-helper-dm.tsx → core/state/Store.ts
- `SetConnectionInputAction` --references--> `InputConnection`  [EXTRACTED]
  core/state/DataMapSlice.ts → src/models/Connection.ts
- `FunctionListItemProps` --references--> `FunctionData`  [EXTRACTED]
  components/functionList/FunctionListItem.tsx → src/models/Function.ts
- `InputDropdownProps` --references--> `FunctionData`  [EXTRACTED]
  components/functionConfigurationMenu/inputDropdown/InputDropdown.tsx → src/models/Function.ts

## Import Cycles
- None detected.

## Communities (76 total, 9 thin omitted)

### Community 0 - "MapDefinitionDeserializer"
Cohesion: 0.13
Nodes (11): DataMapDataProvider(), DataProviderInner(), MapDefinitionDeserializer, createSchemaNodeOrFunction(), getSourceNode(), separateFunctions(), DeserializationError, addSourceReactFlowPrefix() (+3 more)

### Community 1 - "MapDefinitionSerializer.ts"
Cohesion: 0.13
Nodes (28): addConditionalToNewPathItems(), applyValueAtPath(), convertToArray(), convertToMapDefinition(), createNewPathItems(), createSourcePath(), createYamlFromMap(), findKeyInMap() (+20 more)

### Community 2 - "images/FunctionIcons/FunctionIcons.tsx"
Cohesion: 0.05
Nodes (20): AbsoluteValue32Regular, AngleIcon, CeilingValue32Regular, Count32Regular, Divide32Regular, EPowerX32Regular, FloorValue32Regular, GreaterThan32Regular (+12 more)

### Community 3 - "images/FunctionIcons/DataType16Icons.tsx"
Cohesion: 0.08
Nodes (12): Any16Filled, Any16Regular, Array16Filled, Array16Regular, Binary16Filled, Binary16Regular, Decimal16Filled, Decimal16Regular (+4 more)

### Community 4 - "images/FunctionIcons/DataType24Icons.tsx"
Cohesion: 0.08
Nodes (12): Any24Filled, Any24Regular, Array24Filled, Array24Regular, Binary24Filled, Binary24Regular, Decimal24Filled, Decimal24Regular (+4 more)

### Community 5 - "components/functionConfigurationMenu/inputTab/inputTab.tsx"
Cohesion: 0.18
Nodes (14): InputDropdown(), InputOptionProps, useStyles, InputCustomInfoLabel(), CommonProps, CustomListItem(), CustomListItemProps, InputListProps (+6 more)

### Community 6 - "core/state/PanelSlice.ts"
Cohesion: 0.09
Nodes (21): DataMapperApiService, DataMapperApiServiceOptions, DmErrorResponse, dataMapperApiVersions, defaultDataMapperApiServiceOptions, GenerateXsltResponse, IDataMapperApiService, InitDataMapperApiService() (+13 more)

### Community 7 - "src/core/state/Store.ts"
Cohesion: 0.17
Nodes (8): AppStore, includedActionsForUndo, store, initialSchemaState, schemaSlice, SchemaState, AppStore, ExtendedRenderOptions

### Community 8 - "Schema.Utils.ts"
Cohesion: 0.13
Nodes (12): convertSchemaNodeToSchemaNodeExtended(), convertSchemaToSchemaExtended(), deepestNode(), getFileNameAndPath(), maxProperties(), nodeCount(), NodeScrollDirectionType, parsePropertiesIntoNodeProperties() (+4 more)

### Community 9 - "core/state/DataMapSlice.ts"
Cohesion: 0.11
Nodes (17): ComponentState, ConnectionAction, dataMapSlice, DataMapState, DeleteConnectionAction, deleteParentRepeatingConnections(), Draft2, emptyPristineState (+9 more)

### Community 10 - "DataMap.Utils.ts"
Cohesion: 0.08
Nodes (36): mapDefinitionVersion, mapNodeParams, reservedMapDefinitionKeys, reservedMapDefinitionKeysArray, reservedMapNodeParamsArray, ConditionalMetadata, getLoopTargetNode(), getLoopTargetNodeWithJson() (+28 more)

### Community 11 - "TrieTree"
Cohesion: 0.15
Nodes (3): TrieTree, TrieTreeNode, AppState

### Community 12 - "components/common/fileDropdownTree/FileDropdownTree.tsx"
Cohesion: 0.48
Nodes (4): useStyles, FileDropdownTree(), FileDropdownTreeProps, MockFileService

### Community 13 - "MapChecker.Utils.ts"
Cohesion: 0.13
Nodes (17): MapCheckerItemProps, MapCheckerItemProps, MapCheckerPanel(), useStyles, nodeHasSourceNodeEventually(), invalidFunctions(), isFunctionData(), IntlMessage (+9 more)

### Community 14 - "core/state/Store.ts"
Cohesion: 0.22
Nodes (16): HandleResponseProps, useSchema(), useSchemaProps, AppDispatch, includedActionsForUndo, SchemaTree(), SchemaTreeProps, SchemaTreeNode() (+8 more)

### Community 15 - "src/components/schema/SchemaPanel.tsx"
Cohesion: 0.11
Nodes (14): ReactFlowStatesProps, schemaFileQuerySettings, usePanelBodyStyles, usePanelStyles, useStyles, AppDispatch, autoLayout(), Direction (+6 more)

### Community 16 - "components/test/TestPanel.tsx"
Cohesion: 0.20
Nodes (12): Panel(), PanelProps, PanelXButton(), PanelXButtonProps, useStyles, useStyles, TestPanel(), TestPanelProps (+4 more)

### Community 17 - "Edge.Utils.ts"
Cohesion: 0.17
Nodes (17): BoundingBox, convertCanvasToGridPoint(), convertGridToCanvasPoint(), findPath(), generateBoundingBoxes(), generatePathfindingGrid(), getLinearDistance(), getLineStretchLength() (+9 more)

### Community 18 - "Function.Utils.ts"
Cohesion: 0.10
Nodes (21): InputTextbox(), InputTextboxProps, collectionBranding, conversionBranding, customBranding, dateTimeBranding, FunctionGroupBranding, logicalBranding (+13 more)

### Community 19 - "components/schema/SchemaPanel.tsx"
Cohesion: 0.17
Nodes (17): ConfigPanelProps, DataMapperFileService(), FileWithVsCodePath, SchemaFile, SchemaPanelNodeReactFlowDataProps, ConfigPanelProps, schemaFileQuerySettings, SchemaPanel() (+9 more)

### Community 20 - "isFunctionNode"
Cohesion: 0.22
Nodes (14): getCoordinatesForHandle(), MapCheckerItem(), useMapCheckerItemStyles, NodeIds, SchemaTreeDataProps, getCoordinatesForHandle(), MapCheckerItem(), useMapCheckerItemStyles (+6 more)

### Community 21 - "components/canvas/ReactFlow.tsx"
Cohesion: 0.15
Nodes (19): EdgePopOver(), EdgePopOverProps, DMReactFlowProps, edgeTypes, nodeTypes, ReactFlowWrapper(), reactFlowStyle, useStyles (+11 more)

### Community 22 - "src/core/state/__test__/DataMapSlice.spec.ts"
Cohesion: 0.13
Nodes (3): connectionDict, functionData, functionDict

### Community 23 - "Icon.Utils.tsx"
Cohesion: 0.08
Nodes (25): String24Regular, AbsoluteValue32Regular, AngleIcon, CeilingValue32Regular, Count32Regular, Divide32Regular, EPowerX32Regular, FloorValue32Regular (+17 more)

### Community 24 - "ThemeConect.ts"
Cohesion: 0.18
Nodes (9): ConnectionLineComponent(), FunctionCategoryColorToken, customDarkTokens, customTokens, DataMapperTheme, extendedWebDarkTheme, extendedWebLightTheme, fnColors (+1 more)

### Community 25 - "src/components/functionConfigurationMenu/inputDropdown/InputDropdown.tsx"
Cohesion: 0.19
Nodes (10): InputDropdown(), InputOptionProps, useStyles, UnboundedInput, isValidConnectionByType(), isValidCustomValueByType(), checkIfValueNeedsQuotes(), quoteSelectedCustomValue() (+2 more)

### Community 26 - "components/common/reactflow/FunctionNode.tsx"
Cohesion: 0.31
Nodes (8): CanvasNode(), CanvasNodeProps, CardProps, FunctionCardProps, FunctionNode(), useStyles, useHoverFunctionNode(), useSelectedNode()

### Community 27 - "ReactFlow.Util.ts"
Cohesion: 0.12
Nodes (17): functionPrefix, ReactFlowEdgeType, ReactFlowNodeType, sourcePrefix, targetPrefix, generateInputHandleId(), ContainerLayoutNode, createReactFlowEdgeLabels() (+9 more)

### Community 28 - "components/canvas/useReactflowStates.ts"
Cohesion: 0.52
Nodes (6): ReactFlowStatesProps, useReactFlowStates(), useReactFlowStates(), createEdgeId(), getFunctionNode(), convertWholeDataMapToLayoutTree()

### Community 29 - "src/core/state/selectors/selectors.ts"
Cohesion: 0.43
Nodes (5): ConnectedEdge(), useEdgePath(), useHoverEdge(), useSelectedEdge(), useSelectedIntermediateEdge()

### Community 30 - "models/index.ts"
Cohesion: 0.23
Nodes (12): validateAndCreateConnectionInput(), validateAndCreateConnectionOutput(), DetailsTabContents(), FunctionConfigurationPopover(), FunctionConfigurationPopoverProps, TabTypes, useStyles, validateAndCreateConnectionInput() (+4 more)

### Community 31 - "RootState"
Cohesion: 0.42
Nodes (6): CodeViewPanel(), CodeViewPanelProps, CodeViewPanelBody(), CodeViewPanelBodyProps, useStyles, RootState

### Community 32 - "src/components/functionsPanel/FunctionPanel.tsx"
Cohesion: 0.39
Nodes (4): FunctionPanel(), PanelProps, useStyles, FunctionsSVG()

### Community 33 - "src/core/state/DataMapSlice.ts"
Cohesion: 0.10
Nodes (24): ComponentState, dataMapSlice, DataMapState, DeleteConnectionAction, deleteNodeFromConnections(), doDataMapOperation(), Draft2, emptyPristineState (+16 more)

### Community 34 - "src/components/functionConfigurationMenu/inputTab/inputTab.tsx"
Cohesion: 0.14
Nodes (15): InputCustomInfoLabel(), CommonProps, CustomListItem(), CustomListItemProps, InputList(), InputListProps, InputListWrapper, TemplateItemProps (+7 more)

### Community 35 - "DataMapperDesignerProvider.tsx"
Cohesion: 0.17
Nodes (7): reactPlugin, DataMapperDesignerContext, DataMapperDesignerProvider(), DataMapperDesignerProviderProps, reactPlugin, getCustomizedTheme(), store

### Community 37 - "src/mapHandling/__test__/MapDefinitionSerializer.spec.ts"
Cohesion: 0.07
Nodes (9): getConnectionForAnyKey(), hasExpectedConnection(), isEqualToCustomValue(), directAccessPseudoFunction, directAccessPseudoFunctionKey, ifPseudoFunctionKey, indexPseudoFunctionKey, fixMapDefinitionCustomValues() (+1 more)

### Community 40 - "DataMapDataProvider.tsx"
Cohesion: 0.12
Nodes (4): DataMapDataProviderProps, appSlice, AppState, initialState

### Community 45 - "isSchemaNodeExtended"
Cohesion: 0.25
Nodes (16): getInputTypeFromNode(), deleteConnectionFromConnections(), deleteParentRepeatingConnections(), getInputTypeFromNode(), addLoopingForToNewPathItems(), collectSourceNodeIdsForConnectionChain(), connectionDoesExist(), createNewEmptyConnection() (+8 more)

### Community 46 - "src/components/canvas/ReactFlow.tsx"
Cohesion: 0.14
Nodes (11): EdgePopOver(), EdgePopOverProps, DMReactFlowProps, edgeTypes, nodeTypes, ReactFlowWrapper(), reactFlowStyle, useStyles (+3 more)

### Community 47 - "src/images/FunctionIcons/DataType16Icons.tsx"
Cohesion: 0.08
Nodes (12): Any16Filled, Any16Regular, Array16Filled, Array16Regular, Binary16Filled, Binary16Regular, Decimal16Filled, Decimal16Regular (+4 more)

### Community 48 - "src/images/FunctionIcons/DataType24Icons.tsx"
Cohesion: 0.08
Nodes (11): Any24Filled, Any24Regular, Array24Filled, Array24Regular, Binary24Filled, Binary24Regular, Decimal24Filled, Decimal24Regular (+3 more)

### Community 49 - "Connection.Utils.ts"
Cohesion: 0.08
Nodes (37): addConnection(), DataMapOperationState, FailedMapDefinition, createSchemaToSchemaNodeConnection(), Connection, ConnectionDictionary, CustomValueConnection, EmptyConnection (+29 more)

### Community 50 - "src/components/schema/SchemaPanelBody.tsx"
Cohesion: 0.29
Nodes (6): FileSelectorOption, SchemaFileSelector(), U, useStyles, SchemaPanelBodyProps, DataMapperFileService()

### Community 51 - "src/components/schema/tree/SchemaTreeNode.tsx"
Cohesion: 0.16
Nodes (15): SchemaPanelBody(), SchemaTree(), SchemaTreeProps, SchemaTreeNode(), SchemaTreeNodeProps, TypeAnnotation(), SchemaTreeNodeHandle(), SchemaTreeNodeHandleProps (+7 more)

### Community 52 - "TrieTree"
Cohesion: 0.22
Nodes (4): TrieTree, TrieTreeNode, AppState, useSearch()

### Community 53 - "FunctionData"
Cohesion: 0.08
Nodes (36): InputDropdownProps, FunctionIconProps, functionCategoryItemKeyPrefix, FunctionDataTreeItem, FunctionList(), FunctionListProps, fuseFunctionSearchOptions, loopFuseFunctionSearchOptions (+28 more)

### Community 54 - "ref_fluentui_react_components"
Cohesion: 0.18
Nodes (12): CodeViewPanel(), CodeViewPanelProps, CodeViewPanelBody(), useStyles, Panel(), PanelProps, PanelXButton(), PanelXButtonProps (+4 more)

### Community 55 - "components/common/selector/__test__/FileSelector.spec.tsx"
Cohesion: 0.20
Nodes (8): IDataMapperFileService, InitDataMapperFileService(), SchemaFile, InputListWrapper, FileSelectorProps, MockFileService, renderWithRedux(), DataMapperDesignerProps

### Community 56 - "src/components/functionConfigurationMenu/functionConfigurationPopover.tsx"
Cohesion: 0.42
Nodes (7): DetailsTabContents(), FunctionConfigurationPopover(), FunctionConfigurationPopoverProps, TabTypes, OutputTabContents(), useStyles, isFileDropdownFunction()

### Community 57 - "ext_logic_apps_shared_src_index_ts"
Cohesion: 0.05
Nodes (30): generateDataMapXslt(), testDataMap(), getFunctions(), getSelectedSchema(), DataMapperApiService, DataMapperApiServiceOptions, DmErrorResponse, DataMapperApiServiceInstance() (+22 more)

### Community 58 - "src/core/state/ModalSlice.ts"
Cohesion: 0.33
Nodes (4): initialState, modalSlice, ModalState, WarningModalState

### Community 59 - "DataMapperDesigner.tsx"
Cohesion: 0.17
Nodes (7): DataMapperWrappedContext, ScrollLocation, ScrollProps, DataMapperDesigner(), DialogView(), useStaticStyles, useStyles

### Community 60 - "core/index.ts"
Cohesion: 0.30
Nodes (5): DataMapperApiServiceInstance(), generateDataMapXslt(), testDataMap(), getFunctions(), getSelectedSchema()

### Community 61 - "src/components/commandBar/EditorCommandBar.tsx"
Cohesion: 0.22
Nodes (3): EditorCommandBar(), EditorCommandBarProps, useStyles

### Community 62 - "components/commandBar/EditorCommandBar.tsx"
Cohesion: 0.24
Nodes (8): EditorCommandBar(), EditorCommandBarProps, useStyles, MetaMapDefinition, initialState, modalSlice, ModalState, WarningModalState

### Community 63 - "ref_react"
Cohesion: 0.12
Nodes (6): CodeViewPanelBodyProps, useStyles, TestPanel(), TestPanelProps, TestPanelBody(), TestPanelBodyProps

### Community 64 - "src/components/common/reactflow/FunctionNode.tsx"
Cohesion: 0.20
Nodes (11): CanvasNode(), CanvasNodeProps, CardProps, FunctionCardProps, FunctionNode(), useStyles, FunctionIcon(), useHoverFunctionNode() (+3 more)

### Community 65 - "src/components/common/selector/__test__/FileSelector.spec.tsx"
Cohesion: 0.18
Nodes (6): FileDropdownTree(), FileDropdownTreeProps, MockFileService, FileSelectorProps, MockFileService, useStyles

### Community 66 - "src/core/state/FunctionSlice.ts"
Cohesion: 0.22
Nodes (6): functionSlice, FunctionState, initialFunctionState, initialSchemaState, schemaSlice, SchemaState

### Community 67 - "MapMetadataSerializer.ts"
Cohesion: 0.40
Nodes (5): convertConnectionShorthandToId(), generateFunctionConnectionMetadata(), generateMapMetadata(), assignFunctionNodePositionsFromMetadata(), assignFunctionNodePositionsFromMetadata()

### Community 68 - "ref_xyflow_react"
Cohesion: 0.24
Nodes (6): SchemaPanelNode(), SchemaPanelNodeReactFlowDataProps, SchemaPanel(), NodeInfo(), NodeInfoProps, NodeInspector()

### Community 69 - "src/core/state/ErrorsSlice.ts"
Cohesion: 0.28
Nodes (7): errorsSlice, ErrorsState, initialFunctionState, errorsSlice, ErrorsState, initialFunctionState, MapIssue

### Community 70 - "getConnectedTargetSchemaNodes"
Cohesion: 0.33
Nodes (7): handleDirectAccessConnection(), handleDirectAccessConnection(), collectSourceNodesForConnectionChain(), collectTargetNodesForConnectionChain(), getConnectedSourceSchemaNodes(), getConnectedTargetSchemaNodes(), getFunctionConnectionUnits()

### Community 71 - "ui/hooks/useAutoLayout.ts"
Cohesion: 0.29
Nodes (5): autoLayout(), Direction, elk, LayoutAlgorithm, LayoutOptions

### Community 74 - "components/functionsPanel/FunctionPanel.tsx"
Cohesion: 0.60
Nodes (3): FunctionPanel(), PanelProps, useStyles

### Community 75 - "core/state/AppSlice.ts"
Cohesion: 0.50
Nodes (3): appSlice, AppState, initialState

## Knowledge Gaps
- **197 isolated node(s):** `cache`, `intl`, `EdgePopOverProps`, `DMReactFlowProps`, `nodeTypes` (+192 more)
  These have ≤1 connection - possible missing edges. (Counts symbols only; 439 node(s) total have ≤1 connection when file, concept and rationale nodes are included.)
- **9 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `FunctionData` connect `FunctionData` to `MapDefinitionDeserializer`, `components/functionConfigurationMenu/inputTab/inputTab.tsx`, `Schema.Utils.ts`, `core/state/DataMapSlice.ts`, `DataMap.Utils.ts`, `MapChecker.Utils.ts`, `Function.Utils.ts`, `src/core/state/__test__/DataMapSlice.spec.ts`, `src/components/functionConfigurationMenu/inputDropdown/InputDropdown.tsx`, `components/common/reactflow/FunctionNode.tsx`, `ReactFlow.Util.ts`, `models/index.ts`, `src/core/state/DataMapSlice.ts`, `src/components/functionConfigurationMenu/inputTab/inputTab.tsx`, `src/mapHandling/__test__/MapDefinitionSerializer.spec.ts`, `DataMapDataProvider.tsx`, `isSchemaNodeExtended`, `Connection.Utils.ts`, `src/components/functionConfigurationMenu/functionConfigurationPopover.tsx`, `ext_logic_apps_shared_src_index_ts`, `core/index.ts`, `src/components/common/reactflow/FunctionNode.tsx`, `src/core/state/FunctionSlice.ts`?**
  _High betweenness centrality (0.032) - this node is a cross-community bridge._
- **What connects `cache`, `intl`, `EdgePopOverProps` to the rest of the system?**
  _197 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Should `MapDefinitionDeserializer` be split into smaller, more focused modules?**
  _Cohesion score 0.1282051282051282 - nodes in this community are weakly interconnected._
- **Should `MapDefinitionSerializer.ts` be split into smaller, more focused modules?**
  _Cohesion score 0.13118279569892474 - nodes in this community are weakly interconnected._
- **Should `images/FunctionIcons/FunctionIcons.tsx` be split into smaller, more focused modules?**
  _Cohesion score 0.04878048780487805 - nodes in this community are weakly interconnected._
- **Should `images/FunctionIcons/DataType16Icons.tsx` be split into smaller, more focused modules?**
  _Cohesion score 0.08 - nodes in this community are weakly interconnected._
- **Should `images/FunctionIcons/DataType24Icons.tsx` be split into smaller, more focused modules?**
  _Cohesion score 0.08 - nodes in this community are weakly interconnected._