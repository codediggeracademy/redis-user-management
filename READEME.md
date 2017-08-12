# Redis User Management

Simple user management app using Node.js and Redis as database. It can be potentially  be used
for server side caching to make ultra fast node application.

## About Redis

Redis is an open source (BSD licensed), in-memory data structure store, used as a database, cache and message broker. It supports data structures such as strings, hashes, lists, sets, sorted sets with range queries, bitmaps, hyperloglogs and geospatial indexes with radius queries. Redis has built-in replication, Lua scripting, LRU eviction, transactions and different levels of on-disk persistence, and provides high availability via Redis Sentinel and automatic partitioning with Redis Cluster
To read mode about it [https://redis.io/]

## Advantages of Redis

###Exceptionally Fast : 
Redis is very fast and can perform about 110000 SETs per second, about 81000 GETs per second. You can use the redis-benchmark utility for doing the same on your machine.

###Supports Rich data types : 
Redis natively supports most of the datatypes that most developers already know like list, set, sorted set, hashes. This makes it very easy to solve a variety of problems because we know which problem can be handled better by which data type.

###Operations are atomic : 
All the Redis operations are atomic, which ensures that if two clients concurrently access Redis server will get the updated value.

###MultiUtility Tool : 
Redis is a multi utility tool and can be used in a number of usecases like caching, messaging-queues (Redis natively supports Publish/ Subscribe ), any short lived data in your application like web application sessions, web page hit counts, etc.  There are a lot of people using Redis and they can be found at http://redis.io/topics/whos-using-redis

## Getting Started [Based on Mac]

### Prerequisites

First you need to install redis server from [https://redis.io/download]. Once you unzip the downloaded
zip file and unzipped run below commands

Start Redis server
```
$ redis-server /usr/local/etc/redis.conf
```

Test your redis server by running  redis cli by below command
```
$ redis-cli ping
```
If it replies “PONG”, then it’s good to go!  



### Installing

Now lets start our user management project 

```
git clone git@github.com:heroku/node-js-sample.git # or clone your own fork
cd node-redis
npm install
npm start
```

And go to browser on below to see your application link

```
http://localhost:3000/
```

End with an example of getting some data out of the system or using it for a little demo


## License

This project is licensed under the MIT License 

## Acknowledgments

* Pls refer [https://redis.io/commands/] for more commands
