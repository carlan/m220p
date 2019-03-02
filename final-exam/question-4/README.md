Final: Question 4
=================

**Problem:**

Suppose a client application is sending writes to a replica set with 3 nodes:

![](/final-exam/images/replica_set_primary_secondary_highlighted_ack.png?raw=true "")

Before returning an acknowledgement back to the client, the replica set **waits**.

When the write has been applied by the nodes marked in **stripes**, it returns an acknowledgement back to the client.

<details> 
  <summary>What Write Concern was used in this operation?</summary>
   Answer: (X) w: majority
</details>


