### MapReduce All The Way Down

Russell Branca - github.com/chewbranca - @chewbranca

map reduce is a distributed algorithm for data processing - divide & conquer algorithm.

map reduce is divide & conquer in parallel and at scale

map: filter & sort data

reduce: aggregation and analysis

canonical example word count

map(doc) ->  
  for word in doc:  
    emit(word, 1)  

google mapreduce is the original implementation, used in web crawler & page rank

hadoop -> open source apache project (distributed & parallel), very popular, highly used in industry

couchdb -> another open source apache project, database not an engine for running parallel map reduce functions.  It actually uses mapreduce for secondary indexes.  Purely functional and stateless.

batch processing means having to run entire map/reduce process every time.

incremental saves the results in a *b-tree* and allows you to run new data against it

