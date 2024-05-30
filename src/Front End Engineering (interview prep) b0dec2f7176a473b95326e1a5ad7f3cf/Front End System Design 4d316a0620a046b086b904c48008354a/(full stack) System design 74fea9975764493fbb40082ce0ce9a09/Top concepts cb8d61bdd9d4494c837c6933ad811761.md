# Top concepts

## Load balancing

Distribute traffic to many web services. Helps with throughput, latency, scalability.

Eg put load balancer in front of servers. 

Various techniques for load balancing

1. NGINX, route requests to IP addresses
2. DNS load balancing, given a domain name it can resolve to various IP address
    1. No need dedicated machine, 
    2. but less customizable 

You can setup rules for load balancing 

1. round robin 
2. Hashing on the ip address
3. figuring out which machine has the least load and assigning traffic to it
4. figuring out which machines are offline, and remove traffic from it
5. etc..

The database is generally more critical to high traffic then the server tho 

## Caching

You can insert an in memory caching layer, eg NYT returning articles. 

Eg you can set it to 24 hours cache

- memcache
- redis
- cassandra

CDN to cache static assets files

- images
- videos
- javascritp
- html
- css

CDN is a global network of servers. Located geographically closer to your users.

it decrease loads on your server.

CDN techniques 

1. Pull technique. First request "slow" but then cached to CND for subsequent requests.
2. Push technique. Faster first request, but higher upfront cost. And might get to CND end points that don't end up being used.

if users uploading images, then distributed file system, eg like S3

## Database schema

define 

- tables
- primary keys
- indices

Replication, slave master replication. One database you write to and others copies for read only.

## Scaling

- Web server
- image/assets server
- database server,

Web server —> Load balancer

image/assets server —> CDN 

Database server —→

- caching
- indexes
- replication

scaling Database writes 

Database **sharding**, splitting up database in multiple master database for the purpose of write.

- **vertical** sharing, splitting tables across different machines.
- **Horizontal** sharing, splitting a single table (eg tweets) across multiple machines. Various ways to do it. Most common, user id mod by number of machines you want to allocate user id to. Eg 5 master machines for that table. this routes the user id to a specific machine.

## NoSQL

Non relational. Collections and documents.

Key value pairs models. Can scale automatically across machines.

Common

- MongoDB
- DynamoDB, AWS
- Firebase/Firestore, GCP

Also can use hybrid approach. 

Eg for an active chat server. you can use NoSQL or in memory table. 

And relational DB like MySQL for a user table.

## API Design

Client & server. 

How do they communicate with each other? What are functions and methods they use?

Data transfer mechanism?

- JSON
- protocol buffer

How to handle security

offline usage

how to make it fast

## Clarifying questions

- What type of load and usage the system will have to deal with?

Eg avoid premature optimization, or scale to early as it might over complicate the system.

simplicity 

from 

[Systems Design Interview Concepts (for software engineers / full-stack web)](https://youtu.be/REB_eGHK_P4)