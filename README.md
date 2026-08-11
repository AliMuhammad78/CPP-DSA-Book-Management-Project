
 <p align="center"> <img src="https://img.shields.io/badge/Language-C%2B%2B-blue?style=for-the-badge&logo=cplusplus" alt="C++"> <img src="https://img.shields.io/badge/Project-DSA-orange?style=for-the-badge" alt="DSA"> <img src="https://img.shields.io/badge/University-Project-purple?style=for-the-badge" alt="University Project"> <img src="https://img.shields.io/badge/Platform-Windows-lightgrey?style=for-the-badge&logo=windows" alt="Windows"> </p>

<h1 align="center">📚 Old Book Corner</h1>

<p align="center"> <b>A Console-Based Book Management & Exchange System in C++</b> </p>

<p align="center"> <i>A university Data Structures & Algorithms project demonstrating the practical use of fundamental data structures through a real-world book management system.</i> </p>

 

## ✨ Overview

**Old Book Corner** is a console-based **Book Management System** developed as a university **Data Structures & Algorithms (DSA)** project.

The project simulates a small second-hand book marketplace where users can manage their books and perform different operations such as:

* 📖 Adding books
* 🔍 Searching for books
* 👀 Viewing available books
* 🛒 Buying books
* 💰 Selling books
* 🔄 Exchanging books
* 🛠️ Updating book information
* 🗑️ Removing books

The project focuses on implementing fundamental **data structures, pointers, dynamic memory allocation, searching, and object-oriented programming concepts** in C++.

---

## 🎯 Project Objective

The main objective of this project is to demonstrate practical understanding of **Data Structures and Algorithms** by implementing a real-world inspired book management application.

Instead of relying entirely on built-in containers, the project uses a **singly linked list** to manage book records and a **stack** to handle menu navigation.

This project was created as part of a university-level DSA course/project.

---

## 🖥️ Main Features

### 👨‍💼 Admin Menu

The Admin section allows management of the book collection.

| Feature           | Description                          |
| ----------------- | ------------------------------------ |
| ➕ Add Book        | Add a new book to the collection     |
| 🗑️ Remove Book   | Remove a book using its ID           |
| ✏️ Update Book    | Modify book title, author, and price |
| 📚 View All Books | Display all available books          |
| ↩️ Back           | Return to the main menu              |

---

### 👤 User Menu

Users can interact with the available books.

| Feature           | Description                    |
| ----------------- | ------------------------------ |
| ➕ Add Book        | Add a book to the collection   |
| 🔍 Search Books   | Search books by title          |
| 📚 View All Books | Display available books        |
| 🛒 Buy Book       | Purchase an available book     |
| 💰 Sell Book      | Sell a book                    |
| 🔄 Exchange Book  | Exchange a book based on price |
| ↩️ Back           | Return to the main menu        |

---

## 🧠 Data Structures Used

One of the main goals of this project is to demonstrate the practical implementation of different data structures.

### 🔗 Singly Linked List

The main book collection is implemented using a **singly linked list**.

Each book is represented by a `Book` node containing:

```text
+---------+----------------+----------------+-------+------+
|   ID    |     Title      |     Author     | Price | Next |
+---------+----------------+----------------+-------+------+
```

Each node points to the next book in the collection.

This allows the program to dynamically add, remove, update, and traverse books.

---

### 📚 Stack

A C++ `stack<string>` is used for menu navigation.

```cpp
stack<string> bookstack;
```

The stack stores menu states and uses operations such as:

* `push()`
* `pop()`

This demonstrates the **LIFO (Last In, First Out)** principle.

---

### 📦 Vector

A `vector<Book>` is also maintained to keep track of the books added to the system.

```cpp
vector<Book> bookArray;
```

The vector is particularly used for maintaining the count of available books.

---

## 🏗️ Object-Oriented Programming

The project also demonstrates fundamental **OOP concepts**.

### `Book` Structure

The `Book` structure represents an individual book.

