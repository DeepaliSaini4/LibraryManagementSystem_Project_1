

# Library Management System

"Explore this comprehensive C++ library management system that efficiently manages book lending, returning, and inventory management, providing a seamless experience for both librarians and users!"

## Dependencies for Running Locally
- CMake >= 3.5
- Make >= 4.1 (Linux, Mac), 3.81 (Windows)
- GCC/G++ >= 5.4

## Instructions for Running the Project

### Step 0: Build the Project
After completing the build process, run the executable by:
```
./library_management_system
```

### Step 1: Initialize the Library System
- The terminal will prompt: "Please set up the library system."
- Type in the total number of books (positive integer) and hit Enter.
- If successful, the terminal will inform you that the library system has been initialized and display the current inventory status.

### Step 2: Add Books to the Library
- The terminal will ask: "Please enter the number of books to add."
- Input the number of books and press Enter.
- For each book, provide details such as title, author, and ISBN when prompted.
- The terminal will confirm that the books have been added to the inventory.

### Step 3: Borrowing and Returning Books
- Users can choose to borrow or return a book. The terminal will prompt:
  - "Enter 1 to borrow a book or 2 to return a book."
- For borrowing, enter the book's ISBN, and the system will check availability.
- For returning, enter the ISBN of the borrowed book, and the system will update the status.

### Step 4: View Inventory
- Users can view the current inventory by typing:
```
view_inventory
```
- The system will display a list of all available books along with their statuses.

### Step 5 (Optional): End the Session
- Users can exit the program at any time by typing:
```
exit
```
- The system will save the current state before closing.

## Overview of Code Structure
The project utilizes Object-Oriented Design (OOD) with the main class `Library`, alongside auxiliary classes like `Book`, `User`, and `Transaction`, contained in `library.h/.cpp`, `book.h/.cpp`, and `user.h/.cpp` respectively. The main simulation logic is implemented in `library_management_system.cpp`. Here are some key methods within the `Library` class:

- **void Library::addBook(Book b)**
  - Takes a `Book` object as input and adds it to the inventory.

- **void Library::borrowBook(string isbn)**
  - Takes the book's ISBN as input and processes the borrowing request, updating availability.

- **void Library::returnBook(string isbn)**
  - Takes the ISBN of a borrowed book and processes its return, updating the inventory.

- **void Library::viewInventory()**
  - Displays the current list of books along with their borrowing statuses.

In addition, there are various auxiliary functions for printing information, handling user input, and managing data. Please refer to the source files for more details.

## Information about Rubric & Criteria

### Loops, Functions, I/O
- The project demonstrates a solid understanding of C++ functions and control structures.
- The project effectively accepts and processes user input.

### Object-Oriented Programming
- The project implements Object-Oriented Programming techniques.
- Classes use appropriate access specifiers for member variables.
- Class constructors utilize member initialization lists.
- Classes encapsulate behavior and abstract implementation details from interfaces.

### Memory Management
- The project makes use of references in function declarations.
- Resource Acquisition Is Initialization (RAII) is applied where appropriate.

### Concurrency
- (Currently, no concurrency strategies have been adopted.)

---

Feel free to adjust any sections or add more details specific to your implementation!

