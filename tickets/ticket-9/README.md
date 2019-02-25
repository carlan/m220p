Ticket: Get Comments
====================

**Problem:**

**User Story**

"As a user, I want to be able to view comments for a movie when I look at the movie detail page."

---

**Task**

For this ticket, you'll be required to extend the **get_movie** method in _db.py_ so that it also fetches the comments for a given movie. The comments should be returned in order from most recent to least recent using the _date_ key.

Movie comments are stored in the _comments_ collection, so this task can be accomplished by performing a _$lookup_. Refer to the Aggregation Quick Reference for the specific syntax.

---

**MFlix Functionality**

Once this ticket is completed, each movie's comments will be displayed on that movie's detail page.

---

**Testing and Running the Application**

You can run the unit tests for this ticket by running:

```
pytest -m get_comments
```

Once the unit tests are passing, run the application with:

```
python run.py
```

Now proceed to the status page to run the full suite of integration tests and get your validation code.

<details> 
  <summary>After passing the relevant tests, what is the validation code for Get Comments?</summary>
   Answer: 5ab5094fb526e43b570e4633
</details>