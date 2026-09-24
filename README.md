# PySpark RDD Assignment

This repository contains a Jupyter Notebook demonstrating **Apache Spark RDD (Resilient Distributed Dataset)** concepts and operations using **PySpark**.

## 📌 Project Overview

The notebook covers practical exercises based on PySpark RDDs, including creating RDDs, applying transformations, and performing actions to process and analyze data.

The main notebook is:

- `PySparkRDD_Assignment.ipynb`

## 🛠️ Technologies Used

- Python
- Apache Spark
- PySpark
- Jupyter Notebook / Google Colab

## 📚 Topics Covered

Based on the notebook, the assignment includes practical work with:

- Creating RDDs using `parallelize()`
- Filtering records using `filter()`
- Transforming RDD data
- Working with key-value RDDs
- Applying `reduceByKey()`
- Using `collect()` to view results
- Processing employee/transaction-style datasets
- Working with tuples and nested tuple structures

## 🚀 How to Run

### Option 1: Google Colab

1. Open [Google Colab](https://colab.research.google.com/).
2. Upload `PySparkRDD_Assignment.ipynb`.
3. Install/configure PySpark if required.
4. Run the notebook cells sequentially.

### Option 2: Local Jupyter Notebook

Install the required packages:

```bash
pip install pyspark jupyter
```

Then start Jupyter:

```bash
jupyter notebook
```

Open `PySparkRDD_Assignment.ipynb` and run the cells.

## 📂 Repository Structure

```text
.
├── PySparkRDD_Assignment.ipynb
└── README.md
```

## 💡 Key PySpark RDD Concepts

### `parallelize()`

Creates an RDD from an existing Python collection.

```python
rdd = sc.parallelize(data)
```

### `filter()`

Returns only the records that satisfy a given condition.

```python
result = rdd.filter(lambda x: condition)
```

### `reduceByKey()`

Combines values belonging to the same key.

```python
result = rdd.reduceByKey(lambda x, y: x + y)
```

### `collect()`

Returns the elements of an RDD to the driver program.

```python
result.collect()
```

## 🎯 Learning Objective

The objective of this assignment is to gain hands-on experience with **PySpark RDDs**, understand common RDD transformations and actions, and practice processing structured data using Spark.

## 👤 Author

**Aditya Kumar Singh**

---

⭐ If you find this repository useful, feel free to star it!
