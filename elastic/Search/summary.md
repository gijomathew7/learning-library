
# Elastic Search

Distributed search engine.

## Lucene vs Elastic Search
Lucene is java library with search/indexing feature.Elastic search is based on lucene and it provides additional capabilites.

## Index
An elastic search index is a collection of json documents.Each document consists of a collection of fields(key-value pairs).

### Shards
A shard is a subset of documents of an index.It is a self contained lucene index.

## Indexing data
Elasticsearch stores the data to be searched as json documents.
When the data is uploaded to elastic search ,it is analysed and broken down into individual terms and is stored in an inverted index.An inverted index is similar to the index of a book.It contains a list of each term and and for each term, the list of documents in which it appears.


## Reference
Lucene(https://lucene.apache.org/core/)
