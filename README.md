# scm-assistant-bot

Public chatbot URL: https://cloud.flowiseai.com/chatbot/ead1accb-f504-447c-90d6-78b380f7dce9

## Objective
Built a Supply Chain chatbot using Flowise and RAG.

## Architecture
PDF
→ Recursive Character Text Splitter
→ Google Gemini Embeddings
→ Qdrant Vector Store
→ Document Store Retriever
→ Conversational Retrieval QA Chain
→ Google Gemini

## LLM & Embeddings
- LLM: Gemini 2.5 Flash
- Embedding: gemini-embedding-001
- Vector Store: Qdrant

## Chunk Configurations Tried
Attempt 1:
- Chunk Size: 1000
- Overlap: 200

Final:
- Recursive Character Text Splitter
- Chunk Size: 1000
- Chunk Overlap: 200

## Public Chatbot URL
(Add Flowise public URL if available)

## Test Questions

Q1:
What is supplier rebate eligibility?

Answer:
Tier-1 suppliers are eligible if:
- OTD ≥ 93%
- Defect rate < 0.5%
- Sustainability ≥ 85

Q2:
What happens if defect rate exceeds threshold?

Answer:
- 4% surcharge
- USD 15000 containment fee
- RCA required

Q3:
Summarize supplier governance policy.

(Add response)

Q4:
What is OTD?

(Add response)

Q5:
What supplier compliance requirements exist?

(Add response)

## Improvements
- Add memory
- Add multiple document support
- Add citations
- Add dashboard analytics
