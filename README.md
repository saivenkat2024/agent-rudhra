# 🧠 Rudhra AI: The Unified Intelligence OS

**Rudhra** is a state-of-the-art AI ecosystem designed to be a professional Research & Operations Assistant. It combines a powerful FastAPI backend, a cinematic Streamlit interface, and a modern Next.js frontend to provide a comprehensive suite of AI-driven capabilities—from advanced RAG (Retrieval-Augmented Generation) to real-time web search and autonomous operation management.

---

## 🚀 Key Features

### 1. 📚 Advanced RAG Mode (Chat with PDF)
- **High-Precision Indexing**: Uses FAISS for lightning-fast vector search.
- **Configurable Retrieval**: Optimized with a chunk size of 1000 and top-k retrieval of 5.
- **Dynamic Connection**: Effortlessly connect to different materials from your knowledge library.

### 2. 🧠 Unified Agent Brain
- **Tool-Augmented Intelligence**: Integrated with GitHub, Filesystem, and Local Calendar via MCP (Model Context Protocol).
- **Real-Time Web Search**: Uses Tavily for hyper-accurate, hallucination-free search results with 2026 data enforcement.
- **Visual Intelligence**: Generate high-fidelity images using FLUX and analyze uploaded images with vision models.

### 3. 📝 Exam & Learning Mode
- **Question Extraction**: Automatically extract questions and MCQs from uploaded documents.
- **Smart Evaluation**: AI-driven answer grading and feedback.
- **Mind Map Generator**: Visualize complex concepts with auto-generated interactive mind maps.

### 4. 🔒 Secure & Personalized
- **Cinematic Auth**: A premium, "hacker-style" login experience with system initialization sequences.
- **Deep Personalization**: Persistent user context storage to tailor responses to your specific background and preferences.

---

## 🛠️ Tech Stack

### **Backend**
- **Core**: Python, FastAPI
- **AI Orchestration**: LangChain, LangGraph
- **Vector Database**: FAISS
- **Models**: OpenAI (GPT-4o-mini), Gemini (Transcription), NVIDIA (Vision/LLM)
- **Database**: PostgreSQL (via Psycopg), JSON-based persistent states

### **Frontend**
- **Streamlit**: A high-performance, feature-rich "Operations Center."
- **Next.js**: A modern, responsive web UI located in `/rudhra-ui`.
- **Styling**: Vanilla CSS with cinematic animations and rich aesthetics.

---

## 📦 Installation & Setup

### Prerequisites
- Python 3.10+
- Node.js & npm (for the web UI)
- API Keys: OpenAI/OpenRouter, Gemini, NVIDIA, Tavily

### 1. Backend Setup
```bash
# Create and activate virtual environment
python -m venv myenv
source myenv/bin/activate  # On Windows use `myenv\Scripts\activate`

# Install dependencies
pip install -r requirements.txt

# Configure environment variables
# Create a .env file based on the project requirements
```

### 2. Frontend Setup (Next.js)
```bash
cd rudhra-ui
npm install
npm run dev
```

### 3. Running the API Server
```bash
uvicorn api_server:app --reload --port 8001
```

### 4. Running the Streamlit Interface
```bash
streamlit run frontend.py
```

---

## 📂 Project Structure

- `api_server.py`: The heart of the system, exposing REST & Streaming endpoints.
- `backend.py`: The LangGraph-based agent logic and tool definitions.
- `frontend.py`: The Streamlit-based user interface.
- `ingest_service.py`: PDF processing and FAISS indexing pipeline.
- `rag.py`: RAG logic and LLM configurations.
- `rudhra-ui/`: The modern Next.js frontend application.
- `exam_mode.py` & `score.py`: Learning and evaluation modules.
- `mcp_tools.py`: Connectors for local and remote tool execution.

---

## 🛡️ License
Proprietary and Confidential. Designed by saivenkat2024 for Rudhra Intelligence Labs.
