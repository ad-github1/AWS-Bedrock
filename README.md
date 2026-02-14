
# AWS Bedrock – Foundation Model Integration with Python

This project demonstrates how to integrate and interact with foundation models hosted on **Amazon Web Services (AWS)** using **Amazon Bedrock**.

It provides example implementations for:

* Text generation using Claude
* Text generation using Llama 2
* Image generation using Stable Diffusion
* Model invocation using AWS SDK (Boto3)

The repository serves as a practical reference for developers building GenAI applications on AWS.

---

##  Features

* 🔹 Invoke Claude models via Bedrock
* 🔹 Invoke Llama 2 models via Bedrock
* 🔹 Generate images using Stable Diffusion
* 🔹 Structured JSON-based prompt handling
* 🔹 Modular Python scripts for each model
* 🔹 Simple, extensible architecture

---

##  Project Structure

```
AWS-Bedrock/
│
├── app.py                # Main application entry point
├── claude.py             # Claude model invocation
├── llama2.py             # Llama 2 model invocation
├── stablediffusion.py    # Stable Diffusion image generation
├── test.json             # Sample input payload
├── requirements.txt      # Project dependencies
└── README.md             # Project documentation
```

---

##  Models Used

This project demonstrates integration with foundation models available in **Amazon Bedrock**, including:

* **Claude** (Anthropic)
* **Llama 2** (Meta)
* **Stable Diffusion** (Text-to-image)

> Note: Model availability depends on your AWS region and access permissions.

---

##  Prerequisites

Before running this project, ensure:

1. You have an active AWS account.
2. You have access to Amazon Bedrock in your AWS region.
3. AWS credentials are configured locally:

```bash
aws configure
```

4. Python 3.8+ installed.

---

##  Installation

Clone the repository:

```bash
git clone https://github.com/krishnaik06/AWS-Bedrock.git
cd AWS-Bedrock
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

##  AWS Configuration

Make sure your IAM role/user has permissions for:

* `bedrock:InvokeModel`
* `bedrock:InvokeModelWithResponseStream`

You can verify Bedrock access in the AWS Console.

---

##  Running the Application

### Run Claude Example

```bash
python claude.py
```

### Run Llama 2 Example

```bash
python llama2.py
```

### Run Stable Diffusion Example

```bash
python stablediffusion.py
```

---

##  Example Payload

The `test.json` file contains sample request bodies used to invoke models. You can modify prompts according to your use case.

---

##  Technologies Used

* Python
* Boto3 (AWS SDK for Python)
* Amazon Bedrock
* JSON

---

##  Use Cases

* Generative AI applications
* Conversational AI systems
* Image generation platforms
* LLM-based backend services
* Rapid prototyping of foundation model integrations

---

##  Future Improvements

* Streamlit / FastAPI UI integration
* RAG (Retrieval-Augmented Generation) pipeline
* Multi-model routing
* Deployment using AWS Lambda
* Docker containerization

---

##  License

This project is licensed under the GPL-3.0 License.

