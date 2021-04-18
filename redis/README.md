# Learn Redis
## Highlights
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
* Following are popular usecases for the use of redis
  * Caching 
  * Any short living data in the application
    * Web application session
    * Web page hit count
  * Messaging Queues (Redis natively supports Pub-Sub)
* Different Data types of Redis values [Redis Commands](https://redis.io/commands/#)
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

## Redis Vs [Other Key-Value](https://en.wikipedia.org/wiki/NoSQL#Key-value_stores) Stores
* In Redis values can contain 
  * multiple complex data types
  * with atomic operation defined on those data types
* Redis is in-memory datastore along with Async persistance on disk

## Redis CLI
* Run the redis server with below command from the terminal / cmd
  ```
  $redis-server" 
  ```
* then execute "redis-cli" which will open the redis cli terminal
  ```
  $redis-cli
  redis 127.0.0.1:6379>
  redis 127.0.0.1:6379>ping
  PONG
  ```
* to connect to a remote redis server
  ```
  $redis-cli -h <hostname> -p <port> -a <password>
  ```
## Redis GUI Tool
* There are many tools available for Redis GUI, free and most convinient is 
  * another redis desktop manager [ref](https://www.electronjs.org/apps/anotherredisdesktopmanager)

## Redis Database / Schemas
 * WIP

## Redis KeySpace in Detail
 * WIP

## Redis Data Types in details

### Strings
 * WIP
 
### Lists 
 * WIP

### Hashesh (HashMap)
 * WIP
 
### Sets
 * WIP

### Sorted Sets
 * WIP

### BitMaps 
 * WIP

### HyperLogLog
 * WIP

### GeoSpatial Indexes
 * WIP

## Redis Transactions [ref](https://redis.io/topics/transactions)
 * WIP

## Redis as Pub-Sub
 * WIP

## Redis Persistance
 * WIP

## Redis Backup and Recovery
 * WIP

## Redis Master Slave
 * WIP

## Redis Cluster
 * WIP

---

### References:
* [redis-tutorial-by-javapoint](https://www.javatpoint.com/redis-tutorial)
* [scan-vs-keys-performance-in-redis](https://stackoverflow.com/questions/32603964/scan-vs-keys-performance-in-redis)
* [redis-iterating-over-keys](https://scalegrid.io/blog/redis-iterating-over-keys/)
* [redis-scan-count-match](https://redis.io/commands/scan)
* [manage-redis-db-keys](https://www.digitalocean.com/community/cheatsheets/how-to-manage-redis-databases-and-keys#:~:text=Redis%20databases%20are%20numbered%20from,select%2015)
* [redis-all-commands](https://www.javatpoint.com/redis-all-commands)
* [redis-interview-questions-and-answers](https://www.javatpoint.com/redis-interview-questions-and-answers)
* [redis-usecases](https://medium.com/@juwelariful1/what-is-redis-and-why-with-use-case-1b294b91e373)
* [redis-sentinel-high-availability](https://medium.com/@amila922/redis-sentinel-high-availability-everything-you-need-to-know-from-dev-to-prod-complete-guide-deb198e70ea6#:~:text=How%20Redis%20offers%20High%20Availability,mode%20without%20any%20human%20intervention.)
* [Data-Modeling-In-Redis](https://www.openmymind.net/Data-Modeling-In-Redis/)


### Video Tutorials:
* [Redis Course - In-Memory Database Tutorial by **freeCodeCamp.org**](https://www.youtube.com/watch?v=XCsS_NVAa1g)
* [Redis Crash Course Tutorial by **Traversy Media**](https://www.youtube.com/watch?v=Hbt56gFj998)
* [Redis Basics: Strings, Hashes, Lists, Pub/Sub by** Engineer Man**](https://www.youtube.com/watch?v=YWIzp3fRvvY&list=PL6HWCwMwHtEA2ByOcodpVQDJmR-BnLFU0&index=5)
