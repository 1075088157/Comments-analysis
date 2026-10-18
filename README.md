# Comments Analysis (Movie Review Sentiment Analysis)

A Natural Language Processing (NLP) project that classifies movie reviews into **Positive**, **Neutral**, or **Negative** categories. It compares traditional machine learning and deep learning models.

## 🛠 Tech Stack
- **Languages & Tools:** Python, Jupyter Notebook
- **Machine Learning:** scikit-learn (SVM), TF-IDF
- **Deep Learning:** TensorFlow/Keras (LSTM), PyTorch, Hugging Face Transformers (BERT)
- **Data Processing & Visualization:** Pandas, NumPy, Matplotlib

## ✨ Core Features
- Text preprocessing: tokenization, stopword removal, vectorization.
- Three different approaches for comparison:
  - **SVM** with TF-IDF features.
  - **LSTM** with BERT sentence embeddings.
  - **BERT**-based text representation generation.
- Model evaluation using classification report, ROC curve, and confusion matrix.

## 📊 Model Performance
- **SVM:** Achieved around **71%** accuracy.
- **LSTM:** Achieved around **63%** accuracy.

## ⚠️ Important Note on Large Files
Due to GitHub's file size limits (100MB), the following large files are **NOT included** in this repository:
1. `imdb_sup.csv` (The raw dataset, ~62MB)
2. `bert_rep.npz` & `tfidf_data.npz` (Generated feature files, ~600MB)
3. `bert/pytorch_model.bin` (BERT model weights, ~392MB)

**How to reproduce:**
1. Place your own `imdb_sup.csv` (with `Review` and `Rating` columns) in the root directory.
2. Run `Bert Text Representation Generation.ipynb` and `SVM Text Representation Generation.ipynb` to generate the `.npz` feature files.
3. The `bert/pytorch_model.bin` can be automatically downloaded by Hugging Face Transformers, or you can place the weights in the `bert/` folder manually.

## 🚀 How to Run
1. Install the required dependencies:
   ```bash
   pip install pandas numpy scikit-learn tensorflow torch transformers matplotlib tqdm
