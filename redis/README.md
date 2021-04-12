# Redis Highlights:
* ReDiS stands for **Re**mote **Di**ctionary **S**erver
* It is a NoSQL (Key-Value Store) open-source data store
* It is in-memory data store and data can also be persited on disk aynchronously
* Redis is very easy to install and manage
* It is very very fast in serving the queries
  * Approx it can serve 100K (1 Lacks ) queries per second [ref](https://www.digitalocean.com/community/tutorials/how-to-perform-redis-benchmark-tests)
  * It is fast because the data is stored in-memory
* Redis can have key length max size of 2GB
* Sides is Single Threaded 
* Redis supports simple master-slave replication
* 
* Following are popular usecases for the use of redis
  * Caching 
  * Any short living data in the application
    * Web application session
    * Web page hit count
  * Messaging Queues (Redis natively supports Pub-Sub)
* Different Data types of Redis values
  * String
  * Lists
  * Sets
  * Sorted Sets
  * Hashes
  * Bitmaps
  * HyperLogLog
  * Geo Spatial Indexes
* Durability with Redis
 * There is always tradeoff between durability and speed
 * So because the data is stored in-memroy, there are chances of data loss
 * To minimize the data loss, Redis provides option to persist data on disk Asynchronously
  * Whenever new command is added to append log file -> class fsync() eachtime
  * or keep calling fsync() in every second (so at max there will be data loss of 1 second)   


---

# References:
[scan-vs-keys-performance-in-redis](https://stackoverflow.com/questions/32603964/scan-vs-keys-performance-in-redis)
[redis-iterating-over-keys](https://scalegrid.io/blog/redis-iterating-over-keys/)
