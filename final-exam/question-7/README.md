Final: Question 7
=================

**Problem:**

Assume a collection called **people_heights** with documents that look like this:

```
{
  "name": "Ada",
  "height": 1.7
}
```

<details> 
  <summary>Which of the following queries will find only the 4th- and 5th-tallest people in the people_heights collection represented by the coll object?</summary>
   Answer: (X) db.people_heights.find().sort("height", -1).skip(3).limit(2)
</details>


