### NLP Sentiment Analysis API

- Project Description
    - Purpose: A secure and high-performance Natural Language Processing API.
    - Core Logic: Built using FastAPI and Hugging Face Transformers to analyze text sentiment and return structured results.
    - Architecture: Locally deployed pre-trained model to eliminate cloud dependencies and operational costs.
    - Privacy: Ensures data integrity as all processing occurs within the local environment.

- Key Features
    - Sentiment Analysis: High-accuracy classification using the DistilBERT transformer model.
    - Secure Access: Implementation of Bearer Token Authentication to protect the API asset.
    - Rate Limiting: Integrated SlowAPI to restrict traffic to 5 requests per minute per user.
    - Auto-Documentation: Automatic, interactive testing interfaces provided via Swagger UI and ReDoc.

- Tech Stack
    - FastAPI: High-performance, asynchronous backend framework.
    - Hugging Face Transformers: Industry-standard library for machine learning models.
    - DistilBERT: Optimized, lightweight model for sentiment classification.
    - SlowAPI: Middleware for system resource protection.
    - Python 3.10+: Core programming foundation.

- Group Roles and Contributions
    - Agnapan, Iverson: Model Selection (DistilBERT Model evaluation and testing).
    - Awikang, Rachiel: API Architecture, Endpoint Design, and PowerPoint.
    - Buyacao, Sean: NLP Engine integration, DevOps, and Git Strategy (.gitignore / GitHub).
    - Ofo-ob, John Mike: Security Middleware and Secret Management (.env implementation).

- Installation and Setup
    - Step 1 Clone the Repository: git clone https://github.com/aysha312/SIA.git
    - Step 2 Navigate to Directory: cd SIA
    - Step 3 Install Dependencies: pip install -r requirements.txt
    - Step 4 Configure Secrets: 
        - Create a file named '.env' in the root directory.
        - Retrieve the API_TOKEN from the private comment or attachment provided on Google Classroom.
        - Add the line: API_TOKEN=your_retrieved_token_here
    - Step 5 Launch the API: uvicorn main:app --reload