```cpp
struct Book {
    int id;
    string title;
    string author;
    double price;
    Book* next;
};
```

### `BookManager` Class

The `BookManager` class handles the major operations performed on books.

```cpp
class BookManager {
private:
    Book* head;
    vector<Book> bookArray;

public:
    // Book management functions
};
```

The class provides functions for:

* Adding books
* Removing books
* Updating books
* Searching books
* Displaying books
* Buying books
* Selling books
* Exchanging books

---

## 🔎 Searching

The system provides title-based book searching.

The program traverses the linked list and uses C++ string searching:

```cpp
current->title.find(title)
```

This allows the user to find books whose titles contain the entered search text.

---

## 🧩 Project Structure

```text
Old-Book-Corner/
│
├── 📄 main project.cpp
├── 📄 DSA project proposel.docx
└── 📄 README.md
```

### File Description

| File                        | Purpose                              |
| --------------------------- | ------------------------------------ |
| `main project.cpp`          | Main C++ source code                 |
| `DSA project proposel.docx` | Original university project proposal |
| `README.md`                 | Project documentation                |

> `.vscode/` contains Visual Studio Code configuration files and can safely be excluded if you want the repository to contain only the actual project files.

---

## 🛠️ Technologies Used

* 💻 **C++**
* 🧠 **Data Structures & Algorithms**
* 🏗️ **Object-Oriented Programming**
* 🔗 **Singly Linked List**
* 📚 **Stack**
* 📦 **Vector**
* 👉 **Pointers**
* 🧮 **Dynamic Memory Allocation**
* 🪟 **Windows Console API**

### Standard Libraries

```cpp
#include <iostream>
#include <string>
#include <stack>
#include <sstream>
#include <vector>
```

### Windows-Specific Libraries

```cpp
#include <conio.h>
#include <windows.h>
```

These libraries provide functionality such as:

* `_getch()`
* `Sleep()`
* Windows console interaction

---

## ⚙️ Requirements

To run this project, you need:

* 🪟 Windows OS
* 🔧 A C++ compiler such as **G++ / MinGW**
* 💻 Visual Studio, Code::Blocks, Dev-C++, or VS Code with a C++ compiler

Because the project uses Windows-specific libraries such as `windows.h` and `conio.h`, **Windows is recommended**.

---

## 🚀 How to Run

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/old-book-corner.git
```

### 2️⃣ Open the Project

Open:

```text
main project.cpp
```

in your preferred C++ IDE.

### 3️⃣ Compile

Using MinGW/G++:

```bash
g++ "main project.cpp" -o OldBookCorner
```

### 4️⃣ Run

```bash
OldBookCorner
```

---

## 🖼️ Program Flow

```text
                    📚 OLD BOOK CORNER
                           │
                           ▼
                    🏠 MAIN MENU
                     /     |     \
                    /      |      \
                   ▼       ▼       ▼
              👨‍💼 Admin   👤 User   🚪 Exit
                 │          │
       ┌─────────┼──────┐   ├───────────────┐
       │         │      │   │       │       │
       ▼         ▼      ▼   ▼       ▼       ▼
     ➕ Add    🗑️ Remove ✏️ Update 🔍 Search 🛒 Buy
       │         │      │   │       │       │
       └─────────┴──────┘   └───┬───┴───────┘
                                │
                         📚 Book Collection
                                │
                                ▼
                         🔗 Linked List
```

---

## 💡 DSA Concepts Demonstrated

This project demonstrates several important concepts studied in DSA:

```text
                 📚 Old Book Corner
                         │
        ┌────────────────┼────────────────┐
        │                │                │
        ▼                ▼                ▼
 🔗 Linked List       📚 Stack         📦 Vector
        │                │                │
        ▼                ▼                ▼
 Book Management    Menu Navigation   Book Tracking
        │
        ▼
 🔍 Traversal & Searching
        │
        ▼
 ➕ Insert | 🗑️ Delete | ✏️ Update
