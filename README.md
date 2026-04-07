# Flight Delays Pipeline with PySpark and Spark SQL

A data pipeline project analyzing nearly 6 million US flight records from 2015 using PySpark and Spark SQL. Built to practice distributed data processing on a realistically large dataset.

---

## What the project does

- Loads and cleans 5.8 million flight records
- Adds new features: delay category, season, is_delayed flag
- Analyzes delay patterns by airline, season and airport using Spark SQL
- Joins flight data with airline and airport name tables
- Visualizes key findings

---

## Key findings

- Spirit Airlines had the worst delay rate: 28.8% of flights delayed
- Alaska Airlines was the best: average arrival 0.98 minutes ahead of schedule
- Winter and summer are the worst seasons (20%+ delay rate)
- Chicago O'Hare (ORD) is the worst major airport: 23.4% delay rate

---

## Technologies

- Python 3.11
- PySpark 3.5.3 + Spark SQL
- Pandas, Matplotlib
- Java 17 (required by PySpark)

---

## How to run

1. Install Java 17 from [adoptium.net](https://adoptium.net)

2. Install Python dependencies:
```bash
pip install pyspark==3.5.3 pandas matplotlib
```

3. Download `flights.csv` from [Kaggle - 2015 Flight Delays and Cancellations](https://www.kaggle.com/datasets/usdot/flight-delays) and place it in the same folder as the notebook.

4. `airlines.csv` and `airports.csv` are already included in the repository.

5. At the top of the notebook, update `JAVA_HOME` to your Java 17 installation path.

6. Run cells in order.

---

## Dataset

- **flights.csv** - 5819079 flight records (not included - download from Kaggle)
- **airlines.csv** - 14 airline codes and names (included)
- **airports.csv** - 322 airport codes and names (included)
