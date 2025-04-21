Google colab link for code : https://colab.research.google.com/drive/1ME2_xR1-RoJFUUCfz3KkNiFRSul29Yp7?usp=sharing

## 📌 Steps to Run the Code

1. **Open in Google Colab**  
   Upload the `.ipynb` notebook to [Google Colab](https://colab.research.google.com/) and ensure that the runtime is set to **GPU** for faster computation.  
   *(Menu → Runtime → Change Runtime Type → Select GPU)*

2. **Upload the Dataset**  
   Upload the dataset file `Data.csv` to Colab.  
   Alternatively, download it from [Kaggle – Fed Statements and Minutes](https://www.kaggle.com/datasets/drlexus/fed-statements-and-minutes).

3. **Run All Cells**  
   Execute all the cells in the notebook sequentially. The models will process the data and generate summaries accordingly.

4. **Check the Results**  
   The file `ComparisonResults.csv` will contain the evaluation scores for each model across all data entries.

---

## 🔍 Model Comparison Summary

- **TF-IDF**  
  Best for literal extraction, but lacks contextual understanding. It may include irrelevant sentences due to relying on raw term frequency.

- **BART**  
  Generates fluent and natural summaries but tends to paraphrase heavily, risking factual drift. Not ideal when exact phrasing and decisions must be preserved.

- **BERT**  
  Provides the best summarization for Minutes of Meeting by maintaining clarity, structure, and semantic accuracy with relatively low resource usage.

---

So, prefer BERT for summarization to gain high-quality summarization with low resources.
