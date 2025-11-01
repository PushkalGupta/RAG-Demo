# RAG-Bot Demo

RAG-Bot is a simple yet powerful web-based application designed to demonstrate the core concepts of **Retrieval-Augmented Generation (RAG)**.

This demo shows how a Large Language Model (LLM), which has no prior knowledge of "secret" or private information, can be augmented with an external **knowledge base** to answer specific questions about that information.

---

## Project Objective

The goal of this demo is to visualize the **RAG pipeline in action**. It proves that the LLM is not answering from its internal (pre-trained) memory, but is instead using the documents we provide in real-time.

The demo allows you to:

- Add a "secret" to the knowledge base (e.g., "My personal PIN is 1234").
- Ask the bot for that secret ("What is my PIN?").
- See the workflow as the bot retrieves your document, adds it to the prompt, and generates the correct answer.

---

## Features

- **Interactive Chat Interface:** A clean UI for chatting with the RAG-powered bot.
- **Dynamic Knowledge Base:** Manually add, review, and manage the "secret" documents the bot can access.
- **Live RAG Workflow Visualization:** A dedicated tab that shows you exactly how the bot answered your question by revealing the 3-step process.
- **Guided Demo Scenarios:** An animated, step-by-step walkthrough that guides you through the process of adding and querying a secret document.

---

## How It Works: The RAG-Bot Flow

This demo visually exposes the **3-step RAG pipeline**:

1. **Retrieve:**  
   When you ask a question, the app first searches the Knowledge Base for the most relevant document chunk based on your query's keywords. The LLM is not queried yet.

2. **Augment:**  
   The retrieved document (the "context") is fused with your original query into a detailed prompt. The LLM is explicitly instructed to only use this context to answer.

3. **Generate:**  
   The augmented prompt is sent to the Gemini API. The LLM generates an answer **based only on the provided document** and returns it in the chat.

---

## Getting Started: How to Run This Demo

This demo runs entirely in a **single HTML file**. No server setup is needed.

### 1. Download the File
Save the `index.html` file from this project to your computer.

### 2. Get Your API Key
This demo uses the **Google Gemini API**.

- Go to [Google AI Studio](https://ai.google/).
- Sign in and click **Get API Key** (top-left or under "API keys").
- Create and copy a new API key.

### 3. Open the Demo
Open the `index.html` file in any modern web browser (Chrome, Firefox, Edge, etc.).

### 4. Add Your API Key
- In the demo's navigation bar, click the **Key icon (🔑)** in the top-right corner.
- An API Key row will appear. Paste your API key into the input field.
- Click **Save Key**. A green **API Key Saved** notification will appear.

### 5. Run the Guided Demo
- Click the **Demo Scenarios** tab.
- Follow the on-screen instructions to:
  - Add a secret document to the Knowledge Base.
  - Ask the "secret" question in the Chat tab.
  - View the results in the RAG Workflow tab.

---

**Enjoy experimenting with RAG-Bot and visualizing the power of Retrieval-Augmented Generation!**
