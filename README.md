# 🪙 Gold Price Classification with Machine Learning

This project aims to classify daily gold prices into **Low**, **Medium**, or **High** categories using historical data from **2014 to 2024**.  
Machine learning models were trained and compared based on multiple evaluation metrics, and feature importance analysis was also conducted.

## 📁 Project Structure

- `gold_price_classification.ipynb` — Main notebook with the entire ML pipeline (data prep, training, evaluation, plots).
- `gold_price_classification.py` — Python script version of the notebook.
- `report.pdf` — Full project report including results, analysis, and visuals (in Turkish).
- `README.md` — Project overview.

---

## 📊 Dataset

- **Source:** [Kaggle – Daily Gold Price (2015–2024)](https://www.kaggle.com/datasets/nisargchodavadiya/daily-gold-price-20152021-time-series?resource=download)
- **Size:** 2,477 records × 7 features  
- **Features Used:**
  - `Open`, `High`, `Low`, `Volume`, `Date` (transformed into Year, Month, Day)
  - `Price` column was categorized into 3 classes using quantile-based binning (`Low`, `Medium`, `High`)

---

## ⚙️ Machine Learning Models Used

| Algorithm              | Test Accuracy | Cross-Validation Accuracy |
|------------------------|---------------|----------------------------|
| Random Forest          | **99.4%**     | **96.4%**                  |
| MLP (Neural Network)   | 99.1%         | 55.1% (overfitting)        |
| Logistic Regression    | 98.2%         | 97.6%                      |
| KNN                    | 97.3%         | 92.2%                      |
| SVM                    | 96.6%         | 89.5%                      |
| Naive Bayes            | 88.9%         | 82.2%                      |
| Decision Tree          | 98.7%         | 97.1%                      |

- **Best Model:** Random Forest with high generalization and stability
- Evaluation metrics: Accuracy, Precision, Recall, F1-Score, Confusion Matrix, Learning Curves

---

## 📈 Insights

- Clear upward trend in gold prices from 2014 to 2024.
- 2020 onward, sharp increase due to economic factors such as global inflation and the pandemic.
- Random Forest model achieved nearly perfect classification across all three categories.

---

## 🔧 Technologies & Libraries

- Python 3.10
- Scikit-learn
- Pandas, NumPy
- Matplotlib, Seaborn
- Google Colab

---

## 💡 Future Improvements

- Apply **time-series aware splitting** (e.g., train on earlier years, test on latest)
- Add more recent data (2025+)
- Explore **regression approach** instead of classification
- Use regularization and dropout to reduce overfitting in MLP

---

## 📚 Report Language

- Full academic report (`report.pdf`) is written in **Turkish** 🇹🇷

---

## 👨‍💻 Authors

- **Yusuf Kuşçu** – [LinkedIn](https://www.linkedin.com/in/yusufkuscu/)  
- **Emin Osman Toprak** [LinkedIn](https://www.linkedin.com/in/emin-osman-toprak-740730222/) 

---

## 📬 Feedback

Feel free to open issues or contact us for any questions or improvements.  
Your suggestions are always welcome!

