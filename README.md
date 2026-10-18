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

SVM:

<img width="719" height="504" alt="image" src="https://github.com/user-attachments/assets/73dc3d7e-ffde-4416-adda-e38f3146608f" />
<img width="638" height="579" alt="image" src="https://github.com/user-attachments/assets/cc3592b5-0e74-4c93-8ef6-bf286ab8ed31" />





LSTM:
<img width="1074" height="722" alt="image" src="https://github.com/user-attachments/assets/6df3471a-4517-4b27-8b0c-539060a499e6" />
<img width="736" height="514" alt="image" src="https://github.com/user-attachments/assets/208cefe8-e70a-454a-8c8a-a90dbd58ee97" />
