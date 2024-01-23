# Modular Ontology Evaluation MoOnEv

This implementation aligns with our paper titled "MoonCAB ontology: enrichment using SWRL rules and evaluation with MoOnEv, a new tool for modular ontologies evaluation".

As there is currently no existing application capable of measuring all ontology evaluation metrics and testing ues cases to evaluate and validate a modular ontology, we have created a novel desktop tool known as Modular Ontology Evaluation (MoOnEv) with Python 3, Tkinter, rdflib, and owlready2. MoOnEv relies on the OMEVA metrics list [Gobin-Rahimbux, B. 2022] (13 criteria proposed by [Khan, Z.C. 2016] and an additional 22 criteria were identified by them), and utilizes SPARQL queries for ontology evaluation, validating SWRL rules through use case testing.

  ### ==> We displays in the images shown below the results of evaluation and validation MoOnEv tool for our MoonCAB ontology.
- The repository includes the output report of evaluation and validation MoonCAB ontology with MoOnEv tool.
## MoOnEv Interfaces :
### 1) Get start
In the initial interface, the easiest way to begin is by selecting the ontology file with a '.owl' extension.
![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/6030e097-2bc7-48dc-a064-cd4e8c7e2b2f)

### 2) Select Ontology Modules
To streamline the process of tool extraction for module selection, we recommend including the name and IRI of each module in this interface.

![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/4cb42400-60f4-4b24-a2f5-4fb1615beaf6)



### 3) Naming Convention
  The Naming criteria are employed to verify the utilization of naming conventions and ensure name consistency. The metrics in this context indicate the presence of human-readable descriptions within the ontology, which is facilitated by the inclusion of labels and definitions in three languages.
  
![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/1b788830-1128-48ef-a0d4-aa763c45609d)



### 4) Modules Syntax Evaluation
A higher Syntactic Quality score is desirable as it indicates a well-structured ontology that adheres to language specifications and best practices, making it more usable and maintainable for ontology users and developers.

- #### Lawfulness:
Focuses on assessing the syntactic correctness and adherence to language rules:  ![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/98185127-841c-4487-b823-c615e6cd0aff), where ![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/1a8b5f24-27ef-4a57-b668-368e776ce178)
: Total breached rules and ![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/5ef40f63-05ea-43ed-a1ee-f9fe2e0b1cfd)
: Number of statements in the ontology.
- #### Syntax Richness:
   Evaluates the ontology's expressiveness and completeness in representing the domain of interest:  ![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/359743fb-3e5a-450d-a375-79098a1d7d34), where Y: Total syntactical features available in the ontology language and Z: Be the total syntactical features used in the ontology.
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
 How various components (classes, attributes, and relation-ships) are distributed across different modules of the ontology: ![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/0ee83176-738d-4f71-b1b8-142ea5aa0fb3).

![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/19203589-5bef-4a00-b122-f92ebe8a15c3)


### 6) Modules Structure Evaluation
These metrics assess the quantitative and qualitative aspects of module structure, providing a comprehensive evaluation of its composition and complexity.
 
- #### Size of Module:
Provides a simple measure of the module's content and the amount of knowledge it represents: ![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/14cd02b0-477a-41b9-8a61-18a31299b5c9), where C: Named class/individuals, P: Its properties 
- #### Relative Size:
Indicates the proportion of the original ontology covered by the module: ![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/a53957b1-2ca7-4d82-8b60-0cc369d7e696).  
- #### Atomic Size:
Helps identify the complexity of tightly connected axioms within the module: ![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/7a67ec6c-01eb-4ca2-956d-c81deec86007), where Atom: Group of interdependent axioms.   
- #### Depth of Module:
  Measures the hierarchical depth of the ontology within the module: ![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/d78bd00d-1b4f-45d8-80ae-7d8c782e33d2)
- #### Average Depth on inheritance Tree:
  Quantifies the average depth of the class hierarchy within the module:  ![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/63dca925-c041-4fbf-952d-fb529d3a610b)
- #### Breadth of Module:
  Provides insights into the diversity of concepts represented by understanding the number of sibling classes within the module.
- #### Module Density:
  Evaluates the ontology's density by assessing how well-connected the entities:
  - Class Density: ![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/0b04badb-8bd7-45d0-8129-d35ce215fcee)
  - Edge Node Ration: ![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/20b9ffda-d358-4970-8c66-4541245ad862), where E: edges and C: classes.
