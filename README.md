# GitHub-like Repository Management System

This is a comprehensive Data Structures project built in C++ that simulates a mini version control and social network system similar to GitHub.

## Features

*   **User Management**: Implements user registration and login functionality. User data is stored and managed using **Hash Tables** for efficient searching and retrieval.
*   **Repository Management**: Users can create multiple repositories, add files to them, and delete files. The file structure within each repository is managed using an **AVL Tree** to ensure balanced and efficient file operations.
*   **Commit System**: Users can commit their repositories, saving their state.
*   **Social Network (Friends/Followers)**: Users can add friends, unfollow friends, and view their friend list. This feature is implemented using **Graphs** (Adjacency List representation) to model the connections between users.

## Data Structures Used

1.  **Hash Tables**: For O(1) average time complexity user lookups during login, registration, and friend search.
2.  **AVL Trees**: A self-balancing Binary Search Tree used to store files within a repository, ensuring O(log n) time complexity for adding, deleting, and searching files.
3.  **Graphs (Adjacency List)**: To represent the network of friends, allowing efficient traversal and management of followers/followings.
4.  **Linked Lists**: Used internally within Hash Table collision resolution (chaining) and Graph Adjacency Lists.

## How to Run

1. Compile the C++ source files (`main.cpp`, `function.cpp`). You can use any standard C++ compiler like `g++` or use the provided Visual Studio project file (`changing.vcxproj`).
2. Run the executable.
3. Use the interactive console menu to register, login, create repositories, and add friends.

## File Structure

*   `main.cpp`: Contains the main menu loop and user interface.
*   `class.h`: Header file containing definitions for all classes and data structures (`User`, `HashTable`, `Node`, `AVLTree`, `Repository`, `FriendNode`, `Friends`, `UserManagement`).
*   `function.cpp`: Contains the implementation of the methods defined in `class.h`.
*   `.txt` and `.csv` files: Used as local file-based databases to persist user data, repositories, and relationships across sessions.
