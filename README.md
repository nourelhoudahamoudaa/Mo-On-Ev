# Modular Ontology Evaluation MoOnEv

This implementation follows the our paper "MoonCAB ontology: enrichment using SWRL rules and evaluation with  MoOnEv, a new tool for modular ontologies evaluation."

As there is currently no existing application capable of measuring all ontology evaluation metrics, we have created a novel desktop tool known as Modular Ontology Evaluation (MoOnEv).on Python 3, Tkinter, rdflib, and owlready2. MoOnEv relies on the OMEVA metrics list [Gobin-Rahimbux, B. 2022] and utilizes SPARQL queries for ontology evaluation, validating SWRL rules through use case testing.
  
- OMEVA metrics list: Composed from 13 criteria proposed by [Khan, Z.C. 2016] and an additional 22 criteria were identified by [Gobin-Rahimbux, B. 2022]. The list of criteria is classified into eight categories, as shown in table :


![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/648e00fa-ce69-43cd-8e74-ebc5019cad87)



## MoOnEv Interfaces :
### 1) Start
![startppl](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/e225e070-b40d-4d61-af55-bb54a9d9b381)

### 2) Select Ontology Modules
To streamline the process of tool extraction for module selection, we recommend including the name and IRI of each module in this interface.

![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/4cb42400-60f4-4b24-a2f5-4fb1615beaf6)



### 3) Naming Convention
  The Naming criteria are employed to verify the utilization of naming conventions and ensure name consistency. The metrics in this context indicate the presence of human-readable descriptions within the ontology, which is facilitated by the inclusion of labels and definitions in three languages.
  
![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/e1a7ea92-1525-4b75-b918-db4a729d0068)



### 4) Modules Syntax Evaluation
A higher Syntactic Quality score is desirable as it indicates a well-structured ontology that adheres to language specifications and best practices, making it more usable and maintainable for ontology users and developers.

![image](https://github.com/nourelhoudahamoudaa/Mo-On-Ev/assets/48714413/15cd9cd9-3ae5-4f0f-948f-a65d4f006b71)


### 5) Modules Categorization & Distribution Evaluation
Categorization and Distribution Evaluation assesses how effectively modules within an ontology are organized and distributed. This evaluation ensures efficient ontology performance, ease of maintenance, and scalability.

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