```

---

## 📊 Core Operations

### ➕ Insertion

New books are inserted at the beginning of the linked list.

```cpp
newBook->next = head;
head = newBook;
```

**Time Complexity:** `O(1)`

---

### 🔍 Searching

The linked list is traversed to find a matching book.

**Time Complexity:** `O(n)`

---

### 🗑️ Deletion

A book is located using its ID and then removed from the linked list.

**Time Complexity:** `O(n)`

---

### ✏️ Updating

The linked list is traversed until the requested book ID is found.

**Time Complexity:** `O(n)`

---

### 👀 Display

Every node is traversed and displayed.

**Time Complexity:** `O(n)`

---

## 🎓 Learning Outcomes

Through this project, the following concepts were practiced:

* ✅ Understanding linked lists
* ✅ Creating and manipulating nodes
* ✅ Working with pointers
* ✅ Dynamic memory allocation
* ✅ Implementing insertion and deletion
* ✅ Traversing data structures
* ✅ Searching data
* ✅ Using stacks
* ✅ Using vectors
* ✅ Applying OOP concepts
* ✅ Creating classes and structures
* ✅ Handling invalid input
* ✅ Building a menu-driven application
* ✅ Designing a real-world DSA application

---

## ⚠️ Current Limitations

This is a university-level console project, so there are some limitations:

* 💾 Books are stored only in memory.
* 🔄 Data is lost when the program exits.
* 🪟 The application is designed primarily for Windows.
* 🔐 There is no real authentication system.
* 💳 There is no actual payment processing.
* 🗄️ No database is currently connected.
* 📦 Book inventory persistence is not implemented.

These limitations also provide opportunities for future development.

---

## 🔮 Future Improvements

The project can be expanded into a much more complete application by adding:

* 💾 File handling for permanent book storage
* 🗄️ Database integration
* 🔐 Admin/user authentication
* 👤 User profiles
* ❤️ Wishlist functionality
* ⭐ Book ratings and reviews
* 🏷️ Book categories
* 🔍 Advanced filtering and sorting
* 📊 Inventory statistics
* 💰 Transaction history
* 🧾 Purchase receipts
* 🌐 Web-based interface
* 🖥️ Graphical User Interface
* 📱 Mobile application
* 🔌 REST API integration

---

## 📸 Application Preview

> Add screenshots of your program here to make the repository more attractive.

Example:

```text
📸 Main Menu
📸 Admin Menu
📸 User Menu
📸 Book Search
📸 Book Purchase
📸 Book Exchange
```

You can later add them like:

```markdown
![Main Menu](screenshots/main-menu.png)
![User Menu](screenshots/user-menu.png)
```

---

## 👨‍💻 Author

### **Muhammad Ali Saagar**

🎓 **BS Computer Science — Section BSCS-C**

📌 **University DSA Project**

This project was developed as part of a university course to demonstrate practical implementation of **Data Structures and Algorithms using C++**.

---

## 📚 Academic Topics

This project is relevant to the following university subjects/topics:

* **Data Structures & Algorithms**
* **Object-Oriented Programming**
* **Programming Fundamentals**
* **C++ Programming**
* **Memory Management**
* **Algorithm Analysis**
* **Problem Solving**

---

## ⭐ Project Highlights

```text
🔗 Singly Linked List
📚 Stack
📦 Vector
👉 Pointers
🏗️ OOP
🔍 Searching
➕ Insertion
🗑️ Deletion
✏️ Updating
🛒 Buying
💰 Selling
🔄 Book Exchange
🪟 Windows Console UI
```

---

## 📜 License

This project was created for **educational and academic purposes**.

You are welcome to study, modify, and improve the project.

---

<div align="center">

### 📚 Old Book Corner

**Buy • Sell • Search • Exchange • Manage**

Made with ❤️ and C++

⭐ **If you find this project useful, consider giving it a star!** ⭐

</div>
