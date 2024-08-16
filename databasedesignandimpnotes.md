# Database Design & Implementation

## Database Systems
DBMS (Database Management System): A suite of tools for efficiently creating, managing, and persisting large amounts of data. Examples include Google, Yahoo, and Amazon.
Database: A collection of data managed by a DBMS.

## Functions of a DBMS:
Create and specify database schemas.
Query data.
Store large amounts of data.
Ensure durability and recovery from failures.
Control multi-user data access without partial or incomplete actions.

## DBMS Components:
Storage: Data storage manager.
Memory: Buffer manager and buffers.
Indexing: Index/file/record manager.
Execution: Logging, recovery, concurrency control.
User/Application Interaction: Query compiler, transaction manager.
Data Administration: DDL compiler.
Metadata: Data about data (e.g., data inception).
DDL (Data Definition Language): Language for defining database schemas.

## Data Models:
Mathematical Representation: Examples include relational models (tables) and semi-structured models (trees/graphs).
Operations: Query, modification, and defining constraints.
Sources of Data:
File Systems Based: Record-based.
Database Systems Based: Structured, semi-structured, and unstructured data.
Newer Forms: Web-based, dynamic data.

## Data Types:
Structured Data: Formatted and largely numeric.
Semi-Structured Data: Partially structured, with some variability.
Unstructured Data: Minimal structure, such as text documents.

## Database Design Process:
Idea Generation: Ideas -> High-Level Design -> Relational DB Schema -> Relational DBMS.
Problem-Solving: Problems -> Data -> Digital World -> Data Models -> Physical Design.
Understanding Domain: Identify objects, classes, instances, trees, and entities.

## ER (Entity-Relationship) Models:
Discover Entities: Identify nouns in the problem domain.
Identify Attributes: Discover the attributes of each entity.
Establish Relationships: Determine relationships between entities.
Refine Design: Repeat steps until the design is perfect.

## ER Design Principles:
Reflect reality, avoid redundancy, and maintain simplicity.
Limit the use of weak entity sets and avoid unnecessary elements.
Entity sets should have meaningful attributes and relationships.

## ER Diagram Components:
Entities: E.g., Customer, Store.
Attributes: E.g., Name, Location.
Relationships: E.g., One-to-Many, Many-to-Many.

## Constraints:
Unique Constraint: Ensures unique values in a column.
Null/Not Null Constraint: Specifies if an attribute must have a value.
Check Constraint: Ensures attribute values meet specific conditions.
Foreign Key: Attribute that refers to a key in another relation.

## Subqueries:
Queries within queries are used for complex data retrieval.

## ER to Relational Model Conversion:
Strong Entities: Create relations with identifiers as keys.
Relationships:
1:1 Relationship: Add a foreign key to either entity.
1 Relationship: Add a foreign key to the entity on the many side.
M Relationship: Create a new relation with keys from both entities.
Attributes on Relationship: Include attributes in the relationship table.
Recursive Relationship: Handle self-referencing keys appropriately.
