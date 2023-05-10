# Relational diagram
## Table of contents
 * [**Introduction**](#introduction)
 * [**Diagram**](#diagram)
 * [**Explanation**](#explanation)

# Introduction
This time we have to create a entity relationship diagram which contains the following requirements:
- Entities
- Attributes, Primary Key
- Roles in recursive relationships.
- (optional) Ternary relationships
- optional) Complex attributes. Composite attributes. Multivalued attributes. Derived attributes.
- All possible cardinalities: one-to-one, one-to-many, many-to-many.
- Total and partial participation.
- Weak entities.
- Generalization-specialization. Overlapping/disjoint. Total/partial.

# Diagram

The image below represents the relationships between entities,entities sets and their attributes:

![image](https://github.com/SPiedra955/er_diagram/assets/114516225/5957ee18-3c47-4227-ad88-3cb78fa52f18)

# Explanation

The diagram starts from the top to the bottom and works in the following way
- ````Hospital```` it's a entity who has attributes like name that can be a composite attribute like is address which contains composite attributes like country,state, city and address(Street).The primary key is ```id_hospital``` that it's underlined like all the primaries keys we are going to found.
- In the right side in color red it's te generalization-specialization in this case is a total because the entity is public or private there is not more alternatives.
- ````Surgeons```` it's a weak entity who depends of Hospital, it's a relationship __one-to-many__ has his attributes and compose ones that it's ````name````.
- ````Speciality```` its a complementary entity set of ````Surgeons```` and has 
