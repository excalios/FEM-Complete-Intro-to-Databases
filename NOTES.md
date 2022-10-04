# Postgres

## JSON

### Access JSON Properties

`Column Name -> Property Name`

Cast to text using double arrows
`Column Name ->> Property Name`

# Graph Databases

## Terminology

### Nodes / Entities

Represents a thing, a row, a document

### Relationships / Edges

It just defines that node A is connected to node B and it's gonna draw a line
between these nodes

### Properties / Attributes

Both nodes and relationships can have properties

# Redis

It's just caching with basically all SET and GET. There's also MSET and MGET
M for Many. Lua is also integrated in Redis. You can do transactions in redis

## Lists

Create
`RPUSH name "Data" "Data"`

Get
`LRANGE name start_index end_index`
index go from 0 to length or -1

Pop // Pop as in remove from array
`LPOP`
`RPOP`

Trim // Remove multiple
`LTRIM`
`RTRIM`

## Hash

Key value pair

Create
`HMSET name key value key value`

Get
`HGET name key`
`HGETALL name key`

## Set

Create
`SADD name values`

Check if value
`SISMEMBER name value`

Get all members
`SMEMBERS name`

Pop random member
`SPOP name`

## Sorted set

Similar to set but it uses kinda key value pair where the key is their priority

## Streams

A system where you can publish and subscribe to a key and get notified

## LRU

Least Recently Used it's where redis gonna check in the cache the least read and
updated key and delete it

## Redis Cluster (Revisit)

Sharding

## Redis Sentinel (Revisit)

Self Healing

# Questions

1. What is sharding
2. What is fragment
