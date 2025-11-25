# Deep-Learning_-NLP
Deep Learning_ NLP
# Document Analysis and Topic Modeling System

## 📖 Project Overview
An AI-powered document analysis system that automatically extracts topics, generates summaries, and creates comprehensive reports from PDF documents using state-of-the-art NLP techniques including BERTopic and transformer models.

## 🚀 Features
- **PDF Text Extraction**: Automated extraction of text content from PDF files
- **Topic Modeling**: Advanced topic discovery using BERTopic with UMAP and HDBSCAN
- **Document Summarization**: Intelligent summarization using transformer models
- **Coherence Analysis**: Quantitative evaluation of topic quality
- **Automated Reporting**: Professional Word document generation with insights
- **GPU Acceleration**: Optimized performance with CUDA support

## 🛠️ Technology Stack
- **Natural Language Processing**: BERTopic, Sentence Transformers
- **Clustering**: UMAP (dimensionality reduction), HDBSCAN (density-based clustering)
- **Summarization**: Hugging Face Transformers (BART/DistilBART)
- **Text Processing**: PDFMiner, Gensim
- **Reporting**: python-docx for Word document generation
- **Environment**: Google Colab with GPU acceleration


## 🏗️ Architecture

### Data Processing Pipeline
1. **PDF Extraction** → Text preprocessing → Document chunking
2. **Embedding Generation** → Sentence transformers → Vector representations
3. **Topic Modeling** → UMAP + HDBSCAN → Topic clusters
4. **Summary Generation** → Transformer models → Document summaries
5. **Report Generation** → Automated Word documents → Final outputs

### Model Components
- **Embedding Model**: `all-mpnet-base-v2` for document representations
- **Dimensionality Reduction**: UMAP with cosine metric
- **Clustering**: HDBSCAN with optimized parameters
- **Summarization**: `sshleifer/distilbart-cnn-12-6` for efficient summarization

## 📊 Installation & Setup

### Prerequisites
- Python 3.8+
- Google Colab account (recommended)
- Google Drive for file storage

### Quick Start (Google Colab)
1. **Upload PDF** to Google Drive
2. **Open Notebook** in Google Colab
3. **Mount Drive** and set file path
4. **Run All Cells** for complete analysis
5. **Download Results** from generated Word documents

### Local Installation
```bash
# Clone repository
git clone https://github.com/yourusername/document-analysis-project.git
cd document-analysis-project

# Install dependencies
pip install -r requirements.txt

# Run in Jupyter notebook
jupyter notebook Document_Analysis_Notebook.ipynb
