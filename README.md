# NexaBrand: AI-Powered Branding Assistant

![NexaBrand Banner](https://your-image-url.com/banner.png)

## Overview
NexaBrand is a **full-stack SaaS application** that generates AI-driven branding snippets and keyword suggestions for businesses. This project serves as a tutorial for building AI-powered SaaS applications from scratch, leveraging modern cloud technologies.

## 🚀 Live Demo
🔗 **Try out the live demo here** (Authentication Required): [NexaBrand](https://www.nexabrand.co)

## ✨ Features
- AI-generated brand snippets and keyword suggestions
- Full authentication system
- Serverless architecture for scalability
- Responsive and modern UI with TailwindCSS
- Deployed on AWS Lambda and Vercel

## 🛠 Tech Stack

### Backend Stack
| Type      | Tech      |
|-----------|----------|
| Language  | Python   |
| Framework | FastAPI  |
| Hosting   | AWS (Lambda + API Gateway) |
| Other     | OpenAI API, AWS CDK, Docker |

### Frontend Stack
| Type      | Tech      |
|-----------|----------|
| Language  | TypeScript |
| Framework | Next.js / React |
| Styling   | TailwindCSS |
| Hosting   | Vercel |

## 📦 Setup Instructions

### Prerequisites
Ensure you have the following installed:
- **Node.js** (v16+)
- **Python 3.9+**
- **AWS CLI** (configured with necessary permissions)
- **Docker** (for building Lambda layers)
- **CDK CLI** (for AWS Infrastructure deployment)

### Backend Setup
```sh
# Clone the repository
git clone https://github.com/yourusername/nexabrand.git
cd nexabrand

# Set up a virtual environment and install dependencies
python -m venv venv
source venv/bin/activate   # On Windows, use `venv\Scripts\activate`
pip install -r requirements.txt

# Run the backend locally
uvicorn app.main:app --reload
```
The backend will be available at `http://127.0.0.1:8000`.

### Frontend Setup
```sh
# Navigate to the frontend directory
cd frontend

# Install dependencies
npm install

# Run the development server
npm run dev
```
The frontend will be available at `http://localhost:3000`.

### 🚀 AWS Deployment
```sh
# Deploy backend using AWS CDK
cd nexabrand-infra
cdk deploy

# Deploy frontend to Vercel
vercel --prod
```

## 📂 Lambda Layer ZIP
For users having trouble building the Lambda layer, the pre-built layer is available in:
```
nexabrand-infra/lambda_base_layer/layer.zip
```
You can either build it manually using Docker or use the provided file.

## 📡 API Endpoints
| Method | Endpoint | Description |
|--------|---------|-------------|
| POST   | `/generate-snippet` | Generates branding snippets using OpenAI |
| POST   | `/generate-keywords` | Suggests brand-related keywords |
| GET    | `/status` | Health check for the API |

---
🚀 **Start building with NexaBrand today!** 🚀