# Graph Report - src  (2026-10-07)

## Corpus Check
- 141 files · ~80,919 words
- Verdict: corpus is large enough that graph structure adds value.

## Summary
- 820 nodes · 2320 edges · 48 communities (23 shown, 25 thin omitted)
- Extraction: 99% EXTRACTED · 1% INFERRED · 0% AMBIGUOUS · INFERRED: 15 edges (avg confidence: 0.85)
- Token cost: 0 input · 0 output

## Graph Freshness
- Built from commit: `04df5b5c`
- Run `git rev-parse HEAD` and compare to check if the graph is stale.
- Run `graphify update .` after code changes (no API cost).

## Community Hubs (Navigation)
- history-types.ts
- schemas.ts
- src/react/store/chatStore.ts
- a2a-client.stream.test.ts
- plugins/index.ts
- SessionManager
- react/store/chatStore.ts
- ChatInterface
- SSEClient
- A2A Chat React Components
- DataTransferPolyfill
- a2a-client.accumulation.test.ts
- react/components/FileUpload/FileUpload.tsx
- src/react/components/Message/Message.tsx
- agent-discovery.ts
- AuthRequiredPart
- src/react/components/MessageInput/MessageInput.tsx
- react/index.ts
- src/react/types/index.ts
- src/react/components/ChatWindow/ChatWindow.tsx
- DataTransferPolyfill
- a2a-client.ts
- MockSSEClient
- MockSSEClient
- src/react/components/FileUpload/FileUpload.tsx
- use-a2a.ts
- src/react/hooks/useTheme.ts
- react/components/ChatWindow/ChatWindow.tsx
- src/react/components/MessageList/MessageList.tsx
- ref_vitest
- AgentCard
- ref_react

## God Nodes (most connected - your core abstractions)
1. `AgentCard` - 45 edges
2. `A2AClient` - 33 edges
3. `SessionManager` - 29 edges
4. `useChatStore` - 28 edges
5. `ChatSession` - 26 edges
6. `HttpClient` - 26 edges
7. `AuthConfig` - 26 edges
8. `ChatInterface` - 23 edges
9. `SSEClient` - 21 edges
10. `Message` - 20 edges

## Surprising Connections (you probably didn't know these)
- `ChatState` --references--> `ChatSession`  [EXTRACTED]
  react/store/chatStore.ts → src/api/history-types.ts
- `ChatState` --references--> `Message`  [EXTRACTED]
  react/store/chatStore.ts → src/api/history-types.ts
- `ChatState` --references--> `A2AClient`  [EXTRACTED]
  react/store/chatStore.ts → src/client/a2a-client.ts
- `AgentConfig` --references--> `AuthConfig`  [EXTRACTED]
  react/types/index.ts → src/client/types.ts
- `AuthPartState` --inherits--> `AuthRequiredPart`  [EXTRACTED]
  react/components/Message/AuthenticationMessage.tsx → src/client/types.ts

## Import Cycles
- None detected.

## Communities (48 total, 25 thin omitted)

### Community 0 - "history-types.ts"
Cohesion: 0.06
Nodes (46): createHistoryApi(), HistoryApi, HistoryApiClient, HistoryApiConfig, JsonRpcRequest, extractAuthEventFromMessage(), extractLastMessage(), isAuthRequiredMessage() (+38 more)

### Community 1 - "schemas.ts"
Cohesion: 0.06
Nodes (53): formatErrorMessage(), getUserFriendlyErrorMessage(), A2AError, AuthenticationError, createJsonRpcError(), extractErrorDetails(), isJsonRpcErrorResponse(), JsonRpcErrorCode (+45 more)

### Community 2 - "src/react/store/chatStore.ts"
Cohesion: 0.09
Nodes (28): A2AClientConfig, WaitForCompletionOptions, HttpClient, AuthConfig, AuthRequiredEvent, AuthRequiredHandler, HttpClientOptions, IdentityProvider (+20 more)

### Community 4 - "plugins/index.ts"
Cohesion: 0.08
Nodes (18): AnalyticsConfig, AnalyticsEvent, AnalyticsPlugin, LoggerConfig, LoggerPlugin, LogLevel, AnalyticsConfig, AnalyticsEvent (+10 more)

### Community 5 - "SessionManager"
Cohesion: 0.10
Nodes (10): LocalStoragePlugin, SessionManager, mockLocalStorage, mockSessionStorage, SessionChangeEvent, SessionData, SessionEventMap, SessionOptions (+2 more)

### Community 6 - "react/store/chatStore.ts"
Cohesion: 0.06
Nodes (39): CodeBlockHeader(), CodeBlockHeaderProps, useStyles, escapeAttr(), formatTime(), link(), Message, MessageComponent() (+31 more)

### Community 7 - "ChatInterface"
Cohesion: 0.16
Nodes (10): ChatInterface, ChatInterfaceConfig, ChatEventMap, ChatMessage, ChatOptions, ChatRole, ConversationExport, StreamUpdate (+2 more)

### Community 8 - "SSEClient"
Cohesion: 0.18
Nodes (7): SSEClient, MockEventSource, ErrorHandler, MessageHandler, SSEClientOptions, SSEMessage, SSEParser

### Community 9 - "A2A Chat React Components"
Cohesion: 0.17
Nodes (11): A2A Chat React Components, Components, Features, Hooks, Important: CSS Import Required, Main Component, State Management, TypeScript Support (+3 more)

### Community 21 - "src/react/components/Message/Message.tsx"
Cohesion: 0.14
Nodes (16): AuthenticationMessage(), AuthenticationMessageProps, useStyles, CodeBlockHeader(), CodeBlockHeaderProps, useStyles, escapeAttr(), formatFileSize() (+8 more)

