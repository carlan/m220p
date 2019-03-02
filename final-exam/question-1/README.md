Final: Question 1
=================

**Problem:**

Assume a collection called _elections_ that holds data about all United States Presidential Elections since 1789. All the documents in the _elections_ collection look like this:

```
{
  "year" : 1828,
  "winner" : "Andrew Jackson",
  "winner_running_mate" : "John C. Calhoun",
  "winner_party" : "Democratic",
  "winner_electoral_votes" : 178,
  "total_electoral_votes" : 261
}
```

_total_electoral_votes_ represents the total number of electoral votes that year, and _winner_electoral_votes_ represents the number of electoral votes received by the winning candidates.

<details> 
  <summary>Which of the following query filters will retrieve all the Republican winners with at least 160 electoral votes?</summary>
   Answer: db.elections.find( { "winner_party": "Republican",
                                "winner_electoral_votes": { "$gte": 160 } } )
</details>