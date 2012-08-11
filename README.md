# dbak

A simple DynamoDB backup tool.


## Meta

* author: Randall Degges
* email:  rdegges@gmail.com
* status: maintained, in development


## Purpose

I like using Amazon's [DynamoDB](http://aws.amazon.com/dynamodb/). It's fast as
*fuck*, easy to scale up (and down), has a [beautiful
API](http://boto.cloudhackers.com/en/latest/dynamodb_tut.html), and is great
for telephony stuff (which I do a lot of).

The only thing that really bothers me about DynamoDB is that there isn't a
decent backup tool for it--until now.

`dbak` is a simple, straightforward, and brainless DynamoDB backup tool
written in Python. It takes a dump of all your tables, and stores them either
locally, or to an S3 bucket of your choosing.

It even ships with a restore script so you can feed it the dump file, and watch
as it rebuilds your broken tables from scratch.


## Note

`dbak` is still in development. As time progresses, I'll gradually upgrade the
tool to be more efficient, but for now the main goal is getting the job done.
