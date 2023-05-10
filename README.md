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

The diagram starts from the top down and works as follows
- ````Hospital```` is an entity that has attributes like name which can be a composite attribute like __address__ which contains composite attributes __like country, state, city and street address__. The primary key is ``id_hospital`` which is underlined like all the primary keys we will find, its relationship is __one-to_many__ a __Hospital__ has several surgeons and the surgeons work for a __Hospital__.
- On the right side in red is the __generalization-specialization__ in this case it is a __total-disjoint__ because the entity is public or private there are no other alternatives.
- ````Surgeons```` is a weak entity that depends on __Hospital__, it is a __many-to-one__ relationship because several surgeons can have the same speciality and normally a surgeon is usually specialised in a certain type of surgery and works in this or related positions, e.g. a surgeon specialised in heart surgery.
- ````Speciality```` is a complementary entity to ````Surgeons````. The primary key has roles depending on the speciality we need a __prerequisite__.e.g. A surgeon needs a university degree.
- ````Patient```` is an entity with a relationship __many-to_many__ a surgeon has several patients and vice versa e.g. it is not the same surgeon for a transplant and a rhinoplasty, the participation is total because a patient must have a surgeon assigned and there is also an attribute __multivalued__ which is phone_number e.g. a patient can have different numbers associated to it.A __derived values__ like __age__
- ````Medical history```` is a weak entity and depends of the entity patient, a set of relationships called __register__ with an attribute which is __date__ this data stores the date of the patient's last surgery. The relationship is __one-to-one__ a patient only has one medical history and the medical history belongs to one patient.
