# SmartDialog AI – Context-Aware Conversational Engine

SmartDialog AI is a flexible and robust chatbot system that empowers users to train an AI assistant using personalized data sources including documents, web content, and multimedia transcripts. It is built on a scalable backend using Django REST Framework and connects with modern AI tools to deliver human-like interactions.

Whether you want to build a customer support assistant, an educational tutor, or a personalized knowledge retriever, SmartDialog AI provides the tools to do so with ease and reliability.

---

## 🔧 Key Features

• **Multi-source Knowledge Ingestion**  
  Train your chatbot using a variety of sources, such as PDFs, website URLs, plain text, and video subtitles.

• **Modern Authentication System**  
  Supports secure login with Google via social authentication for seamless onboarding.

• **Advanced AI Conversation Engine**  
  Integrates with GPT-based models for natural and context-aware dialogue.

• **High-performance Vector Search**  
  Leverages FAISS and Pinecone for fast, scalable similarity search on embedded content.

• **Efficient File Handling and Parsing**  
  Uses the Langchain library to process and transform files into embeddable knowledge.

• **Environment-Specific Configuration**  
  Clearly separated settings for development, staging, and production workflows.

• **Customizable Prompts and Branding**  
  Easily adjust default prompts and application metadata through a dynamic site configuration.

• **Multilingual Ready**  
  Offers support for multiple languages with future improvements planned for auto-detection.

• **Integrated Task Queues**  
  Async background tasks managed using Celery with Redis or AWS SQS.

• **Cloud-Friendly File Storage**  
  Compatible with AWS S3 for scalable file storage and access.

---

## ⚙️ Tech Stack

• **Language**: Python  
• **Backend Framework**: Django REST Framework  
• **Database**: PostgreSQL  

### 🔌 Libraries & Tools

• Celery  
• OpenAI  
• Langchain  
• FAISS  
• Pinecone  
• Django-Allauth (for social login)  

---

## 📦 Requirements

• Python 3.8 or newer  
• Django 4.1+  
• OpenAI API Key  
• Pinecone API Key  
• Redis or AWS SQS (for task queue)  
• PostgreSQL Database  

---

## 🚀 Installation Guide

1. **Clone the repository**  
   ```bash
   git clone https://github.com/your-username/smartdialog-ai.git
   cd smartdialog-ai
   ```

2. **Install dependencies**  
   ```bash
   pip install -r requirements.txt
   ```

3. **Run background tasks with Celery**  
   ```bash
   celery -A config worker --loglevel=info
   ```

4. **Start the development server**  
   ```bash
   python manage.py runserver
   ```

5. **Open your browser**  
   Visit `http://127.0.0.1:8000/` to access the chatbot interface.

---

## 🐧 Linux/macOS Setup Notes

Make sure required system packages are installed:

```bash
sudo apt install python3-dev libcurl4-openssl-dev gcc libssl-dev -y
pip install --upgrade pip setuptools
pip install pycurl
```

---

## ☁️ Deployment Options

You can deploy SmartDialog AI on platforms like **Heroku** or **AWS** by following the standard Django deployment best practices.

---

## ⚠️ Notes

• If you are not using AWS SQS, skip installing `pycurl` and `boto3`.  
• If AWS S3 is not needed, you can omit `django-storages`.  
• Make sure to generate your OpenAI API key before launching the app.

---

## 🔮 Future Enhancements

• Extend support to additional media types and file formats  
• Improved understanding of user queries with advanced NLP techniques  
• Deeper multilingual support with automatic translation  
• Native integration with messaging platforms like Slack and WhatsApp  
• Real-time analytics for chat performance

---

## 🎉 Final Words

SmartDialog AI is built with modularity and extensibility in mind. Whether you're building an AI tutor or a support agent, you can tailor it to meet your specific needs. Contributions are welcome.

Build smarter conversations with your content, your way.