### Community 22 - "agent-discovery.ts"
Cohesion: 0.16
Nodes (6): AgentDiscoveryOptions, CacheEntry, AgentRegistry, AgentSummary, EnterpriseAgentRegistry, PublicAgentRegistry

### Community 23 - "AuthRequiredPart"
Cohesion: 0.15
Nodes (15): AuthRequiredPart, ExampleWithHooks(), manualAuthFlow(), AuthenticationMessage(), AuthenticationMessageProps, AuthPartState, useStyles, AuthPartState (+7 more)

### Community 24 - "src/react/components/MessageInput/MessageInput.tsx"
Cohesion: 0.19
Nodes (14): MessageInput(), MessageInputProps, useStyles, StatusMessage(), StatusMessageProps, useStyles, Attachment, ArtifactData (+6 more)

### Community 25 - "react/index.ts"
Cohesion: 0.15
Nodes (19): AuthenticatedUsernameExample(), CustomUsernameExample(), DynamicUsernameExample(), ChatWithCustomAuthHandler(), ChatWithDefaultAuth(), ChatWidget(), useStyles, ChatThemeProvider() (+11 more)

### Community 26 - "src/react/types/index.ts"
Cohesion: 0.18
Nodes (10): Message, mockFormat, AgentConfig, Branding, ChatConfig, FileAttachment, Message, AgentConfig (+2 more)

### Community 27 - "src/react/components/ChatWindow/ChatWindow.tsx"
Cohesion: 0.30
Nodes (9): AuthStateExample(), CustomChatImplementation(), ManualAuthUIExample(), useChatWidget(), ChatWindow(), ChatWindowProps, useStyles, mockUseChatWidget (+1 more)

### Community 29 - "a2a-client.ts"
Cohesion: 0.23
Nodes (4): A2AClient, mockAgentCard, AgentCapabilities, Task

### Community 32 - "src/react/components/FileUpload/FileUpload.tsx"
Cohesion: 0.53
Nodes (3): FileUpload(), FileUploadProps, formatFileSize()

### Community 33 - "use-a2a.ts"
Cohesion: 0.22
Nodes (8): FileAttachment, mockStreamReturnValue, useA2A(), UseA2AReturn, createHistoryStorage(), getAgentContextStorageKey(), getAgentMessagesStorageKey(), getAgentStorageIdentifier()

### Community 34 - "src/react/hooks/useTheme.ts"
Cohesion: 0.26
Nodes (7): CompanyLogo(), CompanyLogoProps, applyTheme(), DEFAULT_THEME, mergeTheme(), useTheme(), ChatTheme

### Community 36 - "react/components/ChatWindow/ChatWindow.tsx"
Cohesion: 0.10
Nodes (21): ChatWidget(), useStyles, ChatWindow(), ChatWindowProps, useStyles, CompanyLogo(), CompanyLogoProps, DEFAULT_THEME (+13 more)

### Community 44 - "src/react/components/MessageList/MessageList.tsx"
Cohesion: 0.29
Nodes (5): MessageList(), MessageListProps, useStyles, TypingIndicator(), TypingIndicatorProps

### Community 47 - "ref_react"
Cohesion: 0.43
Nodes (3): SessionList(), SessionListProps, useStyles

## Knowledge Gaps
- **60 isolated node(s):** `JsonRpcRequest`, `mockAgentCard`, `mockAgentCard`, `mockAgentCard`, `mockUseChatWidget` (+55 more)
  These have ≤1 connection - possible missing edges or undocumented components. (Counts symbols only; 174 node(s) total have ≤1 connection when file, concept and rationale nodes are included.)
- **25 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `AgentCard` connect `AgentCard` to `use-a2a.ts`, `src/react/store/chatStore.ts`, `a2a-client.stream.test.ts`, `schemas.ts`, `react/store/chatStore.ts`, `a2a-client.accumulation.test.ts`, `ref_vitest`, `agent-discovery.ts`, `react/index.ts`, `src/react/types/index.ts`, `a2a-client.ts`?**
  _High betweenness centrality (0.093) - this node is a cross-community bridge._
- **Are the 7 inferred relationships involving `useChatStore` (e.g. with `.addMessage()` and `.clear()`) actually correct?**
  _`useChatStore` has 7 INFERRED edges - model-reasoned connections that need verification._
- **What connects `JsonRpcRequest`, `mockAgentCard`, `mockAgentCard` to the rest of the system?**
  _60 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Should `history-types.ts` be split into smaller, more focused modules?**
  _Cohesion score 0.0616729088639201 - nodes in this community are weakly interconnected._
- **Why does `Message` connect `react/store/chatStore.ts` to `src/react/store/chatStore.ts`, `plugins/index.ts`, `ChatInterface`, `AuthRequiredPart`, `react/index.ts`, `a2a-client.ts`?**
  _High betweenness centrality (0.076) - this node is a cross-community bridge._
- **Should `schemas.ts` be split into smaller, more focused modules?**
  _Cohesion score 0.05960705960705961 - nodes in this community are weakly interconnected._
- **Why does `A2AClient` connect `a2a-client.ts` to `history-types.ts`, `use-a2a.ts`, `src/react/store/chatStore.ts`, `a2a-client.stream.test.ts`, `plugins/index.ts`, `react/store/chatStore.ts`, `ChatInterface`, `a2a-client.accumulation.test.ts`, `ref_vitest`, `AgentCard`, `AuthRequiredPart`?**
  _High betweenness centrality (0.062) - this node is a cross-community bridge._