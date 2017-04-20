# atlas-es-indexer
PoC to pull RIPE Atlas measurement results from the streaming API and push them to Elasticsearch.

Elasticsearch mapping needs to be optimised as the streaming of all 13 root name servers over both address families and multiple measurement types will quickly yield many dozens of millions of documents.
