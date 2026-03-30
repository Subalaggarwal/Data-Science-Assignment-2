# Movie Data Analysis Project

## Overview

This project is based on analyzing a dataset of around **3000 movies**.
The goal is to explore the data and find useful insights like profit, ROI, top actors, producers, etc.

This project is done using **Python (Pandas)**.

---

## Dataset

The dataset contains information like:

* Movie title
* Budget
* Revenue
* Cast
* Crew
* Genres
* Language , etc.

---

## Tools & Libraries Used

* Google Colab
* Python
* Pandas
* NumPy
* AST (for parsing JSON-like data)

---

## Data Preprocessing

Some columns like `cast` and `crew` were in string format, so:

* Converted them using `ast.literal_eval()`
* Extracted:

  * Actors from `cast`
  * Director from `crew`
  * Producers from `crew`

Also:

* Removed rows where budget = 0
* Calculated:

  * **Profit = Revenue - Budget**
  * **ROI = (Profit / Budget) * 100**

---

## Questions Solved

### 1. Highest Profit Movie

* Found the movie with maximum profit
* Displayed its director, actors, and producers

---

### 2. Language with Highest ROI

* Grouped data by language
* Calculated average ROI

---

### 3. Unique Genres

* Extracted all genres
* Found unique values

---

### 4. Top 3 Producers by ROI

* Used `explode()` to separate producers
* Calculated average ROI per producer
* Selected top 3

---

### 5. Actor with Most Movies

* Counted frequency of actors
* Found actor with highest appearances
* Analyzed their movies and profits

---

### 6. Top Directors & Their Favorite Actors

* Found top 3 directors
* Checked which actors they work with most

---


## How to Run

1. Install required libraries:

```
pip install pandas numpy
```

2. Run the Python file:

```
python your_file_name.py
```

---

## Conclusion

* Data analysis helps in identifying profitable trends
* ROI is important for decision making
* Certain actors and producers consistently perform well

---

## Author

**Subal Aggarwal**

