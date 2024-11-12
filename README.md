# Interactive Data Exploration Using Knowledge Graphs and Queries

This project explores the construction and use of a knowledge graph, specifically utilizing a movie dataset. The objective is to create a knowledge graph that can be queried, enhanced with RAG (Retrieval-Augmented Generation), and integrated into a chatbot interface for answering user queries.

![image](https://github.com/user-attachments/assets/2fa4233d-19fa-4409-b242-d2aac33df695)




## Table of Contents

1. [Why Knowledge Graph](#1-why-knowledge-graph)
2. [Series Schema](#2-series-schema)
3. [Knowledge Graph Fundamentals](#3-knowledge-graph-fundamentals)
4. [How to Construct a Knowledge Graph](#4-how-to-construct-a-knowledge-graph)
5. [ChatBot Schema](#5-chatbot-schema)
6. [Knowledge Graph Agent](#6-knowledge-graph-agent)
7. [RAG with Knowledge Graph](#7-rag-with-knowledge-graph)
8. [Constructing Knowledge Graph with Movie Dataset](#8-constructing-knowledge-graph-with-movie-dataset)
    - a) Code Walkthrough (Notebooks)
        - [I. Preparing GraphDB](#i-preparing-graphdb)
        - [II. Data Preparation](#ii-data-preparation)
        - [III. Populating the Graph DB](#iii-populating-the-graph-db)
        - [IV. Q&A with Graph DB](#iv-q-a-with-graph-db)
        - [V. RAG with Graph DB](#v-rag-with-graph-db)
        - [VI. Chatbot Design and Test](#vi-chatbot-design-and-test)

---

### 1. Why Knowledge Graph
A knowledge graph provides a structured representation of knowledge, enabling better understanding and reasoning. By linking entities and defining their relationships, it becomes possible to retrieve relevant information efficiently. In this project, a knowledge graph helps represent movie data, which can be queried for complex questions about movies, actors, genres, and more. This structured approach makes it easier to answer questions that require multi-hop reasoning.

### 2. Series Schema
The schema defines the structure of the knowledge graph. It includes the entities (e.g., movies, actors, directors) and the relationships between them (e.g., acted_in, directed_by). The schema is crucial as it dictates how data is stored and queried within the graph. A well-designed schema enables seamless querying and ensures that the graph can scale with additional data without significant changes.

![HACK_1_4](https://github.com/user-attachments/assets/adf83813-d645-49ec-ba11-e539fa6b1698)


### 3. Knowledge Graph Fundamentals
Understanding the fundamentals of knowledge graphs involves learning about nodes (entities), edges (relationships), and properties (attributes). Knowledge graphs are designed to link related entities and provide context, making it possible to answer complex questions. This section covers the basics, including graph theory principles, storage techniques, and common use cases.

![image](https://github.com/user-attachments/assets/8d1a1303-a26b-4049-9f13-c2d677e89d92)


### 4. How to Construct a Knowledge Graph
This section provides a step-by-step guide on building a knowledge graph. It covers the setup of a Graph Database (GraphDB), data modeling based on the schema, and data ingestion techniques. Constructing a knowledge graph requires defining the schema, preparing the data, and loading it into the database in a way that preserves the relationships.

### 5. ChatBot Schema
The chatbot schema defines how the knowledge graph integrates with a chatbot. It includes defining intents and entities that the chatbot can understand, linking them to the knowledge graph for responses. This schema ensures that the chatbot can interpret user queries and retrieve answers from the knowledge graph effectively.

### 6. Knowledge Graph Agent
The Knowledge Graph Agent acts as an intermediary between the chatbot and the knowledge graph. It interprets queries from the chatbot, converts them into graph queries, retrieves the relevant information, and formats it for the chatbot's response. The agent plays a critical role in ensuring seamless communication between the chatbot and the graph database.

### 7. RAG with Knowledge Graph
Retrieval-Augmented Generation (RAG) combines knowledge graph retrieval with language generation models to provide enriched responses. In this project, RAG helps improve the chatbot’s responses by using the knowledge graph to fetch relevant data and a language model to generate coherent answers. This combination provides contextually accurate and fluent responses.

![HACK_1_3](https://github.com/user-attachments/assets/09130110-f3bc-4c37-b3d8-b90e52a6fdbe)


### 8. Constructing Knowledge Graph with Movie Dataset

This section describes the practical implementation of building a knowledge graph with a movie dataset.

#### a) Code Walkthrough (Notebooks)
This code walkthrough is divided into six steps, each with its own notebook, to make the process clear and manageable.

##### I. Preparing GraphDB
   - This step involves setting up a Graph Database (GraphDB) to store and manage the knowledge graph. We select a suitable graph database, configure it, and prepare it to store entities and relationships as defined in the schema.

##### II. Data Preparation
   - In this step, we prepare the movie dataset for ingestion. Data cleaning, transformation, and formatting are performed to ensure compatibility with the graph schema. This may involve converting data into nodes and relationships that align with our defined entities.

##### III. Populating the Graph DB
   - Here, we load the prepared data into GraphDB. This involves creating nodes (e.g., movies, actors, directors) and relationships (e.g., acted_in, directed_by). The graph is populated using scripts or tools that allow bulk loading, making the process efficient.

##### IV. Q&A with Graph DB
   - With the graph populated, we can now query it to answer questions. This section includes querying techniques for retrieving information, such as finding movies by genre, actors in a particular movie, or movies directed by a specific director. Sample queries are provided to demonstrate the graph's capabilities.

##### V. RAG with Graph DB
   - In this step, we integrate RAG (Retrieval-Augmented Generation) with the GraphDB. This involves using retrieval from the graph to provide context to a language generation model, allowing for more detailed and contextually relevant answers.

##### VI. Chatbot Design and Test
   - The final step involves designing and testing the chatbot. The chatbot uses the knowledge graph and RAG integration to answer user queries about movies. Testing ensures that the chatbot can accurately interpret and respond to queries, providing meaningful answers based on the knowledge graph.

## WorkFlow
![HACK_1_2](https://github.com/user-attachments/assets/4ae8c964-2584-49ea-b13d-58887de44d01)

## YOUTUBE LINK: https://youtu.be/KChdJkoikMk

## Requirements

- **Graph Database** (e.g., Neo4j, GraphDB)
- **Python** for data processing and chatbot development
- **Notebook Environment** for code walkthrough (e.g., Jupyter)
- **RAG Model** for retrieval-augmented generation

