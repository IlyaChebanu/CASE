Methodologies
Object Oriented Development
  Suited to process oriented systems implemented in OO environment
  “systems that are strongly database-oriented……are not ideally suited to object oriented development”
   Requires high level of expertise
   Often used for customisable packages (e.g. SAP)
RAD
  Iterative development
  Process and user expectations must be carefully handled
  Can be used in conjunction with Structured Methods
  Particularly suited to small projects and user interface development
  DSDM

Structured Systems Analysis & Design Method (SSADM)
  Each of the three system models provides a different viewpoint of the same system, 
  each of which are required to form a complete model of the system. 
  Within SSADM, each of the three techniques is cross-referenced against the others to ensure the completeness and accuracy 
  of the complete model.

  The Data/Structure View: 
    - a description of all the data and information the system uses (gained from the DFDs above)
  The Process View:
    - a description of all the processes or actions carried out by the system (taken from the process descriptions and the 
      process catalogue)
  The Event/Time View:
    - a description of the systems events, that is the 'triggers' that set processes running (from the Entity life histories)
  
  Taking these different views allows us to gain much more information about the system than we could have done otherwise.
__________________________________________________

Business Activity Modelling
  Network of activities
  Pictorial representation of the business.
  Purpose:
    - Helps pick out the requirements, focus on the areas of concern. 
    - Puts the system in perspective, helps to inform the client what is possible.
    - It can increase user participation and encourage users to build a sense of ownership for the future system.
    - Defines what and when of the business activity.
    
Work Practice Modelling
  Purpose:
    - Defines who, where, how, and (maybe) why of the business activity. 
    -  responsibilities to humans.
    Products include: User Catalogue, Task Models, Task Scenarios, and User Roles.
  
Hierarchical Task Model
  The arrangement of the activties/tasks (from the BAM) in a hierarchy.
  Purpose:
    - Validating Task Models.
    
User Catalogue
  Documenting job title and business activities of each jobholder (user). A summary of the Work Practice Model arranged by 
  job title.
  Purpose:
    - Identify relevenat jobholders (users)
    - Define the outward appearance of the new system.
   Coloumns: Job Title, Responsibility (Job Activity)
   
   
______________________________________________________

Logical Data Modelling
  Logical Data Model
    Vehicle for analysising the logical structure of an organisation's information.
    Graphical representation of information, its relations to other information and business concepts.
    Consists of:
      - Logical Data Structure (LDS)
      - Textual description explaining all parts of the LDS
   Validating LDM:
    LDM must provide access to all data items required by each update or enquiry process.
      
  Entity
    EXAMPLE
    Entity Type:           Occurances/Attributes:
     Supplier               Supplier No
                            Supplier Name
                            Supplier Address
    Must be occurances > 1
    Occurances of that entity must be unqiuely identifiable.
    
      Relationships
      (m:n) - ><
      (1:m) - -<
      (1:1) - ___Has each process a strong imperative verb and object?
        Redundant Relationships:
          Unnecessary relationships.
          Explain how M:N, 1:1 and redundant relationships can be removed from an LDS and
          update your LDS from 1(a) to reflect this. ????
        Reflexive Relationship:
          1:1
          example: Pig's Ear, Product (entity) 'substitution'
      
      example of optionality (dash): supplier ----< pruchase order
______________________________________________________

Data FLow Diagrams
  Validating Data Flow Diagrams:
    - Has each process a strong imperative verb and object?
    - Are the input data flows related to the output data flows?
    - Can the flows be reduced?
    - Have all data stores flows in and out?
    - Are symbols correctly labelled and uniquely referenced?
    - Do external entities communicate with at least one process?
    - Does the user think that it is an accurate portrayal of the business area?
    
Document Flow Diagram
    Purpose:
     - Illustrates the flow of physical documents associated with the area being investigated. 
    Process (5 steps):
      - Identify recipients and sources of documents (inside or outside boundry).
      - Identify documents which connect recipient and source.
      - Convert each source and recipient into an external entity symbol.
      - Add data flow to represent each connecting document.
      - Add system boundary (exclude external entities found in context diagram).
      - Are the input data flows related to the output data flows?
______________________________________________________

Entity Life History
  Puropose:
   Analysis - to show the consideration of the occurances of the entity (updates and current states)
   Design - program specification