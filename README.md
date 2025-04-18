# 📦 GenAI Assistant for Supply Chain Optimization

This project is an AI-powered assistant that reads supply chain data, flags issues, and suggests improvements based on uploaded policy documents using LLM and RAG.

## 🧠 Use Case

Businesses handle tons of supply chain data—stock levels, lead times, defect rates, and more. But:

- ❌ It's hard to spot issues in real-time
- ❌ No easy way to get suggestions based on best practices

This AI Assistant solves that using a hybrid approach:
- 🧮 Structured data (CSV/invoice)
- 📄 Unstructured policy docs (PDFs)
- 🤖 AI model (OpenAI GPT + LangChain RAG)

---

## 🚀 Features

✅ Read supply chain data from Excel/CSV  
✅ Automatically flag delays, low stock, high defects, or demand  
✅ Use a **PDF policy guide** as context (RAG)  
✅ Get **tailored suggestions** from an LLM (OpenAI)  
✅ Output in organized table for presentation or export

---

## 📂 Dataset Reference

- **Supply Chain CSV:** A synthetic dataset created for testing AI optimization in product inventory, supplier performance, and delivery patterns.https://www.kaggle.com/code/amirmotefaker/supply-chain-analysis
- **Policy PDF Document:** ["World Bank Supply Chain Management Guidance"](https://thedocs.worldbank.org/en/doc/1c3b517f003b53a2e2e170e93124be84-0290032023/original/World-Bank-Supply-Chain-Management-Guidance.pdf)

You can replace the sample data with your own supply chain invoices or real-time CSV exports.

---

## 🧩 How It Works

1. **Data Input**: Upload a CSV/Excel table or invoice
2. **Issue Detection**: Check for problems like:
   - Long lead time (>20 days)
   - Low stock (<10 units)
   - High demand (optional)
   - High defect rate (>3%)
3. **Document Retrieval**:
   - Supply chain guide (PDF) is vectorized
   - The LLM pulls relevant paragraphs (RAG)
4. **LLM Reasoning**:
   - LLM generates human-like recommendations
5. **Organized Output**:
   - Issues + suggestions shown in a nice table or exported

---

## 📚 Roadmap

```mermaid
graph TD
A[User Uploads Supply Chain CSV] --> B[Flag Delays / High Demand / Quality Issues]
B --> C[Convert Issues into Natural Language Summaries]
C --> D[Use LangChain RAG to Search Supply Chain PDF]
D --> E[Prompt GPT-4 for Tailored Suggestions]
E --> F[Show Results in Table: Issue + Suggestion]
