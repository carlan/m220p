Final: Question 3
=================

**Problem:**

Suppose an instance of **MongoClient** is created with the _default settings_:

```
from pymongo import MongoClient

uri = "mongodb+srv://m220-user:m220-pass@m220-lessons-mcxlm.mongodb.net/test"
mc = MongoClient(uri)

mc.stats
```

<details> 
  <summary>What will be the output of mc.stats?</summary>
   Answer: Database(MongoClient(host=['m220-lessons-shard-00-02-mcxlm.mongodb.net:27017', 'm220-lessons-shard-00-00-mcxlm.mongodb.net:27017', 'm220-lessons-shard-00-01-mcxlm.mongodb.net:27017'], document_class=dict, tz_aware=False, connect=True, authsource='admin', replicaset='m220-lessons-shard-0', ssl=True), 'stats')
</details>