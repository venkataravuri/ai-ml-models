## Vector Databases

|Topic|Name|Description|
|---|---|---|
|Corpus Collection|[Web Scrape Content](5-vector-db/1-web-scrape.ipynb)|?|

- [The Best Vector Database for Stablecog's Semantic Search](https://stablecog.com/blog/the-best-vector-database-for-stablecogs-semantic-search)

## External Colab Notebooks

Qdrant & Text Data - https://colab.research.google.com/github/qdrant/examples/blob/master/qdrant_101_text_data/qdrant_and_text_data.ipynb


Approximate Neighbor Search

To reduce the computation complexity added by an exhaustive search like kNN we make use of approximate neighbor search.

Instead of checking distances between each vector in the database, we retrieve a “good guess” of the nearest neighbor. In some use cases, we would rather lose some accuracy in favor of performance gain, thus allowing us to scale our search. ANN allows us to get a massive performance boost on similarity search when dealing with huge datasets.

In approximately nearest neighbors (ANN), we build index structures that narrow down the search space and improve lookup times. 

### vector similarity search algorithms

Hierarchical Navigable Small World (HNSW) graphs are among the top-performing indexes for vector similarity search[1]. HNSW is a hugely popular technology that time and time again produces state-of-the-art performance with super fast search speeds and fantastic recall.

Yet despite being a popular and robust algorithm for approximate nearest neighbors (ANN) searches, understanding how it works is far from easy.
