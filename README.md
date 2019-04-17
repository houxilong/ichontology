# ICHontology
A knowledge ontology for Intangible Cultural Heriteg(ICH).
The ontlogy was designed based on the FOAF, GeoNames, Relationship, DC. The knowledge ontology contains 10 classes, together with 26 object properties and 27 data properties. The classes of the ontology primarily includes _Items_, _Agent_, _Place_ , _Category_, _Batch_ and _Level_.
## The prefix
prefix | URI
-|-
foaf|http://xmlns.com/foaf/0.1/
rel|http://purl.org/vocab/relationship/
ich(custom)|http://www.ich.cn/ontology/
dc|http://purl.org/dc/elements/1.1/
dct|http://purl.org/dc/terms/
## The object properties
| Object Property| Domain | Range | Explanation |
-|-|-|-
ich:hasInheritor|ich:Items|foaf:Agent|an item's inheritor
ich:isInheritorOf|foaf:Agent|ich:Items| the inheritor of an item
ich:hasType|ich:Items|ich:Category| the item's category
rel:mentorOf|foaf:Person|foaf:Person|A person who serves as a trusted counselor or teacher to this person.
rel:apprenticeTo|foaf:Person|foaf:Person|A person to whom this person serves as a trusted counselor or teacher.'
rel:parentOf|foaf:Person|foaf:Person|A person who has given birth to or nurtured and raised this person.
rel:childOf|foaf:Person|foaf:Person|A person who was given birth to or nurtured and raised by this person.
rel:influencedBy|foaf:Person|foaf:Person|A person who has influenced this person.
foaf:member|foaf:Organization|foaf:Person|Indicates a member of a Group.
ich:hasPlace|ich:Item|ich:Place| The location of the item.
ich:certificationLevel|ich:Item ich:Person|ich:Level| "National - provincial - city - county" level
ich:batch|ich:Item ich:Person|ich:Batch|The batches included in the list, such as the first batch, the second batch, etc.

## The data properties
The data properties are defined according to internationan metadata standards.

## Visualization of Ontology Structure

![OntoGrf-protege](https://raw.githubusercontent.com/houxilong/ichontology/master/OntoGraf.png)
