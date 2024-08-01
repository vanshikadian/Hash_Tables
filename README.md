# 🌟 Hash Table Project

## 📝 Overview

This project implements a hash table and a session management system using Python. The hash table is designed for efficient storage and retrieval of key-value pairs, while the session management system tracks user sessions with timestamp validation and session ID generation.

## 🚀 Features

- **Hash Table Implementation:** A custom hash table that supports insertion, deletion, and retrieval of data.
- **Session Management:** Tracks user sessions with unique session IDs and checks if a user was online within a specific timeframe.
- **Custom Hash Functions:** Implements two hash functions for efficient key distribution.
- **Timestamp Validation:** Ensures that session timestamps are in the correct format.
- **Session ID Generation:** Creates unique session IDs using a combination of username and timestamp.

## 🛠️ Classes

### `HashNode`

- **Attributes:**
  - `key`: The key associated with the node.
  - `value`: The value associated with the node.
  - `deleted`: A boolean indicating if the node has been deleted.

### `HashTable`

- **Attributes:**
  - `capacity`: The current capacity of the hash table.
  - `size`: The number of elements currently stored in the table.
  - `table`: A list of hash nodes representing the hash table.
  - `prime_index`: An index for selecting prime numbers for hash functions.

- **Methods:**
  - `_hash_1(key: str)`: Computes the hash value for a given key using the first hash function.
  - `_hash_2(key: str)`: Computes the hash value for a given key using the second hash function.

## 📂 Setup and Installation

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/your-username/hash-table-project.git
   cd hash-table-project

2. **Install Dependencies:**

    Ensure you have Python 3.x installed on your system.
    Install any additional libraries if required (e.g., datetime is part of Python's standard library).

3. **Run the Script:**

    Execute the Python script to see the hash table and session management in action.
    
    ```bash
    python solution.py

## 💡 Usage

  Here's how you can use the SessionsTable class to manage user sessions:

  ```bash
    # Create a SessionsTable instance
    sessions = SessionsTable()
    
    # Enroll a new user
    sessions.enroll_user("john_doe")
    
    # Add a session for the user
    sessions.add_session("john_doe", "12:30:00")
    
    # Check if the user was online at a specific time
    was_online = sessions.was_user_online("john_doe", "13:15:00")
    print(f"Was John Doe online at 13:15? {was_online}")
    
    # Generate a session ID for a user
    session_id = sessions.generate_session_id_wrapper("john_doe", "12:30:00")
    print(f"Session ID for John Doe: {session_id}")
```
Feel free to explore the code and modify it to suit your specific needs. Contributions and feedback are welcome!




