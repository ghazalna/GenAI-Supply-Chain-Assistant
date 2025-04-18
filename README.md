# GenAI-Supply-Chain-Assistant
This notebook presents a **Generative AI-powered assistant** for supply chain teams to improve decision-making around supplier delays, quality issues, and restocking needs.
The assistant combines:
- ✅ Document Understanding (simulated delivery records)
- ✅ Embedding Search with FAISS (Retrieval-Augmented Generation)
- ✅ LLM-Based Reasoning (Flan-T5) with business logic
- ✅ Hybrid Agent Logic (rules + language model)

Using these components, the assistant:
1. Parses product and supplier data
2. Flags risks like long lead times, low stock, or high defect rates
3. Suggests actions such as “Reorder”, “Flag for Delay”, or “Monitor”
4. Summarizes decisions in a structured table and visualization

This solution can scale to live enterprise systems and integrate with dashboards or ERP software to support real-time supply chain optimization.
