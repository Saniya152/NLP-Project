# NLP-Based Sentiment Analysis of Customer Reviews

## Pipeline
Raw Review Text -> Preprocessing -> TF-IDF -> Classification Model -> Evaluation

## Results
| Model | Accuracy | Precision | Recall | F1-score |
|---|---|---|---|---|
| Naive Bayes | 0.876 | 0.867 | 0.888 | 0.877 |
| Logistic Regression | 0.878 | 0.899 | 0.852 | 0.875 |

## Project Structure
```
NLP-Project/
├── README.md
├── source_code.py       # full pipeline: preprocessing, TF-IDF, model, evaluation
├── dataset/              # product reviews CSV (review, rating)
├── screenshots/          # confusion matrix, output screenshots
├── report/               # full project report (report.docx)
└── requirements.txt
```

## How to Run
```bash
pip install -r requirements.txt
python source_code.py
```

## Dataset
Flipkart-style e-commerce product reviews (`review`, `rating` 1-5).
Ratings 4-5 mapped to "positive", 1-2 to "negative"; 3-star (neutral)
rows dropped. Classes balanced via undersampling before training.
