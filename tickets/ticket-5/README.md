Ticket: Faceted Search
======================

**Problem:**

**User Story**

"As a user, I want to be able to filter cast search results by one facet, **metacritic** rating."

---

**Task**

For this ticket, you'll be required to modify the **getMoviesCastFaceted** method inin _db.py_, **get_movies_faceted**, so the MFlix application can perform faceted searches. 

What is a Faceted Search?

Faceted search is a way of narrowing down search results as search parameters are added. For example, let's say MFlix allows users to filter movies by a rating from 1 to 10, but Kate Winslet has only acted in movies that have a rating of 6 or higher.

If we didn't specify any other search parameters, MFlix would allow us to choose a rating between 1 and 10. But if we first search for Kate Winslet, MFlix would only let us choose a rating between 6 and 10, because none of the movie documents in the result set have a rating below 6.

If you're curious, you can read more about Faceted Search here.

_Faceted Search in MFlix_

Faceted searches on the MFlix site cannot be supported with the basic search method **get_movies**. For faceted searches, the application must use the Aggregation Framework.

The method **get_movies_faceted** uses the Aggregation Framework, and the individual stages in the pipeline have already been completed. Follow instructions in the _db.py_ file to add the required stages to the pipeline object.

---

**MFlix Functionality**

By default, faceted searches are not enabled. To enable faceted search in the UI, open the **index.html** file and enter:

```
useFacets: true
```

in the **mflix** object.

Once implemented, the available movie search parameters will reflect the other search criteria.

---

**Testing and Running the Application**

Look in the _test_facets.pyt file in your **tests** directory to view the unit tests for this ticket.

You can run the unit tests for this ticket by running:

```
pytest -m facets
```

Once the unit tests are passing, run the application with:

```
python run.py
```

Now proceed to the status page to run the full suite of integration tests and get your validation code.

<details> 
  <summary>After passing the relevant tests, what is the validation code for Faceted Search?</summary>
   Answer: 5aa7d3948adcc3fb770f06fb
</details>