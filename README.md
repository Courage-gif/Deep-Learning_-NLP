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

## 📁 Project Structure
document-analysis-project/
│
├── 📓 Document_Analysis_Notebook.ipynb # Main Colab notebook
├── 📄 requirements.txt # Python dependencies
├── 📄 README.md # Project documentation
├── 📄 LICENSE # MIT License
└── 📁 sample_output/ # Example outputs (optional)
├── Topic_Modeling_Results.docx
└── Global_Summary_Report.docx


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

🎯 Usage
Basic Usage
Prepare Document: Place PDF file in Google Drive

Configure Path: Update PDF_FILE_PATH in notebook

Execute Analysis: Run all cells sequentially

Review Outputs: Check generated Word reports

Advanced Configuration
Adjust MAX_DOCS parameter for document limit

Modify UMAP/HDBSCAN parameters for clustering sensitivity

Change summarization model for different quality/speed trade-offs

📈 Outputs Generated
1. Topic Modeling Report
Topic clusters with representative keywords

Document distribution across topics

Coherence scores for topic quality

Representative document examples

2. Global Summary Report
Comprehensive document summary

Reading time estimation

Document complexity assessment

Reading strategy recommendations

Statistical analysis

3. Visualizations (Optional)
Topic distribution charts

Document clustering visualization

Topic hierarchy trees

⚙️ Configuration
Key Parameters
python
# Document Processing
MAX_DOCS = 2500          # Maximum documents to process
MAX_CHARS = 800          # Chunk size for summarization

# Topic Modeling
UMAP_NEIGHBORS = 15      # Local neighborhood size
HDBSCAN_MIN_CLUSTER = 8  # Minimum cluster size

# Summarization
SUMMARY_MAX_LENGTH = 120 # Maximum summary length
SUMMARY_MIN_LENGTH = 40  # Minimum summary length
Model Settings
Embedding: all-mpnet-base-v2 (default)

Summarization: sshleifer/distilbart-cnn-12-6 (balanced)

Alternative Models: BART-large, T5, etc.

📊 Performance
Processing Times (Approximate)
Small documents (<50 pages): 2-5 minutes

Medium documents (50-200 pages): 5-15 minutes

Large documents (>200 pages): 15-30 minutes

Hardware Requirements
Recommended: Google Colab with GPU runtime

Minimum: 8GB RAM, multi-core CPU

Optimal: NVIDIA GPU with 8GB+ VRAM

🎓 Academic Applications
Research Use Cases
Literature review analysis

Research paper topic extraction

Document collection clustering

Content summarization for study

Educational Benefits
Automated document analysis

Quantitative topic evaluation

Structured report generation

Reproducible research methodology

🔧 Troubleshooting
Common Issues
GPU Memory Errors: Reduce MAX_DOCS parameter

Long Processing Time: Use smaller document samples

Poor Topic Quality: Adjust UMAP/HDBSCAN parameters

PDF Extraction Issues: Ensure text-based PDF (not scanned)

Solutions
Enable GPU in Colab: Runtime → Change runtime type → GPU

Clear memory: Restart runtime if needed

Check file paths: Verify Google Drive mounting
