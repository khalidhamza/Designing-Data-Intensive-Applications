# Chapter 2
This chapter explores the evolution of data models, comparing relational and document models, and delves into the rise of NoSQL, graph-like data models, and query languages.

## Relational Model Versus Document Mode
### Relational model
Relational model introduced by Edgar Codd in 1970, organizes data into tables (relations) with rows and columns. It emphasizes structured data and relationships enforced through foreign keys.

### Document model
Document model (used in NoSQL databases like MongoDB) stores data in flexible, semi-structured formats like JSON or XML. It is schema-on-read, allowing for more flexibility in data representation.

## The Birth of NoSQL
NoSQL databases emerged in the late 2000s to address scalability, flexibility, and performance issues in relational databases. They were designed for distributed systems, large-scale data, and unstructured or semi-structured data.

## The Object-Relational Mismatch
- Relational databases often struggle to represent complex object hierarchies from application code, leading to an "impedance mismatch." ORMs (Object-Relational Mappers) help bridge this gap but add complexity.
- Document databases align more closely with object-oriented programming, as they can store nested structures directly.

## Many-to-One and Many-to-Many Relationships
- Relational databases excel at handling many-to-one and many-to-many relationships using joins.
- Document databases can struggle with these relationships, often requiring application-level logic to resolve them.

## Are Document Databases Repeating History?
Document databases resemble the hierarchical model (e.g., XML, JSON), which was popular before relational databases. However, they address some limitations of the hierarchical model by allowing more flexible schemas.

### The network mode
- The network model (pre-relational) represented data as a graph of records connected by pointers. It was complex and rigid.

### The relational model
- The relational model simplified data representation by using tables and declarative queries, making it easier to work with.

### Comparison to document databases
- Document databases are more flexible for unstructured or semi-structured data, while relational databases enforce stricter schemas and relationships.
- Relational databases are better suited for complex queries involving joins and transactions.

## Relational Versus Document Databases Today
- Relational databases remain dominant for transactional systems and complex queries.
- Document databases are popular for use cases requiring schema flexibility, scalability, and fast iteration.

### Which data model leads to simpler application code?
- Document databases can simplify code for hierarchical or nested data structures.
- Relational databases are better for complex relationships and queries.

### Schema flexibility in the document model
- Document databases allow for schema-on-read, meaning the schema is interpreted at runtime. This is useful for evolving data structures but can lead to inconsistencies.

### Data locality for queries
- Document databases store related data together (e.g., a user profile and its nested data), which can improve query performance by reducing the need for joins.

### Convergence of document and relational databases
- Some relational databases now support JSON and schema flexibility, while some document databases are adding relational features like joins.

## Query Languages for Data
- Query languages can be declarative (e.g., SQL) or imperative (e.g., MapReduce). Declarative languages are often more concise and easier to optimize.

## Declarative Queries on the Web
- Declarative languages like CSS and XPath are used to query web documents, demonstrating the power of declarative approaches.

## MapReduce Querying
- MapReduce is a programming model for processing large datasets in distributed systems. It is powerful but low-level compared to declarative query languages.

## Graph-Like Data Models
- Graph models are ideal for data with complex relationships, such as social networks or recommendation systems.

## Property Graphs
- Property graphs consist of nodes (entities) and edges (relationships), both of which can have properties (key-value pairs).

## The Cypher Query Language
- Cypher is a declarative query language for property graphs, used in databases like Neo4j.

## Graph Queries in SQL
- SQL can represent graph queries using recursive common table expressions (CTEs), but it is less intuitive than graph-specific languages.

## Triple-Stores and SPARQL
- Triple-stores store data as subject-predicate-object triples (e.g., RDF). SPARQL is a query language for triple-stores.

### The semantic web
- The semantic web aims to make web data machine-readable using standards like RDF and SPARQL.

### The RDF data model
- RDF (Resource Description Framework) represents data as triples, enabling interoperability across systems.

### The SPARQL query language
- SPARQL is a declarative query language for RDF data, similar to SQL for relational databases.

## The Foundation: Datalog
- Datalog is a declarative logic-based query language that serves as the foundation for many graph and semantic web query languages.



> - The choice of data model depends on the application's requirements: relational for structured data and complex relationships, document for flexibility and nested data, and graph for highly interconnected data.
> - Query languages play a critical role in how data is accessed and manipulated, with declarative languages offering simplicity and optimization benefits.
> - The evolution of data models reflects a trade-off between flexibility, scalability, and complexity, with ongoing convergence between relational and non-relational systems.

