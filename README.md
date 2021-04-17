# B4nk API

## Table of Contents

- [About](#about)
- [Getting Started](#getting_started)
- [Usage](#usage)

## About <a name = "about"></a>

a Bank Api - as a manager in the bank the user can do the following tasks:
Add users,Depositing,Update credit,Withdraw money,Transferring,Show details of user,Show details of all users.

## Getting Started(Docs) <a name = "getting_started"></a>

| Action                         | Method | Link                              |
| ------------------------------ | ------ | --------------------------------- |
| Get all users                  | GET    | /users                            |
| Get user                       | GET    | /users/:id                        |
| Create new user                | POST   | /users                            |
| Deposit cash in user           | PUT    | /users/:id/deposit/:amount        |
| Update credit in user          | PUT    | /users/:id/credit/:amount         |
| Transfer cash between 2 users  | POST   | /users/transfer/:id1/:id2/:amount |
| Withdraw cash from user        | POST   | /users/:id/withdraw/:amount       |
| Filter by Cash                 | GET    | /users/query/:query               |
| Filter by negative of positive | GET    | /users/np/:p                      |

## Usage <a name = "usage"></a>

To start and serve the API :

```bash
node app.js
```

then make the different requests to API in http://localhost:3000

![Alt text](screenshots\post_man_reqs_to_bank_api.png "postman_reqs")
