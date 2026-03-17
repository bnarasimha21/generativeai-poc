# Generative AI POC

A comprehensive collection of proof-of-concept applications exploring generative AI capabilities. Includes examples using IBM Generative AI SDK, HuggingFace models, LangChain integrations, and practical use cases like feedback analysis and sentiment classification.

## Features

- **Text generation** -- Code generation, poem writing, and summarization using IBM Generative AI (BAM) SDK
- **Sentiment analysis** -- Analyze feedback and survey data for sentiment classification
- **Text summarization** -- Summarize feedback text using LLM models (FLAN-UL2, StarCoder, etc.)
- **RAG (Retrieval-Augmented Generation)** -- Question answering with LangChain and ChromaDB vector store
- **Image generation** -- Text-to-image generation using Stable Diffusion via HuggingFace Diffusers
- **Feedback analysis use cases** -- End-to-end pipelines with Flask APIs and Angular frontend
- **LangChain integration** -- Multiple examples of LangChain chains, retrieval QA, and sequential chains
- **Jupyter notebooks** -- Interactive exploration and experimentation

## Tech Stack

- **Language:** Python, Jupyter Notebook
- **AI/ML SDKs:** IBM Generative AI SDK (`ibm-generative-ai`), HuggingFace Diffusers, LangChain
- **Models:** FLAN-UL2, StarCoder, Stable Diffusion v1.5
- **Vector Store:** ChromaDB
- **Embeddings:** OpenAI Embeddings, Sentence Transformers
- **Web Frameworks:** Flask (API endpoints), Angular (feedback analysis frontend)
- **Data:** pandas, matplotlib, plotly
- **Other:** python-dotenv, Streamlit, pypdf

## Project Structure

```
generativeai-poc/
├── HuggingFace/               # HuggingFace model examples
│   └── texttoimage.py         # Stable Diffusion text-to-image
├── ibm-generative-ai/         # IBM GenAI SDK examples
│   ├── generate.py            # Text generation
│   ├── sentiment.py           # Sentiment analysis
│   ├── summarize.py           # Text summarization
│   ├── codegen.py             # Code generation
│   ├── langchain_retrievalQA.py  # RAG with LangChain
│   ├── rag.ipynb              # RAG notebook
│   └── ...
├── use-cases/
│   ├── feedback_sentiment/    # Feedback sentiment API & analysis
│   ├── feedback_summary/      # Feedback summarization with Flask
│   ├── feedback_analysis/     # Angular frontend for feedback
│   └── challenge/             # Survey sentiment challenge
├── Others/                    # Miscellaneous experiments
├── assets/                    # Sample data files (CSV, JSON, PDF)
├── requirements.txt
└── cookbook.ipynb
```

## Setup / Installation

```bash
git clone https://github.com/bnarasimha21/generativeai-poc.git
cd generativeai-poc
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

Set up environment variables in a `.env` file:

```
GENAI_KEY=<your-ibm-genai-api-key>
GENAI_API=<your-ibm-genai-api-endpoint>
OPEN_AI_KEY=<your-openai-key>  # Required for RAG examples
```

## Usage

### Text Generation
```bash
python ibm-generative-ai/generate.py
```

### Sentiment Analysis
```bash
python ibm-generative-ai/sentiment.py
```

### Feedback Summary API
```bash
cd use-cases/feedback_summary
python flask_endpoint.py
```

### Text-to-Image (requires GPU)
```bash
python HuggingFace/texttoimage.py
```

### Jupyter Notebooks
```bash
jupyter notebook cookbook.ipynb
```

## License

MIT
