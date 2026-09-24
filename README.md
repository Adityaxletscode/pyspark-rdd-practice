# PySpark RDD Practice

A hands-on PySpark practice repository covering **RDD creation, transformations, actions, key-value RDDs, filtering, aggregation, joins, and data processing using Apache Spark**.

## 📌 Project Overview

This repository contains a Jupyter Notebook with practical PySpark RDD problems and their solutions. It is designed to build a strong understanding of how RDDs can be used to process structured and unstructured data.

## 📂 Repository Contents

```text
pyspark-rdd-practice/
├── PySparkRDD_Assignment.ipynb
├── questions.md
└── README.md
```

### `PySparkRDD_Assignment.ipynb`

Contains the PySpark code, datasets, RDD operations, and solutions to the practice questions.

### `questions.md`

Contains the **10 PySpark RDD practice questions** covered in the notebook. The questions cover topics such as:

- Department-wise salary analysis
- Customer purchase analysis
- Word frequency analysis
- Customer and order joins
- Product-wise sales analysis
- Highest-paid employee by department
- Order status analysis
- Student performance analysis
- Customer-category spending analysis
- Complete e-commerce RDD analysis

Keeping the questions in a separate file makes it easy to review or practice the problems independently before checking the notebook solutions.

## 🛠️ Technologies Used

- Python
- Apache Spark
- PySpark
- Jupyter Notebook / Google Colab

## 📚 PySpark Concepts Covered

The repository provides practical examples of:

- Creating RDDs using `parallelize()`
- `map()`
- `filter()`
- `flatMap()`
- `reduceByKey()`
- `mapValues()`
- `join()`
- `leftOuterJoin()`
- `sortBy()`
- `take()`
- `takeOrdered()`
- Key-value RDDs
- Composite keys
- Aggregation and data analysis

## 🚀 How to Run

### Google Colab

1. Open Google Colab.
2. Upload `PySparkRDD_Assignment.ipynb`.
3. Install/configure PySpark if required.
4. Run the notebook cells sequentially.

### Local Jupyter Notebook

Install PySpark and Jupyter:

```bash
pip install pyspark jupyter
```

Start Jupyter:

```bash
jupyter notebook
```

Then open:

```text
PySparkRDD_Assignment.ipynb
```

## 🎯 Learning Objectives

By working through this repository, you can practice:

- Understanding the fundamentals of RDDs
- Creating and manipulating RDDs
- Applying transformations and actions
- Working with key-value RDDs
- Performing aggregations with `reduceByKey()`
- Joining multiple RDDs
- Filtering and sorting data
- Solving real-world data-processing problems with PySpark

## 📝 Practice Workflow

A recommended way to use this repository:

1. Read a question from `questions.md`.
2. Try solving it independently using PySpark RDDs.
3. Open `PySparkRDD_Assignment.ipynb`.
4. Compare your solution with the notebook.
5. Experiment with different datasets and RDD transformations.

## 👤 Author

**Aditya Kumar Singh**

⭐ If you find this repository useful, feel free to star it!
