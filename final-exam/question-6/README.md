Final: Question 6
=================

**Problem:**

Suppose a client application is sending writes to a replica set with three nodes, but the primary node stops responding:

![](/final-exam/images/replica_set_primary_down.png?raw=true "")

BAssume that none of the connection settings have been changed, and that the client is only sending insert statements with write concern w: 1 to the server.

<details> 
  <summary>If after 30 seconds, the client still cannot connect to a new primary; which of the following exceptions will be raised by the Pymongo?</summary>
   Answer: (X) ServerSelectionTimeoutError
</details>