- #### Overall Complexity of Module:
  Is introduced as a means to quantitatively measure the complexity of the module:
 - Tree Impurity:![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/8790e4f9-cc54-4931-b784-4c662f933d93)
 - Entropy of ontology Module:  ![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/ebb564c5-4ffe-45e0-a618-419d3427b5b6),
 - Overall complexity: ![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/e4059d01-3500-4e2c-b2e1-b0c3d4653c8a)
![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/be37af64-6310-4f3c-bd50-7b6c0cce2e2d)


![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/6e33f314-dcd1-4050-86fa-3e07f6963198)


### 7) Modules Richness Evaluation
This category of metrics assesses the amount of relational information in relation to classes within the module.
- #### Attribute Richness:
Measures the diversity of attributes in a class, contributing to ontology quality: ![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/e1cd57f5-4342-4e0f-806a-54004de08069) .
- #### Inheritance Richness:
Indicates a structured hierarchy of classes for effective knowledge representation: ![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/c001ab5c-52ce-4159-ac6f-4f3a3d510d97) .
- #### Relationship Richness:
Reflects the use of non-inheritance relationships, enhancing ontology interconnectedness and expressiveness: ![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/b693e15a-dab8-41d3-988e-8130fc4c2873).


![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/f8e66ee5-e897-45e1-9fb0-b455c49c72cc)


### 8) Logical Criteria Evaluation

- #### Correctness of Module: 
Measures how well the module aligns with the source ontology: 
![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/6fbdcc23-c167-4ed6-a13b-09a32265e5ea)

- #### Completeness of Module: 
Assesses whether the module’s ax- ioms are semantically equivalent to those in the source ontology: 
![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/b4c69df7-3ab7-41fb-8e6e-47daebc72a6f)


![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/41a9777c-b379-4b15-8eb6-3ab1b2efb667)


### 9) Modules Relatedness Evaluation
This category evaluates relationships between modules. It includes metrics like Inter-Module Distance and Intra-Module Distance, measuring the number of modules required and the distance between entities within a module. Additional criteria, such as Relative Intra-Module Distance, Encapsulation, Redundancy, and Independence, provide insights into the connections, duplication, and self-sufficiency of modules.

- #### Inter-module Distance:
Suggests strong interconnections and potential dependencies among entities that frequently appear together in different modules.
- #### Intra-module Distance:
Indicates high cohesion and relatedness among entities that frequently appear together within the same module.
- #### Relative Intra-module Distance:
Highlights potential structural differences or adjustments between the module and the source based on significant differences in intra-module distances.
- #### Encapsulation:
Evaluates the degree of sharing and reuse of axioms between the module and other interconnected modules.
- #### Redundancy:
Identifies instances of duplicated information in multiple modules, promoting efficiency and consistency by reducing redundancy. 
- #### Independence:
Assesses the module’s self-sufficiency and potential for standalone use in various contexts, enhancing reusability and flexibility.

![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/338adc1c-0395-4fe2-bb4e-94a1f1a6bca9)


### 10) Modules Quality Evaluation
These metrics assesses ontology modules through Precision and Recall for taxonomical relations alignment, Cohesion for interrelation degree, and Coupling, examining disconnected classes. Module Overall Quality considers size and redundancy indicators for a comprehensive evaluation of module structure.

- #### Precision:
Ensures that the module accurately captures hierarchical relationships from the parent ontology, avoiding any additional or conflicting relationships.
- #### Recall:
Ensures that the module includes all the necessary information and concepts from the parent ontology, leaving no gaps or omissions.
- #### Module cohesion:
High cohesion indicates that the entities in the module are closely related, forming a coherent and well-organized set of knowledge.
- #### Module Coupling:
Metrics like the Number of Separated Hierarchical Relations and Non-Hierarchical Relations quantify the extent of coupling in the module.
- #### Module Overall Quality:
Size indicator assesses the module’s size, while the redundancy indicator identifies duplicated information in the module.

![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/9ad8883a-8342-46dc-846e-28cd619b4e8b)


### 9) Test Use Case
#### 9.1) Add individuals step
![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/90a5e6d5-0cca-4451-8a97-abdc32f99820)

#### 9.2) Add properties step
![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/cee37b4b-ed4f-4eed-a5a9-3bb59261b5b8)

#### 9.3) Apply SWRL rules step

![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/a86b7e97-3026-44b7-b864-6aa31cc804e0)



### 10) Get Synthesis Report
![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/a6b53a12-d779-4f25-8a86-e5449a27ace5)

![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/02adc6a1-bb39-402b-b44b-1da31dd19696)


