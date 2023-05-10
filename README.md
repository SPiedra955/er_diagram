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
- ````Hospital```` it's a entity who has attributes like name that can be a composite attribute like is __address__ which contains composite attributes like country,state, city and address(Street).The primary key is ```id_hospital``` that it's underlined like all the primaries keys we are going to found, his relationship is __one-to_many__ a __Hospital__ have various surgeons and the surgeons works for one Hospital.
- In the right side in color red it's the __generalization-specialization__ in this case is a total because the entity is public or private there is not more alternatives.
- ````Surgeons```` it's a weak entity who depends of __Hospital__, it's a relationship __many-to-one__ because various surgeons can have the same speciality and normally a surgeon normally it's specialize in a determinated type of surgeries and works in it or related charges .e.g. A surgeon specialize in heart surgeries.
- ````Speciality```` its a complementary entity of ````Surgeons````. The primary key has roles depending on the speciality we need a prerequierement.e.g. A surgeon needs a university carreer.
- ````Patient```` is a entity with a relation __many-to_many__ a surgeons has various patients and in reverse e.g. it's not the same surgeon for a transplant and rinoplastia, the participation is total because a patient must have assigned a surgeon also there is a __multivalued attribute__ that is phone_number e.g a patient can have differents numbers associated.
- ````Medical history```` is a weak entity with a relationship set called __register__ with one attribute thats is __date__ this data stores the date of the last sirurgy of the patient.The relation is __one-to-one__ a patient only has one medical history and reverse.


The diagram starts from the top down and works as follows
- ````Hospital```` is an entity that has attributes like name which can be a composite attribute like __address__ which contains composite attributes like country, state, city and street address. The primary key is ``id_hospital`` which is underlined like all the primary keys we will find, its relationship is __one-to_many__ a __Hospital__ has several surgeons and the surgeons work for a Hospital.
- On the right side in red is the __generalization-specialization__ in this case it is a total because the entity is public or private there are no other alternatives.
- ````Surgeons```` is a weak entity that depends on __Hospital__, it is a __many-to-one__ relationship because several surgeons can have the same speciality and normally a surgeon is usually specialised in a certain type of surgery and works in this or related positions, e.g. a surgeon specialised in heart surgery.
- ````Speciality```` is a complementary entity to ````Surgeons````. The primary key has roles depending on the speciality we need a prerequisite.e.g. A surgeon needs a university degree.
- ````Patient```` is an entity with a relationship __many-to_many__ a surgeon has several patients and vice versa e.g. it is not the same surgeon for a transplant and a rhinoplasty, the participation is total because a patient must have a surgeon assigned and there is also an attribute __multivalued__ which is phone_number e.g. a patient can have different numbers associated to it.
- ````Medical history```` is a weak entity with a set of relationships called __register__ with an attribute which is __date__ this data stores the date of the patient's last surgery. The relationship is __one-to-one__ a patient only has one medical history and the medical history belongs to one patient.
