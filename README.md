# Transaction Processing System

## Mini Project

This project is a C language mini project that manages bank account records using a random access file. The program stores account information in `credit.dat` and allows the user to add, view, search, update, and delete account records.

## Objective

The objective of this project is to understand file handling in C, especially random access file processing. The project also improves the given base program by adding new features, validation, and better menu options.

## Files Included

| File Name | Description |
|---|---|
| `trans.c` | Main C source code |
| `credit.dat` | Binary file used to store account records |
| `clients.dat` | Sample binary account data file |
| `MINI PROJECT Guidelines.pdf` | Project guideline file |
| `README.md` | Project documentation |

## Features

1. Create a printable `accounts.txt` file.
2. List all active accounts on the screen.
3. Search an account by account number.
4. Add a new account.
5. Deposit amount into an account.
6. Withdraw amount from an account.
7. Prevent withdrawal when balance is insufficient.
8. Delete an existing account.
9. Count total active accounts.
10. Validate account numbers from 1 to 100.
11. Automatically create `credit.dat` if it is missing.
12. Regenerate `credit.dat` if the file size is invalid.

## Menu Options

```text
1 - store a formatted text file of accounts called "accounts.txt" for printing
2 - list all accounts
3 - search an account
4 - add a new account
5 - deposit amount
6 - withdraw amount
7 - delete an account
8 - count active accounts
9 - end program
```

## How to Compile

Open the project folder in VS Code or terminal and run:

```powershell
gcc trans.c -o trans.exe
```

## How to Run

```powershell
.\trans.exe
```

## Sample Test

```text
4
1
Smith John 1000
2
5
1
500
6
1
200
3
1
8
1
9
```

## Sample Test Explanation

| Input | Action |
|---|---|
| `4` | Add new account |
| `1` | Account number |
| `Smith John 1000` | Last name, first name, balance |
| `2` | List all accounts |
| `5` | Deposit amount |
| `1` | Account number |
| `500` | Deposit amount |
| `6` | Withdraw amount |
| `1` | Account number |
| `200` | Withdraw amount |
| `3` | Search account |
| `1` | Account number |
| `8` | Count active accounts |
| `1` | Generate `accounts.txt` |
| `9` | Exit program |

## Output File

When option `1` is selected, the program creates:

```text
accounts.txt
```

This file contains the formatted account details for printing.

## Error Handling

The program handles the following errors:

- Invalid account numbers
- Missing `credit.dat` file
- Incorrect `credit.dat` file size
- Duplicate account creation
- Searching for non-existing accounts
- Deleting non-existing accounts
- Invalid deposit or withdrawal amount
- Insufficient balance during withdrawal

## Conclusion

This project demonstrates random access file handling in C and provides a simple transaction processing system with useful banking operations.
