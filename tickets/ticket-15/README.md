Ticket: Handling Timeouts
=========================

**Problem:**

**Task**

For this ticket, you'll be required to modify the connection information for **MongoClient** to set a write concern timeout of **2500** milliseconds.

The **MongoClient** in _db.py_ is initialized in the _get_db_ method. A link to the relevant documentation is included here for your reference.
---

**Testing and Running the Application**

You can run the unit tests for this ticket by running:

```
pytest -m timeouts
```

Once the unit tests are passing, run the application with:

```
python run.py
```

Now proceed to the status page to run the full suite of integration tests and get your validation code.

<details> 
  <summary>After passing the relevant tests, what is the validation code for Timeouts?</summary>
   Answer: 5addf035498efdeb55e90b01
</details>