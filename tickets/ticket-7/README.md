Ticket: Durable Writes
======================

**Problem:**

**Task**

For this ticket, you'll be required to increase the durability of the **add_user** method from the default Write Concern of **w: 1**.

When a new user registers for MFlix, their information must be added to the database before they can do anything else on the site. For this reason, we want to make sure that the data written by the **add_user** method will not be rolled back.

We can decrease the chances of a rollback by increasing the write durability of the **add_user** method. To use a non-default Write Concern with a database operation, use Pymongo's with_options flag when issuing the query.

---

**Testing and Running the Application**

There are no unit or integration tests for this lab.

Please complete the multiple choice question below, and then implement the correct Write Concern in the **add_user** method.

The implementation of this task will not be tested, but using the default of _w: 1_ might result in a rollback of your users' account data!

---

**Correct answers:**

**WriteConcern.W2 and WriteConcern.MAJORITY**

n a 3-node replica set, these two Write Concerns will both wait until 2 nodes have applied a write. This is because 2 out of 3 nodes is a majority, and waiting for 2 nodes to apply a write is **more durable** than only waiting for 1 node to apply it.

**Incorrect answers:**

_WriteConcern.W1_

This is already the default Write Concern in MongoDB, so it does not represent a higher durability than the default.

_WriteConcern.UNACKNOWLEDGED_

This will not wait for any nodes to apply a write before sending an acknowledgement, so it is a less durable write than the default value of **WriteConcern.W1**.

**Updated addUser method (using w: majority ):**

```
/**
* @return Success or failure
*/
public boolean addUser(User user) {
    usersCollection.withWriteConcern(WriteConcern.MAJORITY).insertOne(user);
    return true;
}
```
