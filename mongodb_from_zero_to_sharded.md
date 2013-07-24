###MongoDB from Zero to Sharded

Shaun Verch - Server Engineer @ 10gen
github.com/Zarkantho/OSCON_Examples

scripts in his github repo with lots of examples for using mongodb, i.e. inserts, updates, basics…

indexes are the single biggest tunable performance factor in MongoDB

collections can not have > 64 indexes

queries can only use 1 index *

tons of good information in the slides - not sure where to find them

documents have a 16mb limit - would be difficult on a very large blog post or something with a lot of embedded data.

replica sets: high availability, operations
sharding: horizontal scale

replication allows for data being served from multiple different data centers

you need to have an odd number of nodes in a replica set

adding in another two replicas could be used to do analytics & backups

strong consistency is resulted from reading and writing to the primary of a replica set

delayed consistency is you read from the secondary servers and write to the primary

write concern conditions are used for testing whether write was successful.

for upgrades, you can upgrade all your secondaries, then take down the primary and upgrade it

you can use arbiters to achieve a odd number of replicas if needed.  it could be run on app server or monitoring server as it doesn't keep a copy of any data.

mongo localhost:30002 setup.js (connects to a certain instance, then runs the javascript file)

lots of performance upgrades should be made before moving on to sharing

sharding, you determine your key range.  think encyclopedias hit-ind, inf-kan, etc…

a shard can be a single mongod or a replica set

production shard setups must have 3 config servers, not a replica set

config servers store cluster chunk ranges

mongos replaces mongod in communication with app server (clients) in sharded cluster

he has another session on wednesday discussing how to choose a shard key

each shard could be a replica set so you could have each shard spread out across the world

