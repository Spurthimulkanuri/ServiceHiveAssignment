🤖 ServiceHive Assignment - Social-to-Lead Agent

📌 Project Overview

This project is a conversational AI agent built for a fictional SaaS product called AutoStream.

The chatbot can:

- Answer user queries (pricing, plans)
- Detect user intent (greeting, pricing, high-intent)
- Capture leads (name, email, platform)
- Validate email before capturing lead
- Use RAG (Retrieval Augmented Generation) for responses

---

⚙️ Features

🧠 Intent Detection

- Greeting → "Hi", "Hello"
- Pricing → "price", "plans", "cost"
- High Intent → "buy", "want", "subscribe"

📚 RAG (Retrieval System)

- Uses FAISS vector database
- Uses Sentence Transformers (MiniLM)
- Retrieves relevant information from "knowledge.md"

🧾 Lead Capture Flow

1. Ask Name
2. Ask Email (with validation)
3. Ask Platform (YouTube / Instagram)
4. Store lead

📧 Email Validation

- Uses regex to check valid email format
- Rejects invalid emails

---

💻 Tech Stack

- Python
- LangChain
- FAISS
- Sentence Transformers

---

📂 Project Structure

- ServiceHiveAssignment.ipynb
- knowledge.md

---

🚀 How to Run

1. Open the notebook in Google Colab
2. Run the install cell:
   !pip install -q langchain langchain-community faiss-cpu sentence-transformers
3. Run all cells
4. Start chatting using:
   chat("Hi")
chat("What is pricing?")
chat("I want pro plan")

---

💬 Example Interaction

User: Hi
Bot: Hi! 👋 How can I help you with AutoStream?

User: What is pricing?
Bot: Shows plans (Basic & Pro)

User: I want pro plan
Bot: Ask name → email → platform

User: Spurthi
Bot: Please enter your email

User: spurthi@gmail.com
Bot: Which platform do you use?

User: Instagram
Bot: 🎉 Lead captured successfully!

---

📊 Knowledge Base

Stored in "knowledge.md":

- Basic Plan: $29/month
- Pro Plan: $79/month
- Policies:
  - No refunds after 7 days
  - 24/7 support only for Pro

---

👩‍💻 Author

Spurthi Mulkanuri
