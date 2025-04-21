# ✈️ Travel Booking AI Assistant

An AI-powered travel booking assistant built using Google Gemini 1.5 Flash models, Retrieval Augmented Generation (RAG), and few-shot prompting. This project simulates smart travel ticket booking workflows, structured output generation, and dynamic FAQ retrieval using embeddings.

---

## 📚 Project Features

- ✅ Structured Output / JSON Mode (Flight booking details)
- ✅ Few-shot Prompting (Booking examples to guide generation)
- ✅ Retrieval Augmented Generation (Mini-RAG for FAQs)
- ✅ Embeddings and Similarity Search (Sentence Transformers)
- ✅ Function Calling Simulation (Ticket Booking System)
- ✅ Light Gen AI Evaluation (JSON parsing and error handling)

---

## 🏗️ Technologies Used

- Google Generative AI (`google-generativeai` Python SDK)
- Google Gemini 1.5 Flash model
- Sentence Transformers (`all-MiniLM-L6-v2`)
- Python 3
- Kaggle Notebook Environment

---

## 🚀 How It Works

1. **Few-shot Prompting:** Provide example travel bookings to Gemini to control response format.
2. **Generate Content:** Gemini Flash generates structured JSON output based on user input.
3. **Parse and Validate:** Parse the generated JSON safely to extract flight booking details.
4. **Book Ticket Simulation:** Simulate booking with a simple Python function.
5. **FAQ Retrieval:** Search for frequently asked travel questions using sentence embeddings and similarity scoring.

---

## 🧩 Example Flow

```mermaid
graph TD;
    User_Input --> Few-shot_Prompting
    Few-shot_Prompting --> Gemini_Response
    Gemini_Response --> JSON_Parsing
    JSON_Parsing --> Book_Ticket_Function
    User_Input --> FAQ_Query
    FAQ_Query --> Embeddings_Search
    Embeddings_Search --> FAQ_Answer
