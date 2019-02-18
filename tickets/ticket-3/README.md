Ticket: Subfield Text Search
============================

**Problem:**

**User Story**

"As a user, I'd like to be able to search movies by cast members, genre, or perform a text search of the plot summary, full plot, and title."

---

**Task**

For this ticket, you will need to modify the method **build_query_sort_project** in db.py_ to allow the following movie search criteria:

- _cast_: finds all movies that match the cast members of a movie

Already, the **build_query_sort_project** method is able to return results for two different types of movie search criteria:

- _text_: performs a text search in the movies collection
- _genres_: finds movies that include any of the wanted genres.

You just need to construct the query that retrieves the _movies_ collection by cast.

A text index was created for you when you restored the collections with **mongorestore**, so these queries will be efficient once they are implemented.

**Hint**

Check the implementation of similar formats of search criteria - the _cast_ query should similar.

---

**MFlix Functionality**

Once you complete this ticket, the UI will allow movie searches by criteria of the **cast**, movie **genres**, movie **title**, and **plot** summary.

---

**Testing and Running the Application**

Make sure to look at the tests in _test_text_and_subfield_search.py_ to understand what is expected.

```
pytest -m text_and_subfield_search
```

Once the unit tests are passing, run the application with:

```
python run.py
```

Now proceed to the status page to run the full suite of integration tests and get your validation code.

<details> 
  <summary>After passing the relevant tests, what is the validation code for Text and Subfield Search?</summary>
   Answer: 5a96a6a29c453a40d04922cc
</details>