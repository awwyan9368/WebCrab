# WebCrab
# TMDB Movies Exploratory Data Analysis

This project performs an **Exploratory Data Analysis (EDA)** on the [TMDB 5000 Movies dataset](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata), which contains metadata on thousands of movies, including their cast, crew, genres, budget, and revenue.


## Project Objectives

- Load and clean the TMDB dataset using **Pandas**.
- Explore trends and answer key questions using **data visualization**.
- Create a clear, reproducible analysis in a single Jupyter Notebook.


## Files Included

| File | Description |
|------|--------------|
| `tmdb_analysis.ipynb` | Main Jupyter Notebook with full analysis and visualizations |
| `tmdb_5000_movies.csv` | Movies dataset |
| `tmdb_5000_credits.csv` | Cast and crew dataset |
| `README.md` | Project documentation (this file) |


## Technology Stack

- **Language:** Python  
- **Libraries:**  
  - `pandas` – data manipulation  
  - `numpy` – numerical computations  
  - `matplotlib` & `seaborn` – visualization  
- **Environment:** Jupyter Notebook  


## Key Analyses

The notebook answers the following questions using visualizations:

1. **Which genres are the most common?**  
   → Bar chart of top genres by movie count  

2. **Who are the top 10 highest-grossing directors?**  
   → Horizontal bar chart based on total revenue  

3. **Is there a correlation between a movie's budget and its revenue?**  
   → Log–log scatter plot with Pearson correlation coefficient  

4. **What is the average movie runtime, and has it changed over the years?**  
   → Line chart showing average runtime by release year  

5. **Which production companies have produced the most high-revenue films?**  
   → Bar chart of top companies in the 75th percentile of revenues  

*(Bonus: Frequent keywords in movie overviews.)*


## Data Cleaning Steps

- Parsed JSON-formatted columns (`genres`, `production_companies`, `keywords`, `cast`, `crew`).
- Merged `movies` and `credits` datasets on `id` / `movie_id`.
- Handled missing values and corrected data types.
- Replaced zero budgets/revenues with `NaN` for accurate analysis.


## How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/<your-username>/tmdb-movie-eda.git
   cd tmdb-movie-eda
   ```

2. Open the notebook:
   ```bash
   jupyter notebook tmdb_analysis.ipynb
   ```

3. Run all cells in order to reproduce the analysis.


## Results Summary

- **Top Genres:** Drama, Comedy, Thriller, Action dominate the dataset.  
- **Top Directors:** James Cameron, Christopher Nolan, Steven Spielberg lead by total box-office revenue.  
- **Budget–Revenue Correlation:** Strong positive correlation observed (Pearson r ≈ 0.75+).  
- **Runtime Trend:** Slight decline in average runtime over recent decades.  
- **Production Leaders:** Warner Bros., Universal Pictures, Paramount consistently top high-revenue productions.


## Author

**Ayan Muhammad**  
 [awwyan9368@gmail.com]  
 [https://www.linkedin.com/in/ayan-muhammad-b4bb85360]


## License

This project is for educational purposes. Dataset © TMDB / Kaggle.
