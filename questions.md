# PySpark RDD Practice Questions

This file contains the questions covered in `PySparkRDD_Assignment.ipynb`.

## 1. Department-wise Salary Analysis

You are given employee data containing `employee_id`, `employee_name`, `department`, and `salary`.

Using RDD operations:
- Calculate the total salary for each department.
- Calculate the average salary for each department.
- Display only departments whose average salary is greater than ₹50,000.
- Sort the departments by average salary in descending order.

**Concepts:** `map()`, `reduceByKey()`, `mapValues()`, `filter()`, `sortBy()`

---

## 2. Customer Purchase Summary

You are given transaction data containing `transaction_id`, `customer_id`, `product`, `amount`, and `status`.

Using RDD operations:
- Filter only `"Completed"` transactions.
- Calculate the total purchase amount for each customer.
- Display the top 5 customers based on their total spending.

**Concepts:** `filter()`, `map()`, `reduceByKey()`, `sortBy()`, `take()`

---

## 3. Word Frequency Analysis

You are given an RDD containing multiple sentences.

Using RDD operations:
- Convert all words to lowercase.
- Split the sentences into individual words.
- Remove words having fewer than four characters.
- Calculate the frequency of each remaining word.
- Display the 10 most frequently occurring words.

**Concepts:** `flatMap()`, `map()`, `filter()`, `reduceByKey()`, `takeOrdered()`

---

## 4. Customer and Order Join

Create two RDDs:

**Customers**
- `customer_id`
- `customer_name`
- `city`

**Orders**
- `order_id`
- `customer_id`
- `order_amount`

Using RDD operations:
- Join the two RDDs using `customer_id`.
- Generate output containing:
  - `customer_id`
  - `customer_name`
  - `city`
  - `order_amount`
- Identify customers who have not placed any orders.

**Concepts:** Key-value RDD, `map()`, `join()`, `leftOuterJoin()`, `filter()`

---

## 5. Product-wise Sales Analysis

You are given sales data containing:

- `order_id`
- `product_name`
- `category`
- `quantity`
- `unit_price`

Using RDD operations:
- Calculate `sales_amount = quantity × unit_price`.
- Calculate the total sales amount for each product.
- Display products whose total sales exceed ₹10,000.
- Sort the products from highest to lowest sales.

**Concepts:** `map()`, `reduceByKey()`, `filter()`, `sortBy()`

---

## 6. Find the Highest-Paid Employee in Each Department

You are given employee records containing:

- `employee_id`
- `employee_name`
- `department`
- `salary`

Using RDD operations, find the employee with the highest salary in each department.

The final output should contain:

`department, employee_name, salary`

**Restriction:** Do not use DataFrames or Spark SQL.

**Concepts:** `map()`, key-value RDD, `reduceByKey()`

---

## 7. Order Status Analysis

You are given e-commerce order data containing:

- `order_id`
- `customer_id`
- `amount`
- `order_status`

Calculate the number of orders for each status, such as:

- Completed
- Cancelled
- Pending
- Returned

Then determine what percentage of the total orders belongs to each status.

Example:

```text
Completed   65%
Cancelled   15%
Pending     12%
Returned     8%
```

**Concepts:** `map()`, `reduceByKey()`, `count()`, `mapValues()`

---

## 8. Student Performance Analysis

You are given student marks containing:

- `student_id`
- `student_name`
- `subject`
- `marks`

A student can have multiple records for different subjects.

Using RDD operations:
- Calculate the average marks for each student.
- Keep only students whose average is at least 60.
- Display the results in descending order of average marks.

**Concepts:** `map()`, `reduceByKey()`, `mapValues()`, `filter()`, `sortBy()`

---

## 9. Customer Purchase Category Analysis

You are given transaction records containing:

- `transaction_id`
- `customer_id`
- `category`
- `amount`

Calculate the total amount spent by each customer in each category.

Expected result format:

```text
(101, Electronics) → 25000
(101, Grocery)     → 5000
(102, Electronics) → 18000
```

After calculating the totals, display only customer-category combinations where spending exceeds ₹10,000.

**Concepts:** Composite keys, `map()`, `reduceByKey()`, `filter()`

---

## 10. Complete E-commerce RDD Analysis

You are provided with three RDDs:

### Customers

- `customer_id`
- `customer_name`
- `city`

### Orders

- `order_id`
- `customer_id`
- `order_date`
- `status`

### Order Items

- `order_id`
- `product_name`
- `quantity`
- `unit_price`

Using only RDD operations:

1. Filter only `"Completed"` orders.
2. Calculate `item_value = quantity × unit_price`.
3. Calculate the total value of each order.
4. Join the order totals with the completed orders.
5. Join the result with customer information.
6. Calculate the total spending of each customer.
7. Keep customers whose total spending exceeds ₹10,000.
8. Sort customers by total spending in descending order.
9. Display the top 5 customers.

Produce the final output as:

```text
Customer_ID | Customer_Name | City | Total_Spending
```

**Concepts:** `filter()`, `map()`, `reduceByKey()`, `join()`, composite processing, `sortBy()`, `take()`
