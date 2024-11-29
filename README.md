# RAG
Retrieval-Augmented Generation for LLM

- Chunking
    - Viz
        - [chunk viz link](https://chunkviz.up.railway.app/)

- RAG workflow components

- Vector search
    - 2 strategies
        - exact search a.k.a KNN
            - Brute force to find nearest neighbors
                - Example
                    - K-nearest neighbors (KNN)
        - Approximate nearest neighbors (ANN)
            - Trade accuracy for speed gains
            - Examples of indexing algorithms
                - Tree based: ANNOY by spotify
                - Promximity graphs: HNSW
                - Clustering: FAISS by FB
                    - Forms clusters of dense vectors and conducts product quantization
                    - Working:
                        - Compute euclidean distance between all points and query vector
                        - given a query vector, identify which cell it belongs to
                        - find all other vectors belonging to that cell
                    - Limitation:
                        - not good with sparse vectors
                - Hashing: LSH
                - Vector compression: SCaNN by Google
    - How to measure 2 vectors are similar?
        - Distance metrics
            - Higher the metric, less similar
                - L1 (Manhattan) distance
                - L2 (Euclidean) distance
        - Similarity metrics
            - Higher metric, more similar
            - Cosine
                - if 10 degree is the angle between two vector, cos(10) = 0.98 i,e 98% similar


- Filtering
    - Fiter types
        - Post query
        - In-query
        - Pre-query


- Vector store
    - Cons
        - provides search functionality
        - scalability
        - speed
        - full fledged db properties
- Prompt

### AWS Cloud Services

#### Vector DBs

- Amazon OpenSearch Service (provisioned)
- Amazon OpenSearch Serverless
- pgvector extension in Amazon Relational Database Service (Amazon RDS) for PostgreSQL
- pgvector extension in Amazon Aurora PostgreSQL - Compatible Edition


