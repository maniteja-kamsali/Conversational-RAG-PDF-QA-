# **Conversational RAG PDF Chatbot** 📜💬

This project is a **Conversational Retrieval-Augmented Generation (RAG) Q&A System** that allows users to **upload PDFs and chat** with their content in real time. It uses **LangChain, Hugging Face embeddings, ChromaDB, and Groq LLM** to retrieve relevant document context and generate concise answers. Built with **Streamlit**, it maintains **chat history** for context-aware responses, providing an interactive experience.

---

## **🚀 Features**
- 📂 **Upload multiple PDFs** and extract text content.
- 🤖 **Conversational Q&A** with context-aware responses.
- 🔍 **Retrieves relevant document sections** for accurate answers.
- 🧠 **Uses LangChain, ChromaDB, Hugging Face Embeddings, and Groq LLM**.
- 💾 **Maintains chat history per session** using Streamlit's session state.
- 🌐 **Interactive Streamlit web interface**.

---

## **🛠️ Installation**

### **1️⃣ Clone the Repository**
```bash
git clone https://github.com/your-username/Conversational-RAG-PDF-QA.git
cd Conversational-RAG-PDF-QA
```

### **2️⃣ Create a Virtual Environment**
```bash
conda create --name rag_pdf_chatbot python=3.9 -y
conda activate rag_pdf_chatbot
```

### **3️⃣ Install Dependencies**
```bash
pip install -r requirements.txt
```

### **4️⃣ Set Up API Keys**
- Create a `.env` file and add your **Groq API key** and **Hugging Face API key**:
```env
GROQ_API_KEY=your_groq_api_key
HF_TOKEN=your_huggingface_api_key
```

---

## **🚀 Running the Application**
```bash
streamlit run app.py
```

This will start a local Streamlit server where you can upload PDFs and chat with their content.

---

## **📝 How It Works**
1️⃣ **User uploads PDFs** → Extracts text using `PyPDFLoader`.
2️⃣ **Text is split into chunks** → Embeddings are generated using `Hugging Face`.
3️⃣ **ChromaDB stores embeddings** → Enables fast document retrieval.
4️⃣ **User asks a question** → `contextualize_q_prompt` reformulates it.
5️⃣ **Retriever fetches relevant sections** → `qa_prompt` generates an answer.
6️⃣ **Chat history is stored** → Ensures context-aware conversations.

---

## **📂 Project Structure**
```bash
📂 Conversational-RAG-PDF-QA/
├── 📄 app.py               # Main Streamlit application
├── 📄 requirements.txt     # Dependencies
├── 📄 .env                 # API keys (not included in repo)
└── 📄 README.md            # Project documentation
```

---

## **📌 Future Improvements**
- ☁️ Store chat history in a **database** instead of session state.
- 📊 Add **visualizations** for retrieved content.
- 🔄 Support **multiple document types** (TXT, DOCX, etc.).

---

## **💡 Contributing**
Feel free to open issues or submit pull requests to improve the project!

---

## **🌟 Acknowledgments**
Thanks to **LangChain, ChromaDB, Hugging Face, and Streamlit** for their amazing tools!

---

🚀 **Happy Chatting with PDFs!**

