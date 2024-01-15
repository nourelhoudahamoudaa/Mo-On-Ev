# Modular Ontology Evaluation MoOnEv

This implementation aligns with our paper titled "MoonCAB ontology: enrichment using SWRL rules and evaluation with MoOnEv, a new tool for modular ontologies evaluation," which is part of our PhD research.

As there is currently no existing application capable of measuring all ontology evaluation metrics and testing ues cases to evaluate and validate a modular ontology, we have created a novel desktop tool known as Modular Ontology Evaluation (MoOnEv)on Python 3, Tkinter, rdflib, and owlready2. MoOnEv relies on the OMEVA metrics list [Gobin-Rahimbux, B. 2022] (13 criteria proposed by [Khan, Z.C. 2016] and an additional 22 criteria were identified by them), and utilizes SPARQL queries for ontology evaluation, validating SWRL rules through use case testing.

  ### ==> We displays in the images shown below the results of evaluation and validation MoOnEv tool for MoonCAB ontology
- The repository includes the output report of evaluation and validation MoonCAB ontology with MoOnEv tool.
## MoOnEv Interfaces :
### 1) Get start
In the initial interface, the easiest way to begin is by selecting the ontology file with a '.owl' extension.
![startppl](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/e225e070-b40d-4d61-af55-bb54a9d9b381)

### 2) Select Ontology Modules
To streamline the process of tool extraction for module selection, we recommend including the name and IRI of each module in this interface.

![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/4cb42400-60f4-4b24-a2f5-4fb1615beaf6)



### 3) Naming Convention
  The Naming criteria are employed to verify the utilization of naming conventions and ensure name consistency. The metrics in this context indicate the presence of human-readable descriptions within the ontology, which is facilitated by the inclusion of labels and definitions in three languages.
  
![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/e1a7ea92-1525-4b75-b918-db4a729d0068)



### 4) Modules Syntax Evaluation
A higher Syntactic Quality score is desirable as it indicates a well-structured ontology that adheres to language specifications and best practices, making it more usable and maintainable for ontology users and developers.

- #### Lawfulness:
Focuses on assessing the syntactic correctness and adherence to language rules:  ![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/98185127-841c-4487-b823-c615e6cd0aff), where ![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/1a8b5f24-27ef-4a57-b668-368e776ce178)
: Total breached rules and ![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/5ef40f63-05ea-43ed-a1ee-f9fe2e0b1cfd)
: Number of statements in the ontology.
- #### Syntax Richness:
   Evaluates the ontology's expressiveness and completeness in representing the domain of interest:  ![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/359743fb-3e5a-450d-a375-79098a1d7d34)
, where Y: Total syntactical features available in the ontology language and Z: Be the total syntactical features used in the ontology.
- #### Syntactic Quality:
To avoid potential issues that may arise during integration, reasoning, or application of the ontology in various domains: ![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/fa80ed45-3340-4697-94db-7262bfca48ca) .



![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/15cd9cd9-3ae5-4f0f-948f-a65d4f006b71)


### 5) Modules Categorization & Distribution Evaluation
Categorization and Distribution Evaluation assesses how effectively modules within an ontology are organized and distributed. This evaluation ensures efficient ontology performance, ease of maintenance, and scalability.

- #### Class Distribution:
  Checks if related classes are grouped together within the same module and if there is a balanced representation of classes across modules: ![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/f2758198-7f3f-4003-93cd-0bcffc51319d).

- #### Attribute Distribution:
  Ensures that properties associated with specific classes are located in relevant modules, promoting clarity and consistency in the ontology’s structure: ![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/84880013-1597-4262-9735-fcea348147c3).

- #### Relationship Distribution:
  Ensures that relationships are appropriately assigned to relevant modules, avoiding excessive cross-module dependencies and promoting modularity: ![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/b65481ca-df8d-4496-b805-3c1277e06bac).
- #### Module Distribution:
 how various components (classes, attributes, and relation-ships) are distributed across different modules of the ontology: ![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/0ee83176-738d-4f71-b1b8-142ea5aa0fb3).

![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/19203589-5bef-4a00-b122-f92ebe8a15c3)


### 6) Modules Structure Evaluation
![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/6e33f314-dcd1-4050-86fa-3e07f6963198)


### 7) Modules Richness Evaluation
![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/f8e66ee5-e897-45e1-9fb0-b455c49c72cc)


### 8) Logical Criteria Evaluation
![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/41a9777c-b379-4b15-8eb6-3ab1b2efb667)


### 9) Modules Relatedness Evaluation
![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/d65a2131-82af-4925-8476-be2a13380ad7)


### 10) Modules Quality Evaluation
![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/bf7de737-b4d3-4997-877c-71d931c6e8c0)


### 9) Test Use Case
#### 9.1)
![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/46d83b30-7716-492d-82f9-d6f0bdd8c801)

#### 9.2)
![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/1cce83bc-3655-4d0d-8a29-31d2b1f66f7e)

#### 9.3)

### 10) Get Synthesis Report

![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/02adc6a1-bb39-402b-b44b-1da31dd19696)


