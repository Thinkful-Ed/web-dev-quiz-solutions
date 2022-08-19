Please use the `sample_mflix` database and the `movies` collection to answer the following questions:

1 - Which of the following queries would you use to find all movies in the database that were released after 2010?

A. {"year": {$eq: 2010}}

B. {"year": {$gt: 2010}}

C. {"year": {$lt: 2010}}

D. {"year": {$set: 2010}}

**Answer: B**

2 - Which of the following queries would you use to find all movies from 2006 with a metacritic rating greater than 97?

A. `{$and:[{"year": 2006, {"metacritic": {$gt: 97} ]}`

B. `{$or:[{"year": 2006}, {"rated": {$gt: 97}} ]}`

C. `{$and:[{"year": 2006}, {"metacritic": {$gt: 97}} ]}`

D. `{$and:[{"year": 2006}, {"rated": {$gt: 97}} ]}`

**Answer: C**

3 - For the query above, which movie is returned?

A. Pan's Labyrinth

B. The Science of Sleep

C. Little Miss Sunshine

D. Bride of Chucky

**Answer: A**

4 - Which of the following operators is used to match any of the values specified in an array?

A. $in

B. $eq

C. $array

D. $text

**Answer: A**

5 - Which of the following queries would you use to find all movies that are longer than 2 hours (120 minutes) and have a metacritic rating of less than 20?

A. {$and:[{"runtime": {$gt:120}}, {"metacritic": {$gt: 20}} ]}

B. {$and:[{"runtime": {$gt:120}}, {"metacritic": {$lt: 20}} ]}

C. {$and:[{"runtime": {$lt:120}}, {"metacritic": {$gt: 20}} ]}

D. {$and:[{"runtime": {$lt:120}}, {"metacritic": {$lt: 20}} ]}

**Answer: B**


6 - For the query above, how many documents are returned?

A. 5

B. 10

C. 15

D. 2

**Answer: A**


7 - True or False.

`$push` and `$pull` are used to modify arrays

A. True

B. False

**Answer: A**

