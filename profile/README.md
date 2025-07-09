#  Incubyte AI Platform

<div align="center">

![Incubyte AI Platform Logo](https://github.com/Incubyte-AI-Platform/.github/blob/main/images/logo.png)

**Automate Your RAG Development Lifecycle**

*Connect. Embed. Retrieve. Deploy.*


[🚀 Quick Start](#-quick-start) • [🎯 Use Cases](#-use-cases)

</div>

---

##  **Transform Your Organization's Knowledge Into Intelligent Conversations**

Incubyte AI Platform is an enterprise-grade AI platform that **automates the entire RAG (Retrieval-Augmented Generation) development lifecycle**. Deploy custom AI solutions in hours, not months, with zero AI expertise required.

Connect your data sources → Make them RAG-ready → Deploy intelligent chat, voice & search interfaces

<div align="center">
<img src="./assets/images/Incubyte AI Platform-demo.gif" alt="Incubyte AI Platform Platform Demo" width="900"/>
</div>

---

##  **Platform Architecture**

The platform automates the RAG lifecycle with three layers: Data Collection connects and syncs sources like Gmail and Slack; Embedding & Storage transforms content into AI-ready vectors; and Retrieval delivers precise, context-aware answers using hybrid search and LLMs.

 - [Dive into the platform architecture](https://github.com/Incubyte-AI-Platform/.github/blob/main/images/Cortex%20Architecture.pdf)
---

##  **Three Powerful Modules**

###  **1. Data Collection Engine**
*Connect everything, everywhere*

The Data Collection Module automatically connects, authenticates, and continuously syncs data from your organization's diverse systems into a unified format that can be processed by AI.


**Pre-built connectors for your entire tech stack:**
- **Productivity**: Gmail, Google Drive, Slack
- **Knowledge Bases**: Confluence, SharePoint  
- **Web Sources**: Websites, Social media
- **Custom Sources**: We build it for you

###  **2. Data Embedding Module**
*Make your data AI-ready automatically*

**Intelligent preprocessing and vectorization:**
- **Smart Chunking**: Context-aware document segmentation
- **Multi-format Support**: PDFs, Word docs, presentations, code, images
- **Vector Generation**: State-of-the-art embedding models
- **Metadata Enrichment**: Automatic tagging and categorization using metadata filtering


###  **3. RAG API Engine**
*Retrieve the perfect answers, every time*

**Advanced retrieval with enterprise features:**
- **Hybrid Search**: Combines semantic and keyword search
- **Context-Aware Retrieval**: Understands conversation history
- **Multi-LLM Support**: GPT-4, Claude, Gemini, or your own models
- **Cloud Agnostic**: GCP, AWS, Azure or your own cloud


##  **Why Organizations Choose Incubyte AI Platform**

###  **Speed to Market**
- **Ready-made POCs**: Deploy in hours with pre-built templates

###  **Cost Efficiency** 
- **Zero AI Expertise Required**: Our AI handles the AI complexity
- **Flexible Pricing**: Pay for what you use, scale as you grow
- **ROI Guaranteed**: See measurable productivity gains in weeks

###  **No Vendor Lock-In**
- **Your Cloud**: Deploy on Azure, AWS, GCP, or on-premises
- **Your LLMs**: Use any language model or mix multiple providers
- **Your Data**: Full control, zero data sharing, complete compliance

###  **Enterprise-Ready**
- **Security First**: Compliance from day one
- **Scalable Architecture**: Handle millions of queries per day
- **24/7 Support**: Dedicated enterprise support team

---

##  **Use Cases**

<details>
<summary><strong> AI Companions for Organizations</strong></summary>

Transform your workforce productivity with intelligent AI assistants that know your business inside-out.

**Examples:**
- **"Incubyte AI Platform Helper"**: Your organization's internal ChatGPT
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
<summary><strong> Front Office Productivity</strong></summary>

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

## Clone the repository

- To begin with the local setup, start cloning the repository using the `git clone <repository_link>` command.
- You can use either the HTTPS or SSH links for cloning.

### Using HTTPS

```
git clone https://IncubyteLLP@dev.azure.com/IncubyteLLP/Incubyte AI Platform/_git/repo-name.git
```

### Using SSH

```
git clone git@ssh.dev.azure.com:v3/IncubyteLLP/Incubyte AI Platform/repo-name.git
```

- [How to setup SSH key authentication](https://learn.microsoft.com/en-us/azure/devops/repos/git/use-ssh-keys-to-authenticate?view=azure-devops)


##  **Platform Components**

| Component | Repository | Documentation | Status |
|-----------|------------|---------------|---------|
|  **RAG API Engine)** | [`Incubyte AI Platform-RAG Engine`](https://github.com/Incubyte-AI-Platform/rag-package) | [📖 RAG API Docs] (https://github.com/Incubyte-AI-Platform/rag-package/blob/main/README.md) | [![Build Status](https://img.shields.io/badge/build-passing-green.svg)](https://github.com/Incubyte-AI-Platform/rag-package/actions) |
|  **Embedding Engine** | [`Incubyte AI Platform-embeddings`](https://github.com/Incubyte-AI-Platform/embedding-and-storage) | [📖 Embeddings Docs](https://github.com/Incubyte-AI-Platform/embedding-and-storage/blob/main/README.md) | [![Build Status](https://img.shields.io/badge/build-passing-green.svg)](https://github.com/Incubyte-AI-Platform/embedding-and-storage/actions) |
|  **Connector Package** | [`Incubyte AI Platform-Connector Package`](https://github.com/Incubyte-AI-Platform/connector-packages) | [📖 Connector Docs](https://github.com/Incubyte-AI-Platform/embedding-and-storage/blob/main/README.md) | [![Build Status](https://img.shields.io/badge/build-passing-green.svg)](https://github.com/Incubyte-AI-Platform/embedding-and-storage/actions) |
|  **Gmail Connector** | [`Incubyte AI Platform-gmail connector`](https://github.com/Incubyte-AI-Platform/gmail-connector) | [📖 Gmail Connector Docs](https://github.com/Incubyte-AI-Platform/gmail-connector/blob/main/README.md) | [![Build Status](https://img.shields.io/badge/build-passing-green.svg)] (https://github.com/Incubyte-AI-Platform/gmail-connector/actions/new) |
|  **Website Connector** | [`Incubyte AI Platform-website connector`](https://github.com/Incubyte-AI-Platform/website-connector) | [📖 Website Connector Docs](https://github.com/Incubyte-AI-Platform/connector-packages/blob/main/README.md) | [![Build Status](https://img.shields.io/badge/build-passing-green.svg)] (https://github.com/Incubyte-AI-Platform/connector-packages/actions/new) |

---

###  **Issues & Feature Requests**

- ** [Raise a PR](https://github.com/your-org/Incubyte AI Platform/issues/new?template=bug_report.md)**
- ** [Report a Bug](https://github.com/your-org/Incubyte AI Platform/issues/new?template=bug_report.md)**
  

---

##  **Roadmap**

<details>
<summary><strong> Q3 2025</strong></summary>

- **Multi-modal AI**: Image and video understanding
- **AI Agents**:  Autonomous Task Completion
- **Agentic Workflows**: AI agents at the core of your workflow 
</details>

---

##  **License**

See the [LICENSE](https://github.com/Incubyte-AI-Platform/.github/blob/main/LICENSE.md)

---

Built with ❤️ by the Incubyte team and our amazing community contributors.

---

<div align="center">

**Ready to transform your organization's knowledge into intelligent conversations?**

[🚀 **Get Started Now**](https://cortex.incubyte.co/) • [📅 **Book a Demo**](https://www.incubyte.co/contact-us) • [💬 **Contact Sales**](https://www.incubyte.co/contact-us)

---

