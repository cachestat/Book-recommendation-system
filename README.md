# Book Recommendation System

A simple book recommendation system built using collaborative filtering on the **goodbooks-10k** dataset. The project compares a popularity baseline, Item-Based Collaborative Filtering, and Matrix Factorization (SVD) to see which method produces better recommendations.

## Dataset

- Dataset: https://github.com/zygmuntz/goodbooks-10k
- Ratings from users on books (1–5)
- Filtered to active users and popular books to keep the project manageable



Run the notebooks in this order:

1. `01_eda.ipynb`
2. `02_data_cleaning.ipynb`
3. `03_model_building.ipynb`

## Models

- Popularity baseline
- Item-Based Collaborative Filtering
- Matrix Factorization (SVD)

## Results

| Model | RMSE | Precision@10 | Recall@10 |
|------|------:|-------------:|----------:|
| Popularity | 0.9673 | 0.0035 | 0.0027 |
| Item-Based CF | **0.8394** | 0.0231 | 0.0183 |
| SVD | 0.8875 | **0.1083** | **0.0854** |

Item-Based CF gave the best RMSE, while SVD produced much better recommendation quality based on Precision@10 and Recall@10.

## Tech Stack

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

## Running the Project

```bash
pip install -r requirements.txt
```

Then run the notebooks in order starting with `01_pra.ipynb`.
````
