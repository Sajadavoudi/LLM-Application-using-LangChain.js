# LLM Application with LangChain.js (RAG + Conversational QA)

End-to-end LLM app in **LangChain.js**: document ingestion, embeddings, vector search, retrieval-augmented **question answering**, conversational memory, and **Deno** web API with streaming.

## Pipeline
- **Data ingestion & chunking** → split documents for better retrieval.
- **Embeddings & vector store** → `OpenAIEmbeddings` + LangChain vector store; expose a **retriever**.
- **Question Answering** → compose a retrieval-augmented chain for factual answers from context.
- **Conversational QA** → add memory and prompts that condition on chat history + retrieved context.
- **Shipping** → **Deno** server with a streaming handler for low-latency responses.

## Stack
LangChain.js • TypeScript/JavaScript • OpenAIEmbeddings • Deno (API & streaming)
