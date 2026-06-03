# Password Manager 🔐

A simple command-line Password Manager built with Python. This project allows users to store and retrieve passwords for different websites during program execution.

## Description

The program provides a menu-driven interface where users can:

1. Add a new password for a website.
2. View a saved password.
3. Exit the program.

Passwords are stored in a Python dictionary while the program is running.

## Code

```python
passwords = {}

while True:
    print("\n1. Add a new password")
    print("2. View a password")
    print("3. Exit")

    choice = input("Enter your choice: ")

    if choice == "1":
        website = input("Website: ")
        password = input("Password: ")
        passwords[website] = password

    elif choice == "2":
        website = input("Website: ")
        print(passwords.get(website, "Not found"))

    elif choice == "3":
        break
```

## How to Run

1. Install Python 3.
2. Save the code in a file named `password_manager.py`.
3. Open a terminal or command prompt.
4. Run:

```bash
python password_manager.py
```

## Example

```text
1. Add a new password
2. View a password
3. Exit

Enter your choice: 1
Website: github.com
Password: mypassword123

Enter your choice: 2
Website: github.com
mypassword123
```

## Features

- Store passwords for multiple websites
- Retrieve saved passwords quickly
- Simple menu-based interface
- Uses Python dictionaries for data storage
- Beginner-friendly project

## Concepts Used

- Dictionaries (`dict`)
- Loops (`while`)
- Conditional statements (`if`, `elif`)
- User input handling
- Dictionary methods (`get()`)

## Limitations

- Passwords are not encrypted
- Data is lost when the program closes
- No user authentication
- Passwords are displayed in plain text

## Future Improvements

- Save passwords to a file
- Encrypt stored passwords
- Add a master password for security
- Generate strong random passwords
- Create a graphical user interface (GUI)
- Search and delete saved passwords

## License

This project is open source and free to use.
