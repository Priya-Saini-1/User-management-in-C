# User Management System

## Overview

The **User Management System** is a console-based application developed in C that allows users to register and log in. It includes functionalities to input and verify credentials while ensuring a smooth user experience. It is suitable for basic user management in small projects.

## Features
- **Registration:** Users can register by providing a username and password.
- **Login:** Users can log in with registered credentials.
- **Password Masking:** Passwords are input securely with masking enabled.
- **Multi-platform Support:** Designed to run on Windows and UNIX/Linux systems.
- **Max Users:** Supports up to 10 users.

## Code Description

### File: `main.c`
The primary functionality includes:
- **Main Menu:** A simple interactive menu with options to Register, Login, and Exit.
- **User Storage:** Keeps track of registered users using a `User` struct.
- **Input Handling:** Functions to input and verify credentials (`input_credentials`, `fix_fgets_input`).
- **Cross-platform Password Input:** Handles masked password input differently for Windows and UNIX/Linux systems.

## How to Run

1. **Prerequisites:**
   - Install a C compiler (e.g., GCC or MinGW for Windows).
   - Clone or download this repository to your local machine.

2. **Build Instructions:**
   - Open a terminal or command prompt and navigate to the project folder.
   - Run the following command:
     ```bash
     gcc main.c -o UserManagementSystem
     ```
     This creates an executable named `UserManagementSystem`.

3. **Execution:**
   - Run the executable:
     ```bash
     ./UserManagementSystem
     ```
   - Follow the on-screen menu.

## Limitations

- The number of users is limited to 10.
- This program does not store user data persistently (data is lost on exit).

## Future Improvements

Ideas for potential enhancement:
- Implement persistent storage for user credentials (e.g., using files or a database).
- Allow dynamic user capacity with memory allocation.
- Add features like password recovery and user deletion.

## License

This project is open-source under the [MIT License](LICENSE). Feel free to use and modify it as needed.
