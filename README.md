# File Management System

## Overview
**File Management System** is a Java program that simulates a basic file management system. It demonstrates object-oriented programming principles such as inheritance, polymorphism, and encapsulation. The program allows users to create, add, and display files and directories, showcasing how a file system can be modeled using Java.

---

## Features
- **File and Directory Classes**: Defines classes for files and directories with attributes like name, size, and creation date.
- **Inheritance**: Uses inheritance to extend functionality from a base class (`Mustafa_FileSystemElement`) to derived classes (`File` and `Directory`).
- **Polymorphism**: Demonstrates polymorphism by overriding the `displayDetails` method in derived classes.
- **Encapsulation**: Encapsulates attributes and provides methods to interact with them.
- **User Interaction**: Collects user information and displays a welcome message.

---

## How It Works
1. **Base Class**: `Mustafa_FileSystemElement` serves as the base class with common attributes like name, size, and creation date.
2. **File Class**: Represents a file with an additional attribute for the file extension.
3. **Directory Class**: Represents a directory that can contain files and subdirectories. It includes methods to add files and display directory contents.
4. **Main Function**: Collects user information, creates instances of files and directories, and displays their details.

---

## Usage
1. **Run the Program**: Execute the `File_Management_System` class.
2. **User Input**: Enter your name, major, and favorite programming language when prompted.
3. **Output**: The program displays a welcome message and details of the created files and directory.

---

## Code Structure
- **Base Class**: `Mustafa_FileSystemElement`
  - Attributes: `Fname`, `Fsize`, `createdDate`
  - Methods: `getSize`, `setSize`, `displayDetails`
- **File Class**: `File`
  - Additional Attribute: `Fextension`
  - Methods: Overrides `displayDetails` to include file extension.
- **Directory Class**: `Directory`
  - Attribute: `contents` (list of file system elements)
  - Methods: `addFile`, `displayDetails` (overrides base class method)
- **Main Class**: `File_Management_System`
  - Collects user input and demonstrates file and directory operations.

---

## Example Output

```
Enter your name: Khaled
Enter your major: Computer Science
Enter your favorite programming language: Java

| Welcome, Mr. Mustafa
| You are studying Computer Science at Yarmouk University
| Your favorite programming language is Java
---> Directory Details:

Name : My_Folder
Size : 7168 KB
Created Date : 2024-05-12
Type: Directory

---> Contents of Directory:

Name : Khaled.txt
Size : 2048 KB
Created Date : 2024-05-12
Type: File
Extension : txt

Name : Mohammad_Majdalawy.pdf
Size : 1024 KB
Created Date : 2024-05-12
Type: File
Extension : pdf

Name : Yarmouk_University.doc
Size : 4096 KB
Created Date : 2024-05-12
Type: File
Extension : doc
```
