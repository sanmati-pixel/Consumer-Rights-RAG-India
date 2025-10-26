# Consumer-Rights-RAG-India
💡 Project: NyaySaarthi (The Guide to Justice)

NyaySaarthi is a Retrieval-Augmented Generation (RAG) system built to democratize access to consumer law in India. It serves as an accurate, open-source legal assistant, ensuring consumers get answers grounded solely in official statutes.

Core Mission

To provide fast, reliable, and source-verifiable information regarding the rights and redressal mechanisms established under the Indian Consumer Protection Act, 2019 (CPA 2019).

Why RAG? (The Value Proposition)

Traditional Large Language Models (LLMs) often suffer from "hallucination," which is unacceptable when dealing with legal advice. NyaySaarthi mitigates this risk by:

Grounding: All answers are generated only from retrieved text snippets of the official CPA 2019 document.

Verifiability: Every generated response is accompanied by the exact source citation (the specific section/chunk of the Act) it used.

Focus: The system's knowledge base is narrow (CPA 2019), making the answers deeply specialized and highly relevant to Indian consumer rights.

Key Functionality

Users can ask practical, real-world questions, and NyaySaarthi will respond with legally compliant guidance, such as:

"What is the time limit for filing a complaint about a defective product?"

"Who is liable for a misleading advertisement on an e-commerce site?"

"What is the monetary jurisdiction of the District Consumer Commission?"

🛠️ Technology Stack
Data Source                                  Raw CPA 2019 Document                                        (PDF The legal knowledge base.

Embedding Model                              sentence-transformers/all-MiniLM-L6-v2                       Converts text chunks into numerical vectors.

Vector Store                                 FAISS                                                        Stores embeddings for rapid similarity search.

Framework                                    LangChain / Custom Python Scripts                            Orchestrates the RAG pipeline.                             

LLM                                          [Specify your chosen LLM, e.g., Llama 3 (Local) or Gemini    Generates the final, human-readable answer.
