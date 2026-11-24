# customerSupport_n8n
📧 Customer support emails never stop, so I built an AI agent that answers them using the company’s own knowledge!

Generic chatbots make up answers. I wanted replies grounded in real company information, so I built a RAG-powered support agent in n8n.

How it works:

📥 Gmail trigger: every new email starts the workflow.

🏷️ Text Classifier: AI decides whether the email is a genuine support query or something else. Irrelevant emails are ignored, so the agent never replies to spam or random mail.

🧠 AI Agent (Google Gemini): it understands the customer’s question.

📚 Supabase vector store + OpenAI embeddings: the agent searches the knowledge base for the most relevant information before answering.

✉️ Auto-reply: the answer is sent back to the customer in the same email thread.

What I learned:

How RAG (Retrieval-Augmented Generation) reduces AI hallucinations
Storing and searching embeddings in a vector database
Routing emails with classification before involving an agent
Giving an agent tools so it decides when to look things up

Faster responses for customers, and less repetitive work for the team. 🚀
