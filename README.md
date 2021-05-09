# **WP3: Semantic skillmatching in Open Source Hardware (OSH) Project Communites**

- This repository handles the third workpackage (WP3) of the OPEN!NEXT project to serve possible solutions for Open Source Hardware Commmunity needs.
- Skillmatching as a measure of community management was identified, which is the main focus here.
<br> For this, a generic ontology model of a possible open souce hardware project landscape was developed. 
<br> The implementation of the ontology took results from a previous project (OPEN!) into account that also analysed processes and dynamics of OSH community.
- Purpose of the ontology model is to fulfill the concepted user stories (US) defined below.


## **USER STORIES (US)**

- Two main US are scope of the case: <br>
 1. I, as a user of some OSH management platform, am interested in learning some skill (or want to help and can provide a certain skill) and want to find projects with issues where this is addressed. <br>
 2. I, as project manager/member, need help to do a task requirering a certain skill and want to find people to help me or do the task. 

## **CURRENT STATUS**

- Currently the ontology model is the first draft and has to be validated with OSH project data.
- Afterwards possible adaptions will taken into account.
- The repository will be updated respectively over time.


## **ONTOLOGY MODEL**

For customization reasons, the ontology model consists of three ontologies referring to each other but are therefore replacable necessary:<br>
1. Open source hardware product development (OSHPD) ontology
   - This OWL ontology holds the architecture and semantic restrictions of the project landscape
   - Main classes for the skillmatching case are "Person", "Project", "Task" and "Skill", that are related through properties.
   - Property restrictions arise from the use cases before mentioned
   - The OSHPD ontology imports the skill ontology

2. Skill ontology
   - This OWL ontology is based on the ESCO skill hierarchy
   - The ESCO hierarchy was cropped to the topics of mechanics, electrics/electronics, furniture and cars/mobiliy.
   - Afterwards a reclustering was done for ease of use purposes
   - The skill ontology is still to be validated with OSH project data

3. Instantiation file
   - This file holds needed project data of the individuals
   - The file refers to and uses class and property expressions from the other two ontologies.

## ONTOLOGY RESTRICTIONS
- Based on the US, prevalidation workshops were held. The results specified the scope and functionality that is to be implemented:<br>
  - I, as a person/user/contributor, add my skills to my profile to show others
  - I recieve notifications of invitations/open calls matching my skills
  - I recieve notifications or suggestions for projects with people with whom I have already worked on. <br> This specifically does not contain to the skill matching focus but is often mentioned. This interpreted indicates a need for priorisation of the skill matching (e.g. a first suggestions for a match will be from the circle of acquaintances rather than the whole community).


## **INSTRUCTIONS TO USE**
- The ontologies are provided publicly here on the repository and therefore can be referenced by their namespaces.
- If you want to use them locally, do not forget to rereference them by chaning their namespaces to the new location (file path or URL).

## **CODE**
- Code to handle, instantiate, query and reason the ontology model is in development (in coordination with other project parties) and will be uploaded soon.

