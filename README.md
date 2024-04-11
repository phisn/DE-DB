Idea is to create a DB which focuses on projects that use DDD. 
- Different from conventional DDD we only allow the DB to be mutated through events.
- To force integrety we could either use transactions or force commutivity.
- Our database stores the events and implicitly converts them into views. The views are the actual domain model.
- Users can either listen to events or query the domain model.

In normal DDD applications the domain is enforced at application level. In this concept the domain is enforced at database level therefore the database must be able to capture complex domain rules.
