
# Elastic Search

Distributed search engine.

## Lucene vs Elastic Search
Lucene is java library with search/indexing feature.Elastic search is based on lucene and it provides additional capabilites.

## Index
An elastic search index is a collection of json documents.Each document consists of a collection of fields(key-value pairs).These documents are logically related.For example,documents in an product index will contain product info documents.It is divied into multiple shards.

### Shards
A shard is a subset of documents of an index.It is a self contained lucene index.It can be independently stored in any of the nodes in elastic cluster.Shards can have replica.
The lucene index stores data into segments.These segments are immutable. Primary shards cannot be changed after index creation,whereas replica shards can be.

## Indexing data
Elasticsearch stores the data to be searched as json documents.
When the data is uploaded to elastic search ,it is analysed and broken down into individual terms and is stored in an inverted index.An inverted index is similar to the index of a book.It contains a list of each term and and for each term, the list of documents in which it appears.
Documents are assigned to shards based on routing(https://www.elastic.co/blog/customizing-your-document-routing). 

## Analysis
The process of breaking down documents into text and tokens to insert in inverted index is called analysis.The processs varies based on the type of analyser.
Ex: standard analyser

## Components
### Cluster
Collection of elastic search nodes.One of the nodes is elected as master and is responisble for creating and deleting index and adding/deleting nodes.



## Reference
Lucene(https://lucene.apache.org/core/)
Elastic indexing basic (https://www.elastic.co/blog/found-elasticsearch-from-the-bottom-up)
