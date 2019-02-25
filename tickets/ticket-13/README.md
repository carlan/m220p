Ticket: Migration
=================

**Problem:**

**Task**

For this ticket, you'll be required to complete the command-line script located in the _migrations_ directory of _mflix_ called **movie_last_updated_migration.py**.

Things always change, and a requirement has come down that the _lastupdated_ value in each document of the _movies_ collection needs to be stored as an **ISODate** rather than a **String**.

Complete the script so it updates the values using the bulk API.

To perform the migration, run the script:

```
python movie_last_updated_migration.py
```

---

**Testing and Running the Application**

You can run the unit tests for this ticket by running:

```
pytest -m migration
```

Once the unit tests are passing, run the application with:

```
python run.py
```

Now proceed to the status page to run the full suite of integration tests and get your validation code.

<details> 
  <summary>After passing the relevant tests, what is the validation code for Migration?</summary>
   Answer: 5ad9f6a64fec134d116fb06f
</details>