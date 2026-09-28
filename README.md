# 📱 Mobile Shop CRUD Project

A simple **console-based Mobile Shop Management System** built with **Python**.
The project demonstrates the basic **CRUD operations** — Create, Read, Update, and Delete — using a Python list for in-memory data storage.

## 📌 Project Overview

This application allows a user to manage mobile phone records through an interactive menu-driven dashboard.

Each mobile record is stored in the following format:

```text
[id, brand, model, price, quantity]
```

Example:

```python
[101, "Samsung", "Galaxy A55", 35000, 5]
```

## ✨ Features

| Option | Feature             | Description                                                        |
| ------ | ------------------- | ------------------------------------------------------------------ |
| 1      | Add Mobile          | Add a new mobile record                                            |
| 2      | Display All Mobiles | View all stored mobile records in a formatted table                |
| 3      | Search Mobile       | Search for a mobile using its ID                                   |
| 4      | Update Mobile       | Update the brand, model, price, and quantity of an existing mobile |
| 5      | Delete Mobile       | Delete a mobile record after confirmation                          |
| 6      | Exit                | Close the application                                              |

### Additional Validation

* Prevents duplicate Mobile IDs when adding a record.
* Displays a message when no mobile records are available.
* Confirms deletion before removing a record.
* Handles invalid menu selections with an error message.

## 🛠️ Technologies Used

* **Python**
* **Jupyter Notebook**
* Python **list** for data storage
* `match-case` for menu selection
* Functions for modular program design

> **Note:** The project uses `match-case`, so **Python 3.10 or later** is recommended.

## 🧩 CRUD Operations

The project demonstrates the four core database-style operations:

### Create

`add_mobile()` adds a new mobile record to the `mobiles` list.

### Read

`display_mobiles()` displays all available records, while `search_mobile()` retrieves a specific mobile using its ID.

### Update

`update_mobile()` modifies the details of an existing mobile record.

### Delete

`delete_mobile()` removes a mobile record after user confirmation.

## 📂 Project Structure

```text
Mobile-Shop-CRUD/
│
├── Mobile_Shop.ipynb
└── README.md
```

## ▶️ How to Run

### Using Jupyter Notebook

1. Clone or download this repository.
2. Open `Mobile_Shop.ipynb`.
3. Run the cells containing the function definitions.
4. Run the final cell containing:

```python
dashboard()
```

5. Use the displayed menu to manage mobile records.

### Using Python Script

The notebook can also be converted to a `.py` file and run from a Python environment that supports `match-case`.

## 💻 Example Menu

```text
=============================================
        MOBILE SHOP MANAGEMENT
=============================================
1. Add Mobile
2. Display All Mobiles
3. Search Mobile
4. Update Mobile
5. Delete Mobile
6. Exit
=============================================
Enter your choice:
```

## 📊 Sample Record

```text
ID      Brand          Model               Price          Quantity
---------------------------------------------------------------------------
101     Samsung        Galaxy A55          35000.00       5
103     Asus           ROG 3               80000.00       5
```

## 🎯 Learning Objectives

This project is useful for practicing:

* Python functions
* Lists and list manipulation
* `for` loops
* Conditional statements
* User input and output
* CRUD concepts
* Menu-driven programming
* Basic input validation
* `match-case` statements
* Modular programming

## ⚠️ Data Storage

The application stores all mobile information in a Python list:

```python
mobiles = []
```

Because the data is stored **in memory**, records are lost when the program ends. No external database or file-based persistence is used in the current version.

## 🚀 Possible Future Enhancements

The current project can be extended by:

* Adding file-based storage using CSV or JSON
* Connecting the application to MySQL or another database
* Adding stronger input validation
* Supporting search by brand or model
* Adding stock and sales management
* Creating a graphical or web-based interface
* Adding login and user roles
