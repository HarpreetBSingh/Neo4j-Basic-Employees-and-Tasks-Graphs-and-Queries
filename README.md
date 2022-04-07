# Neo4j-Basic Employees and Tasks Graphs and Querries
 Using Neo4j, I generated hypothetical data of employees and managers working for a data analyst department for a company. I then generated querries to create relationships and return certain info to show basic knowledge.
## Generating Employee Nodes
CREATE (e1:Employee {Name:"Daniel Mcgee",Age:"35",Sex:"M"})

CREATE (e2:Employee {Name:"Joey Smith",Age:"27",Sex:"M"})

CREATE (e3:Employee {Name:"Paul Carson",Age:"45",Sex:"M"})

CREATE (e4:Employee {Name:"David Pruitt",Age:"43",Sex:"M"})

CREATE (e5:Employee {Name:"Peter Silva",Age:"37",Sex:"M"})

CREATE (e6:Employee {Name:"Andrew Day",Age:"36",Sex:"M"})

CREATE (e7:Employee {Name:"Henry Marks",Age:"29",Sex:"M"})

CREATE (e8:Employee {Name:"Patrick Cruise",Age:"34",Sex:"M"})

CREATE (e9:Employee {Name:"John Freeman",Age:"21",Sex:"M"})

CREATE (e10:Employee {Name:"Michael Schmitt",Age:"47",Sex:"M"})

CREATE (e11:Employee {Name:"Jackie Shaw",Age:"45",Sex:"F"})

CREATE (e12:Employee {Name:"Glenda Collier",Age:"56",Sex:"F"})

CREATE (e13:Employee {Name:"June Russell",Age:"33",Sex:"F"})

CREATE (e14:Employee {Name:"April Lozano",Age:"22",Sex:"F"})

CREATE (e15:Employee {Name:"May Cooper",Age:"25",Sex:"F"})

CREATE (e16:Employee {Name:"Betty Moss",Age:"29",Sex:"F"})

CREATE (e17:Employee {Name:"Faye Moss",Age:"57",Sex:"F"})

CREATE (e18:Employee {Name:"Claudette Stone",Age:"48",Sex:"F"})

CREATE (e19:Employee {Name:"Evelyn Cheryl",Age:"27",Sex:"F"})

CREATE (e20:Employee {Name:"Leigh Glass",Age:"46",Sex:"F"})
![image](https://user-images.githubusercontent.com/99159437/162141866-4601fb0b-98fe-4ff6-a04c-2ac53ec48575.png)

## Generating Task Nodes
CREATE (t1:Task {Type: "Data Cleaning"})

CREATE (t2:Task {Type: "Data Visualization"})

CREATE (t3:Task {Type: "Model Development"})

CREATE (t4:Task {Type: "Data Collection"})

CREATE (t5:Task {Type: "Generating Reports"})

CREATE (t6:Task {Type: "Maintaining Databases"})

CREATE (t7:Task {Type: "Software Development"})

CREATE (t8:Task {Type: "Stakeholder Communication"})

CREATE (t9:Task {Type: "Data Processing"})

![image](https://user-images.githubusercontent.com/99159437/162142423-0d9a63f7-427f-49ce-b06d-b3f8e3aa3528.png)
