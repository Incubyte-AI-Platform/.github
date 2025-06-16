#  Cortex AI Platform

<div align="center">

![Cortex Logo](https://github.com/Incubyte-AI-Platform/.github/blob/main/images/logo.png)

**Automate Your RAG Development Lifecycle**

*Connect. Embed. Retrieve. Deploy.*


[🚀 Quick Start](#-quick-start) • [🎯 Use Cases](#-use-cases)

</div>

---

##  **Transform Your Organization's Knowledge Into Intelligent Conversations**

Cortex is an enterprise-grade AI platform that **automates the entire RAG (Retrieval-Augmented Generation) development lifecycle**. Deploy custom AI solutions in hours, not months, with zero AI expertise required.

> **🎪 The Magic**: Connect your data sources → Make them RAG-ready → Deploy intelligent chat, voice & search interfaces

<div align="center">
<img src="./assets/images/cortex-demo.gif" alt="Cortex Platform Demo" width="800"/>
</div>

---

## 🏗️ **Platform Architecture**

<div align="center">
<img src="https://github.com/Incubyte-AI-Platform/.github/blob/main/images/Screenshot%202025-06-16%20at%204.14.48%20PM.png" alt="Cortex Architecture" width="900"/>
</div>

---

## 🔧 **Three Powerful Modules**

### 📡 **1. Data Collection Engine**
*Connect everything, everywhere*

The Data Collection Module automatically connects, authenticates, and continuously syncs data from your organization's diverse systems into a unified format that can be processed by AI.

<img src="https://github.com/Incubyte-AI-Platform/.github/blob/main/images/Data%20Collection.png" alt="Data Collection" width="64" align="left"/>

**Pre-built connectors for your entire tech stack:**
- **Productivity**: Gmail, Google Drive, Slack
- **Knowledge Bases**: Confluence, SharePoint  
- **Web Sources**: Websites, Social media
- **Custom Sources**: We build it for you

### **Docker Compose (Local Development)**

- Build with a specific Dockerfile: 
 docker buildx build --platform linux/amd64 --provenance=false -t embedding-and-storage:v1 -f Dockerfile.Azure .

- Build for AWS with Azure Artifact URL:
  docker buildx build \
    --no-cache \
    --platform linux/amd64 \
    --provenance=false \
    --build-arg AZURE_PYPI_INDEX_URL=https://__token__:{Personal Access Token}@pkgs.dev.azure.com/IncubyteLLP/Cortex/_packaging/Cortex-Connector-Package/pypi/simple/ \
    -t gmail-connector:v1.2 \
    -f Dockerfile.Lambda .


### 🧠 **2. Data Embedding Module**
*Make your data AI-ready automatically*

<img src="https://github.com/Incubyte-AI-Platform/.github/blob/main/images/Data%20Embedding%20and%20Storage.png" alt="Data Embedding" width="64" align="left"/>

**Intelligent preprocessing and vectorization:**
- **Smart Chunking**: Context-aware document segmentation
- **Multi-format Support**: PDFs, Word docs, presentations, code, images
- **Vector Generation**: State-of-the-art embedding models
- **Metadata Enrichment**: Automatic tagging and categorization using metadata filtering

- Build with a specific Dockerfile: 
 docker buildx build --platform linux/amd64 --provenance=false -t embedding-and-storage:v1 -f Dockerfile.Azure .

### 🎯 **3. RAG API Engine**
*Retrieve the perfect answers, every time*

<img src="https://github.com/Incubyte-AI-Platform/.github/blob/main/images/RAG%20API.png" alt="RAG API" width="64" align="left"/>

**Advanced retrieval with enterprise features:**
- **Hybrid Search**: Combines semantic and keyword search
- **Context-Aware Retrieval**: Understands conversation history
- **Multi-LLM Support**: GPT-4, Claude, Gemini, or your own models
- **Cloud Agnostic**: GCP, AWS, Azure or your own cloud


## ✨ **Why Organizations Choose Cortex**

### 🏃‍♂️ **Speed to Market**
- **Ready-made POCs**: Deploy in hours with pre-built templates

### 💰 **Cost Efficiency** 
- **Zero AI Expertise Required**: Our AI handles the AI complexity
- **Flexible Pricing**: Pay for what you use, scale as you grow
- **ROI Guaranteed**: See measurable productivity gains in weeks

### 🔓 **No Vendor Lock-In**
- **Your Cloud**: Deploy on Azure, AWS, GCP, or on-premises
- **Your LLMs**: Use any language model or mix multiple providers
- **Your Data**: Full control, zero data sharing, complete compliance

### 🛡️ **Enterprise-Ready**
- **Security First**: SOC2, GDPR, HIPAA compliant
- **Scalable Architecture**: Handle millions of queries per day
- **24/7 Support**: Dedicated enterprise support team

---

## 🎯 **Use Cases**

<details>
<summary><strong>🤖 AI Companions for Organizations</strong></summary>

Transform your workforce productivity with intelligent AI assistants that know your business inside-out.

**Examples:**
- **"Cortex Helper"**: Your organization's internal ChatGPT
- **"Parent Companion"**: Instant answers to your child's school needs and preparation 
- **"Onboarding Assistant"**: Guide new employees through your processes

*ROI: 40% reduction in internal support tickets*
</details>

<details>
<summary><strong> Healthcare Patient Experience</strong></summary>

Enhance patient care with AI that understands medical protocols and patient needs.

**Examples:**
- **Patient Portal Assistant**: 24/7 support for patient questions
- **Clinical Decision Support**: AI-assisted diagnosis and treatment recommendations
- **Medical Records Intelligence**: Instant access to patient history and insights

*ROI: 50% reduction in routine medical inquiries*
</details>

<details>
<summary><strong>🏢 Front Office Productivity</strong></summary>

Transform your customer-facing teams into productivity powerhouses with AI assistance.

**Examples:**
- **Customer Support AI**: Instant, accurate answers to customer questions
- **Sales Assistant**: AI that knows your entire product catalog and pricing
- **Reception Intelligence**: Smart call routing and appointment scheduling

*ROI: 60% faster customer query resolution*
</details>

---

## 🚀 **Quick Start**

### Prerequisites
- **Cloud Account**: Azure or AWS
- **Container Runtime**: Docker
- **API Keys**: For Vector Database, Choice of LLM
- **Python**: Version 3.12 or above
- **NodeJS**: Version 20 or above
- **Domain**: For web interfaces (optional)

### 1. **Docker Compose (Local Development)**

## Clone the repository

- To begin with the local setup, start cloning the repository using the `git clone <repository_link>` command.
- You can use either the HTTPS or SSH links for cloning.

### Using HTTPS

```
git clone https://IncubyteLLP@dev.azure.com/IncubyteLLP/Cortex/_git/data-collection.git
```

### Using SSH

```
git clone git@ssh.dev.azure.com:v3/IncubyteLLP/Cortex/data-collection.git
```

- [How to setup SSH key authentication](https://learn.microsoft.com/en-us/azure/devops/repos/git/use-ssh-keys-to-authenticate?view=azure-devops)

## Add Environment variables

- Move into the "data-collection" directory using

```
cd data-collection
```

- Create a new file `.env`.
- Add the below mentioned environment variables in the `.env` file.

```
# Default variables
ENV=local
CLOUD_PROVIDER=AWS


# Configurable variables

# DynamoDB access credentials
CONFIG_REGION
CONFIG_AWS_ACCESS_KEY_ID
CONFIG_AWS_SECRET_ACCESS_KEY

# AWS Textract access credentials
AWS_TEXTRACT_TEST_ACCESS_KEY
AWS_TEXTRACT_TEST_SECRET_ACCESS_KEY
AWS_TEXTRACT_TEST_REGION
```

## Developer setup

Follow this setup for **local development**

- Use python version **3.12** or above.
- Download uv as the package manager using pip command.

```
pip install uv

# or

pip3 install uv
```

- Create a virtual environment

```
uv venv
```

- Enter the virtual environment

  - For windows `.\venv\Scripts\activate`
  - For linux/MacOS `source .venv/bin/activate`
  - To exit the virtual environment run `deactivate` for both windows & linux/MacOS.

- Install all dependencies.

```
uv sync
```

- Add new dependency in the project

```
uv add <package_name>
```

- Remove existing dependency

```
uv remove <package_name>
```

## Docker setup

- Run the application using docker

### Start Docker engine

- Open the Docker desktop app to start the docker engine.

### Build local docker image

```
docker build -f ./Dockerfile.Azure -t data-collection-app .
```

### Run the application

- You can run the application using the `.env` file that we created.

```
docker run --env-file .env data-collection-app
```

- To stop the execution you can do `CTRL+C` in the terminal. Or stop manually from the docker desktop app.
```bash


## 📊 **Platform Components**

| Component | Repository | Documentation | Status |
|-----------|------------|---------------|---------|
| 🎨 **Frontend (React UI)** | [`cortex-frontend`](./packages/frontend) | [📖 Frontend Docs](./packages/frontend/README.md) | [![Build Status](https://img.shields.io/badge/build-passing-green.svg)](https://github.com/your-org/cortex-frontend/actions) |
| ⚡ **RAG API (NestJS)** | [`cortex-api`](./packages/api) | [📖 API Docs](./packages/api/README.md) | [![Build Status](https://img.shields.io/badge/build-passing-green.svg)](https://github.com/your-org/cortex-api/actions) |
| 🎤 **Voice Services** | [`cortex-voice`](./packages/voice) | [📖 Voice Docs](./packages/voice/README.md) | [![Build Status](https://img.shields.io/badge/build-passing-green.svg)](https://github.com/your-org/cortex-voice/actions) |
| 🔌 **Data Connectors** | [`cortex-connectors`](./packages/connectors) | [📖 Connectors Docs](./packages/connectors/README.md) | [![Build Status](https://img.shields.io/badge/build-passing-green.svg)](https://github.com/your-org/cortex-connectors/actions) |
| 🧠 **Embedding Engine** | [`cortex-embeddings`](./packages/embeddings) | [📖 Embeddings Docs](./packages/embeddings/README.md) | [![Build Status](https://img.shields.io/badge/build-passing-green.svg)](https://github.com/your-org/cortex-embeddings/actions) |
| 🏗️ **ChatPackage** | [`cortex-infrastructure`](./infrastructure) | [📖 DevOps Docs](./infrastructure/README.md) | [![Terraform](https://img.shields.io/badge/terraform-validated-purple.svg)](https://github.com/your-org/cortex-infrastructure) |

---


## 📈 **Monitoring & Analytics**

- **Real-time Metrics**: Query volume, response times, user satisfaction
- **Usage Analytics**: Most searched topics, popular data sources, user patterns  
- **Performance Monitoring**: System health, resource utilization, error rates
- **Business Intelligence**: ROI tracking, productivity metrics, cost analysis

---

### 🐛 **Issues & Feature Requests**

- **🐛 [Report a Bug](https://github.com/your-org/cortex/issues/new?template=bug_report.md)**
- **💡 [Request a Feature](https://github.com/your-org/cortex/issues/new?template=feature_request.md)**
- **❓ [Ask a Question](https://github.com/your-org/cortex/discussions/new?category=q-a)**

---

## 🗺️ **Roadmap**

<details>
<summary><strong>🎯 Q3 2025</strong></summary>

- **Multi-modal AI**: Image and video understanding
- **AI Agents**:  Autonomous Task Completion
- **Agentic Workflows**: AI agents at the core of your workflow 
</details>

---

## ⚖️ **License**

See the [LICENSE](./LICENSE) file for details.

---

Built with ❤️ by the Cortex team and our amazing community contributors.

---

<div align="center">

**Ready to transform your organization's knowledge into intelligent conversations?**

[🚀 **Get Started Now**](https://cortex-ai.com/get-started) • [📅 **Book a Demo**](https://calendly.com/cortex-ai/demo) • [💬 **Contact Sales**](mailto:sales@cortex-ai.com)

---

