1 -

True or false.

In MongoDB, databases are containers for *collections*

A. True

B. False

**Answer: A**

2 - 

True or false.

A *document* in MongoDB is a set of field-value pairs that stores data.

A. True

B. False

**Answer: A**

3 - 

Which of the following commands allows you to select the database you want to interact with.

A. with

B. require

C. use

D. try

**Answer: C**

4 - 

Which of the following methods allows you to insert several documents into a collection?

A. db.collection.insert()

B. db.collection.insertOne()

C. db.collection.insertMany()

D. db.collection.insertSeveral()

**Answer: C**

5.

Which of the following code snippets allows you to update the status of all orders from "Awaiting Delivery" to "Delivered?"

A. 
```js
db.orders.updateMany(
  { "orderStatus": "Delivered" },
  { $set: {
      "orderStatus":"Awaiting delivery"
    }
  }
)
```

B.
```js
db.orders.updateMany(
  { "orderStatus": "Awaiting delivery" },
  { $set: {
      "orderStatus":"Delivered"
    }
  }
)
```

C. 

```js
db.orders.update(
  { "orderStatus": "Awaiting delivery" },
  { $set: {
      "orderStatus":"Delivered"
    }
  }
)
```

D.

```js
db.orders.updateMany(
  { "orderStatus": "Awaiting delivery" },
  { "orderStatus":"Delivered" }
)
```

**Answer: B**



