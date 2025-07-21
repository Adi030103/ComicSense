# ComicSense

An NLP-based system for analyzing and classifying stand-up comedy transcripts by comedian style using linguistic features, sentiment analysis, topic modeling, and machine learning models.

## Project Overview

ComicSense is a Natural Language Processing (NLP) pipeline that explores and distinguishes the unique comedic styles of 20 popular stand-up comedians. It incorporates advanced linguistic analysis, sentiment metrics, and topic modeling to classify transcripts with 92% accuracy.

## Key Features

- Text Preprocessing: Tokenization, stopword removal, lemmatization using NLTK  
- Linguistic Feature Extraction: Polarity, subjectivity, POS tagging  
- Sentiment Analysis: Using TextBlob to assess mood and intent  
- Topic Modeling: Implemented Latent Dirichlet Allocation (LDA) with Gensim for thematic analysis  
- ML Classification Models: Trained multiple scikit-learn models (Logistic Regression, SVM, Random Forest)  
- Vectorization: Used CountVectorizer to construct the Document-Term Matrix (DTM)  
- Markov Chain Text Generator: Simulates comedian-style jokes based on transition probabilities  
- Word Cloud Visualization: Showcased comedian-specific vocabulary distribution  
- Exploratory Data Analysis (EDA): Charts and metrics for better interpretability  

## Technologies Used

- Programming Language: Python  
- NLP Libraries: NLTK, TextBlob, Gensim  
- Visualization: Matplotlib, Seaborn, WordCloud  
- Machine Learning: scikit-learn  
- Topic Modeling: Gensim (LDA)  
- Text Generation: Markovify (Markov Chains)  

## Project Structure

ComicSense/  
├── data/                   # Comedy transcript dataset  
├── notebooks/              # Jupyter notebooks for EDA, modeling  
├── models/                 # Trained ML models  
├── src/                    # Source scripts (preprocessing, utils, classifiers)  
│   ├── preprocess.py  
│   ├── feature_engineering.py  
│   ├── topic_modeling.py  
│   ├── markov_generator.py  
│   └── classify.py  
├── outputs/                # Word clouds, plots, metrics  
├── requirements.txt  
└── README.md  

## Installation

1. Clone the repository:  
   git clone https://github.com/yourusername/ComicSense.git  
   cd ComicSense  

2. Create a virtual environment (optional but recommended):  
   python -m venv venv  
   source venv/bin/activate  (On Windows: venv\Scripts\activate)  

3. Install dependencies:  
   pip install -r requirements.txt  

## Usage

Run the pipeline via scripts or notebooks:

python src/preprocess.py  
python src/feature_engineering.py  
python src/topic_modeling.py  
python src/classify.py  
python src/markov_generator.py  

## Results

- Accuracy: 92% across 20 comedians  
- Top Performers: Logistic Regression, Random Forest  
- Insights:  
  - Topic distributions reveal distinct thematic preferences  
  - Subjectivity and polarity vary significantly by comedian  

## Sample Output

You can find generated word clouds and LDA visualizations in the outputs/ directory.

## Future Work

- Add BERT-based embeddings for better semantic understanding  
- Develop a Streamlit web app for real-time style classification  
- Expand dataset to include more comedians and broader diversity  

## Author

Aditya Srivastava

## License

This project is for educational purposes.
