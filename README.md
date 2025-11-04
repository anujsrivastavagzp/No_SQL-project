# No_SQL-project

# 🎓 Student Performance Analysis using NoSQL Database

## 🏫 Project Information
**Course:** NoSQL and DBaaS 101 (NoSQL)  
**Submitted To:** Mr. Ankit Verma  
**Submitted By:**  
- **Name:** Anuj Srivastava  
- **Section:** BCADS22  
- **Roll No:** 1240258108  

---

## 🎯 Objective
The main objective of this project is to **design, store, and analyze academic data** using a NoSQL database.  
It demonstrates how **MongoDB** can efficiently manage large, unstructured, and hierarchical data while supporting **advanced queries, aggregation, and analytics**.

---

## 🧩 Project Description
This project focuses on implementing a **NoSQL-based data model** for managing student academic records.  
Unlike traditional relational databases, NoSQL databases offer:  
- Schema flexibility  
- Faster scalability  
- Efficient handling of complex data such as arrays and subdocuments  

The project demonstrates MongoDB’s capabilities in filtering, joining, grouping, updating, and performing advanced aggregations.

---

## ⚙️ Tools & Technologies Used
- **Database:** MongoDB (NoSQL)  
- **Interface:** Mongo Shell / MongoDB Compass  
- **Optional Language:** Python / Node.js (for connection and queries)  
- **Data Source:** Student Academic Dataset (JSON / CSV)

---

## 📊 Problem Statements (Combined)

### 🧠 Problem 1: Complex Filters & Projections
#### Query 1:
List names and departments of students who have more than 85% attendance and are skilled in both *MongoDB* and *Python*.
```js
db.students_full.find(
  { attendance: { $gt: 85 }, skills: { $all: ["MongoDB", "Python"] } },
  { name: 1, department: 1 }
)
