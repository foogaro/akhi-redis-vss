# Rediscover Redis for Vector Similarity Search
Redis Vector Similarity Search Workshop Materials.

Here is the workshop slides [deck](https://docs.google.com/presentation/d/1-81YCn6ORjXM9HEbLLez9I-8s6DCVq28/edit?usp=sharing&ouid=102681544119043724410&rtpof=true&sd=true).

## Video Tutorials

<table>
    <tr>
        French
        <td><a href="https://drive.google.com/file/d/1pINEMJ_WFa5gusTl4oqtDLBGg3NbTuZ7/view?usp=sharing"><img src="https://github.com/aelkouhen/redis-vss/assets/22400454/d38b67ec-2574-4e8a-a89c-6954b8b6f064" style="float: right;" width="500" height="200"/></a></td> 
        English (Coming soon) 
        <td><a href=""><img src="https://github.com/aelkouhen/redis-vss/assets/22400454/d38b67ec-2574-4e8a-a89c-6954b8b6f064" style="float: right;" width="500" height="200"/></a></td> 
    </tr>
</table>

## Table of Contents

* [Pre-requisites](##Pre-requisites)
* [Text Vector Search](##Demo 1: Text Vector Search)
* [Visual Vector Search](##Demo 2: Visual Vector Search)
* [Hybrid Search](##Demo 2bis: Hybrid Vector Search)
* [Semantic Search](##Demo 3: Semantic Search)
* [Retieval-Augmented Generation](##Demo 4: Retieval-Augmented Generation (RAG))

## Pre-requisites
You need to create a Redis Enterprise DB with `RedisJSON` and `RediSearch` modules. Then, Use the public endpoint in the notebooks.

To create a Redis Enterprise database, you can use [Redis Cloud](https://app.redislabs.com/) or you can provision a cluster in your own infrastructure using [TerrAmine](https://github.com/amineelkouhen/terramine).

<img alt="Capture d’écran 2023-10-06 à 15 59 35" src="https://github.com/aelkouhen/redis-vss/assets/22400454/7c34580a-a200-4f28-89d1-4b1d77d4554e">

## Demo 1: Text Vector Search [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/aelkouhen/redis-vss/blob/main/1-%20Text%20Vector%20Search.ipynb) 

In this demo, you will learn how to:
- Create vector embeddings for text,
- Persist vector integrations in Redis,
- Create a Secondary Search Index on these Vectors,
- Find similarity between a new vector (text) and already persisted vectors.

![image](https://github.com/aelkouhen/redis-vss/assets/22400454/58b95c48-8bb5-4a27-aaf4-4b104149379e)

## Demo 2: Visual Vector Search [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/aelkouhen/redis-vss/blob/main/2-%20Visual%20Vector%20Search.ipynb) 

In this second demo, you will learn how to:
- Create vector embeddings for products (by image),
- Persist vector embeddings in Redis,
- Create a Secondary Search Index on these Vectors,
- Find similarity between a new vector (image) and the already persisted vectors.

![ezgif-2-9f2d8adeb3](https://github.com/aelkouhen/redis-vss/assets/22400454/b939748b-6b8d-4af7-8ef3-fd3fbd8da86a)

## Demo 2bis: Hybrid Search [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/aelkouhen/redis-vss/blob/main/2bis-%20Hybrid%20Search.ipynb)

In this demo, you will learn how to:
- Create vector embeddings for products (by image),
- Persist JSON documents containing the vector embeddings and other fields (e.g., tag, location, price...) in Redis,
- Create a Secondary Search Index on these documents,
- Find similarity between a new vector (image) and the already persisted vectors.
- Search for similarity between a new vector (image) and already persisted vectors, pre-filtered by a tag, a location, or a price range.

![image](https://github.com/aelkouhen/redis-vss/assets/22400454/b4ec3ce7-2f24-4f9a-956f-da8d251bc518)

## Demo 3: Semantic Search [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/aelkouhen/redis-vss/blob/main/3-%20Semantic%20Vector%20Search.ipynb)

In this demo, you will learn how to:
- Create vector embeddings for a private knowledge base (e.g., White papers, blog posts, newsletters...),
- Persist vector embeddings in Redis,
- Create a Secondary Search Index on these Vectors,
- Search semantically (natural language) for the already persisted vectors (relevant resources),
- Use Redis as a semantic cache.

![image](https://github.com/aelkouhen/redis-vss/assets/22400454/14e1c0f6-f414-4c4e-9cbe-4b2c3ed4a021)

## Demo 4: Retieval-Augmented Generation (RAG) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/aelkouhen/redis-vss/blob/main/4-%20Retrieval-Augmented%20Generation%20(RAG).ipynb)

In this last demo, you will learn how to:
- Create vector embeddings for a private knowledge base (e.g., PDF files, blogs posts, Database),
- Persist vector embeddings in Redis,
- Create a Secondary Search Index on these Vectors,
- Search semantically (natural language) for the already persisted vectors (relevant resources),
- Use relevant resources as a prompt context for LLM conversation,
- Generate an augmented response (natural language),
- Use Redis as a standard cache,
- Use Redis as a semantic cache,
- Use Redis as Q/A history.

![image](https://github.com/aelkouhen/redis-vss/assets/22400454/1705f88a-ab4c-45a1-9246-170b20e687dd)



