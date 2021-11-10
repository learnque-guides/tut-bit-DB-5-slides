# Relationship

* When designing a database, common sense dictates that we use different tables for different types of entities.
* Take for example an online store which has information about: customers, orders, items, etc. We would have separate tables for all of these. But we also need to have relationships between these tables. For instance a customer can place several orders, an order belongs to only one customer, an order can contain multiple items. These relationships need to be represented in the database.

There are several types of database relationships:
* One to One relationships,
* One to Many and Many to One relationships,
* Many to Many relationships,
* Self Referencing relationships.