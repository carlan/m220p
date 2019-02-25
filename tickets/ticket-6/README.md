Ticket: User Management
=======================

**Problem:**

**User Story**

"As a user, I should be able to register for an account, log in, and logout."

---

**Task**

For this Ticket, you'll be required to implement all the methods in _db.py_ that are called by the API endpoints in _user.py_. Specifically, you'll implement:

- **get_user**
- **add_user**
- **login_user**
- **logout_user**
- **get_user_session**
- **delete_user**

Registering should create an account and log the user in, ensuring an entry is made in the **sessions** collection. There is a unique index on the **user_id** field in **sessions**, so we can efficiently query on this field.

---

**MFlix Functionality**

Once this ticket is completed, users will be able to register for a new account, log in, logout, and delete their account.

---

**Testing and Running the Application**

Look within the _test_user_management.py_ file in your tests directory to view the unit **tests** for this ticket.

You can run the unit tests for this ticket by running:

```
pytest -m user_management
```

Once the unit tests are passing, run the application with:

```
python run.py
```

Now proceed to the status page to run the full suite of integration tests and get your validation code.

<details> 
  <summary>After passing the relevant tests, what is the validation code for User Management?</summary>
   Answer: 5a8d8ee2f9588ca2701894be
</details>