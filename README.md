# AI Resume Analyzer & Job Match 🚀

An **AI-powered recruitment assistant** that analyzes resumes (CVs) and automatically recommends the most suitable job positions.  
It leverages **AWS Cloud Services** for scalable storage, data extraction, and AI/ML model inference.

---

## ✨ Features

- 📄 **Resume Parsing** – Upload resumes in PDF format, extract structured data using **Amazon Textract**.  
- 🤖 **AI Skill & Experience Matching** – Process CVs with **AWS Bedrock** to identify candidate skills and compare against job descriptions.  
- 🔍 **Job Search & Ranking** – Store and search job descriptions in **Amazon OpenSearch / Kendra** with semantic search and ranking.  
- 💬 **Chatbot Advisor** – Ask natural language questions like *“Which jobs fit this CV?”* and receive AI-powered recommendations.  
- 📊 **Dashboard** – Upload CVs, view extracted info, and explore the **Top 5 job matches** with detailed reasoning.  

---

## 🏗️ Architecture
![System Architecture](docs/overview_architecture.png)
- **Frontend:** ReactJS + AWS Amplify / S3 + CloudFront  
- **Backend:** Python FastAPI, AWS Lambda + API Gateway + Step Functions  
- **AI/ML:** Amazon Textract, AWS Bedrock (Claude, Titan) / SageMaker  
- **Database & Search:** S3 (raw files), DynamoDB (metadata), OpenSearch / Kendra (job descriptions), RDS Aurora (structured storage)  
- **Security:** IAM, KMS, CloudTrail, GuardDuty  