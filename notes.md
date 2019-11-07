# Requirements

A client has hired you to track zoo animals.
For each individual animal, you must track that their name, species, and all zoos in which they have resided (including zoo name and address).

Determine the database tables necessary to track this information.

Label any relationships between table.


# zoos
-name
-address

# animals
-name
-species
-list of all the zoos where they have resided

## Good data model

-capture ALL info the system needs
-capture ONLY the infoo the system needs
-reflect reality 
-is flexible, can evolve with the system
-guarantee 'data integrity' without sacrificing too much performance
-is driven by the way we access data

## Components

-emtities (nouns: zoo, animal, species), like a resource --> tables.
-properties -> columns or fields.
-relationships -> Foreign Keys

## Workflow

-Identify the entities
-Identify the relationships
-Identify the properties

## Relationships
-one to one
-one to many: this is the most common!
-many to many: this is smoke and mirrors

_there are many animals in one species_ one species -many animals

_there can be more than one animal in a zoo_

_an animal could have lived in more than one zoo_
## Mantras

-Every table MUST have a PRIMARY KEY. serial for post, intenger for sql
-Work on **two or three entities at a time.
- **one to many realationships are modeled using a **foreign key
-the FORIEGN KEY ALWAYS goes on the MANY side. animals- 1 species, MANY animals
-the foreign key column MUST be the SAME TYPE as the primary key it references
-MANY TO MANY relationships are modeled using a THIRD TABLE
-the THIRD TABLE could include OTHER COLUMNS

