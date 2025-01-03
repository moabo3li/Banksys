# **Bank-System Documentation**

## **Table of Contents**
1. [Introduction](#introduction)
2. [Features](#features)
3. [Technologies Used](#technologies-used)
4. [Project Structure](#project-structure)
5. [Classes and Their Functionality](#classes-and-their-functionality)
6. [File Descriptions](#file-descriptions)
7. [How to Run the Project](#how-to-run-the-project)
8. [Usage](#usage)


---

## **Introduction**
The **Bank-System** is a console-based banking application designed to simulate basic banking operations. It allows users to manage clients, perform transactions (deposit, withdraw, transfer), and manage user permissions. The system is built using C++ and follows an object-oriented programming (OOP) approach.

---

## **Features**
- **Client Management**:
  - Add, update, delete, and find clients.
  - View a list of all clients.
- **Transactions**:
  - Deposit funds into a client's account.
  - Withdraw funds from a client's account.
  - Transfer funds between clients.
  - View transaction logs.
- **User Management**:
  - Add, update, delete, and find users.
  - Manage user permissions (e.g., access to client lists, transactions, etc.).
- **Login System**:
  - Secure login with username and password.
  - Track login history.
- **Permissions**:
  - Different levels of access for users (e.g., admin, regular user).

---

## **Technologies Used**
- **Programming Language**: C++
- **Libraries**: Standard C++ libraries (`<iostream>`, `<string>`, `<vector>`, `<fstream>`, etc.)
- **Tools**: Visual Studio (as indicated by `.vcxproj` files)

---

## **Project Structure**
The project is organized into multiple header files (`.h`) and source files (`.cpp`). Below is the structure:
```
Bank-System
    ├── clsAddNewClientScreen.h
    ├── clsAddNewUserScreen.h
    ├── clsbankclients.h
    ├── clsClientListScreen.h
    ├── clsDate.h
    ├── clsDeleteClientScreen.h
    ├── clsDeleteUserScreen.h
    ├── clsDepositScreen.h
    ├── clsFindClientScreen.h
    ├── clsFindUserScreen.h
    ├── clsInputValidate.h
    ├── clsListUsersScreen.h
    ├── clsLoginRegisterScreen.h
    ├── clsLoginScreen.h
    ├── clsMainScreen.h
    ├── clsManageUsersScreen.h
    ├── clsperson.h
    ├── clsScreen.h
    ├── clsstring.h
    ├── clsTotalBalancesScreen.h
    ├── clsTransactionsScreen.h
    ├── clsTransferLogScreen.h
    ├── clsTransferScreen.h
    ├── clsUpdateClientScreen.h
    ├── clsUpdateUserScreen.h
    ├── clsUser.h
    ├── clsutil.h
    ├── Global.h
    ├── LoginRegister.txt
    ├── opplib.cpp
    ├── opplib.vcxproj
    ├── opplib.vcxproj.filters
    ├── Users.txt
    └── Clients.txt
```


---

## **Classes and Their Functionality**
The project is built around several classes, each responsible for specific functionality:

1. **`clsPerson`**:
   - Base class for `clsUser` and `clsBankClient`.
   - Contains basic person details (first name, last name, email, phone).

2. **`clsUser`**:
   - Manages user-related operations (login, permissions, etc.).
   - Inherits from `clsPerson`.

3. **`clsBankClient`**:
   - Manages client-related operations (account management, transactions).
   - Inherits from `clsPerson`.

4. **`clsScreen`**:
   - Base class for all screen-related operations.
   - Provides methods for drawing headers and checking access permissions.

5. **`clsUtil`**:
   - Utility class for common operations (e.g., random number generation, encryption).

6. **`clsInputValidate`**:
   - Validates user input (e.g., numbers, dates).

7. **`clsDate`**:
   - Handles date-related operations (e.g., date formatting, calculations).

8. **`clsString`**:
   - Provides string manipulation utilities (e.g., splitting, trimming).

9. **Transaction Screens**:
   - `clsDepositScreen`, `clsWithdrawScreen`, `clsTransferScreen`, etc.
   - Handle specific transaction operations.

10. **Management Screens**:
    - `clsManageUsersScreen`, `clsClientListScreen`, etc.
    - Handle user and client management.

---

## **File Descriptions**
Below is a brief description of the key files in the project:

1. **`clsbankclients.h`**:
   - Manages client data and operations (e.g., deposit, withdraw, transfer).

2. **`clsUser.h`**:
   - Manages user data and operations (e.g., login, permissions).

3. **`clsScreen.h`**:
   - Provides base functionality for all screens (e.g., headers, access control).

4. **`clsMainScreen.h`**:
   - The main menu screen that allows navigation to other screens.

5. **`clsTransactionsScreen.h`**:
   - Handles transaction-related operations (e.g., deposit, withdraw, transfer).

6. **`clsManageUsersScreen.h`**:
   - Manages user-related operations (e.g., add, update, delete users).

7. **`clsDate.h`**:
   - Provides date-related utilities (e.g., date formatting, calculations).

8. **`clsUtil.h`**:
   - Provides utility functions (e.g., random number generation, encryption).

9. **`Global.h`**:
   - Contains global variables (e.g., `CurrentUser`).

10. **`opplib.cpp`**:
    - The main entry point of the application.

11. **`Users.txt`**:
    - Stores user data (e.g., username, password, permissions).

12. **`Clients.txt`**:
    - Stores client data (e.g., account number, balance).

13. **`LoginRegister.txt`**:
    - Stores login history.

---

## **How to Run the Project**
1. **Prerequisites**:
   - Install Visual Studio or any C++ compiler.
   - Ensure the project files are correctly linked.

2. **Steps**:
   - Open the project in Visual Studio.
   - Build the project (`Build > Build Solution`).
   - Run the project (`Debug > Start Without Debugging`).

3. **Login**:
   - Use the default username and password from `Users.txt` (e.g., `User1` with password `3456`).

---

## **Usage**
1. **Main Menu**:
   - The main menu provides options for client management, transactions, and user management.

2. **Client Management**:
   - Add, update, delete, or find clients.

3. **Transactions**:
   - Deposit, withdraw, or transfer funds.

4. **User Management**:
   - Add, update, delete, or find users.

5. **Login Register**:
   - View login history.

---
