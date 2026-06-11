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

Answer: 
The BQBYTE TECHNOLOGIES Supplier Governance & Compliance Policy, effective September 1, 2024, is an internal procurement document that outlines the framework for managing and monitoring suppliers. It covers:

Purpose & Scope: Defining the policy's objectives and applicability.
Supplier Classification: A framework for categorizing suppliers into tiers.
Service Level Agreements (SLAs): Specific performance expectations based on supplier tier.
Penalty & Incentive Structure: Mechanisms for rewarding good performance and penalizing non-compliance (e.g., for defect rates, lead times, and on-time delivery).
Risk Management: Protocols for assessing and escalating risks, including concentration risk limits for procurement spend (e.g., no single region over 45%, no single country over 25%).
Sustainability & Compliance: Requirements related to sustainability scores and overall compliance.
Auditing & Scoring: Methodology for audits and calculating compliance scores.
Disruption Management: Procedures for responding to disruptions and activating alternate suppliers.

## Improvements
- Add memory
- Add multiple document support
- Add citations
- Add dashboard analytics
