# atlas-es-indexer
PoC to pull RIPE Atlas measurement results from the streaming API and push them to Elasticsearch.

Elasticsearch mapping needs to be optimised as the streaming of all 13 root name servers over both address families and multiple measurement types will quickly yield many dozens of millions of documents.

Here's some sample charts created with kibana after the cursory exploratory analysis of data :)

Slowest countries reaching any of the 13 root-servers, split by address-family
![alt text](https://raw.githubusercontent.com/ioc32/atlas-es-indexer/master/latency-desc-by-af-cc.png "latency-desc-by-af-cc")

Fastest countries reaching any of the 13 root-servers, split by address-family
![alt text](https://raw.githubusercontent.com/ioc32/atlas-es-indexer/master/latency-asc-by-af-cc.png "latency-asc-by-af-cc")

Root zone serials seen over time
![alt text](https://raw.githubusercontent.com/ioc32/atlas-es-indexer/master/root-serials.png "root-serials")
