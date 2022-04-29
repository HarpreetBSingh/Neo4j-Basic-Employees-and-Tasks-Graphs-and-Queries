# Neo4j-Basic Employees and Tasks Graphs and Queries
 Using Neo4j, I generated hypothetical data of employees and managers working for a data analyst department for a company. I then generated querries to create relationships and return certain info to show basic knowledge.
## Generating Employee Nodes
CREATE (e1: Employee {Name:"Daniel Mcgee",Age:"35",Sex:"M"})

CREATE (e2: Employee {Name:"Joey Smith",Age:"27",Sex:"M"})

CREATE (e3: Employee {Name:"Paul Carson",Age:"45",Sex:"M"})

CREATE (e4: Employee {Name:"David Pruitt",Age:"43",Sex:"M"})

CREATE (e5: Employee {Name:"Peter Silva",Age:"37",Sex:"M"})

CREATE (e6: Employee {Name:"Andrew Day",Age:"36",Sex:"M"})

CREATE (e7: Employee {Name:"Henry Marks",Age:"29",Sex:"M"})

CREATE (e8: Employee {Name:"Patrick Cruise",Age:"34",Sex:"M"})

CREATE (e9: Employee {Name:"John Freeman",Age:"21",Sex:"M"})

CREATE (e10: Employee {Name:"Michael Schmitt",Age:"47",Sex:"M"})

CREATE (e11: Employee {Name:"Jackie Shaw",Age:"45",Sex:"F"})

CREATE (e12: Employee {Name:"Glenda Collier",Age:"56",Sex:"F"})

CREATE (e13: Employee {Name:"June Russell",Age:"33",Sex:"F"})

CREATE (e14: Employee {Name:"April Lozano",Age:"22",Sex:"F"})

CREATE (e15: Employee {Name:"May Cooper",Age:"25",Sex:"F"})

CREATE (e16: Employee {Name:"Betty Moss",Age:"29",Sex:"F"})

CREATE (e17: Employee {Name:"Faye Moss",Age:"57",Sex:"F"})

CREATE (e18: Employee {Name:"Claudette Stone",Age:"48",Sex:"F"})

CREATE (e19: Employee {Name:"Evelyn Cheryl",Age:"27",Sex:"F"})

CREATE (e20: Employee {Name:"Leigh Glass",Age:"46",Sex:"F"})

![image](https://user-images.githubusercontent.com/99159437/162147781-21c76060-eca3-4742-abe3-b28bc0158b69.png)


## Generating Task Nodes
CREATE (t1: Task {Type: "Data Cleaning"})

CREATE (t2: Task {Type: "Data Visualization"})

CREATE (t3: Task {Type: "Model Development"})

CREATE (t4: Task {Type: "Data Collection"})

CREATE (t5: Task {Type: "Generating Reports"})

CREATE (t6: Task {Type: "Maintaining Databases"})

CREATE (t7: Task {Type: "Software Development"})

CREATE (t8: Task {Type: "Stakeholder Communication"})

CREATE (t9: Task {Type: "Data Processing"})

![image](https://user-images.githubusercontent.com/99159437/162147899-3002fa0e-e5a0-43e0-8991-f7ab85440567.png)


## Generating Manager Nodes
CREATE (m1: Manager {Name:"Jerry Jones",Age:"57",Sex:"M", Specialty:"Data Analyst"})

CREATE (m2: Manager {Name:"Caroline Susan",Age:"45",Sex:"M",Specialty:"Business Analyst"})

CREATE (m3: Manager {Name:"Cathlyn Lin",Age:"55",Sex:"F",Specialty:"Data Analyst"})

CREATE (m4: Manager {Name:"Vanessa Teymori",Age:"42",Sex:"F",Specialty:" Business Analyst"})

![image](https://user-images.githubusercontent.com/99159437/162148008-24748c43-adc8-499b-8501-b43012d35868.png)

## Generating Relationships
### Now we must generate relationships to show the connections between all these nodes. This is assigning tasks to employees and which managers will lead which tasks.
CREATE (e1) – [:Has_Task] -> (t2)

CREATE (e2) – [:Has_Task] -> (t2)

CREATE (e3) – [:Has_Task] -> (t2)

CREATE (e4) – [:Has_Task] -> (t2)

CREATE (e5) – [:Has_Task] -> (t2)

CREATE (e11) – [:Has_Task] -> (t2)

CREATE (e12) – [:Has_Task] -> (t2)

CREATE (e13) – [:Has_Task] -> (t2)

CREATE (e14) – [:Has_Task] -> (t2)

CREATE (e15) – [:Has_Task] -> (t2)

CREATE (e1) – [:Has_Task] -> (t1)

CREATE (e2) – [:Has_Task] -> (t1)

CREATE (e3) – [:Has_Task] -> (t1)

CREATE (e4) – [:Has_Task] -> (t1)

CREATE (e5) – [:Has_Task] -> (t1)

CREATE (e11) – [:Has_Task] -> (t1)

CREATE (e12) – [:Has_Task] -> (t1)

CREATE (e13) – [:Has_Task] -> (t1)

CREATE (e14) – [:Has_Task] -> (t1)

CREATE (e15) – [:Has_Task] -> (t1)

CREATE (e1) – [:Has_Task] -> (t6)

CREATE (e2) – [:Has_Task] -> (t6)

CREATE (e3) – [:Has_Task] -> (t6)

CREATE (e4) – [:Has_Task] -> (t6)

CREATE (e5) – [:Has_Task] -> (t6)

CREATE (e11) – [:Has_Task] -> (t6)

CREATE (e12) – [:Has_Task] -> (t6)

CREATE (e13) – [:Has_Task] -> (t6)

CREATE (e14) – [:Has_Task] -> (t6)

CREATE (e15) – [:Has_Task] -> (t6)

CREATE (e11) – [:Has_Task] -> (t4)

CREATE (e19) – [:Has_Task] -> (t4)

CREATE (e20) – [:Has_Task] -> (t4)

CREATE (e8) – [:Has_Task] -> (t7)

CREATE (e9) – [:Has_Task] -> (t8)

CREATE (e10) – [:Has_Task] -> (t9)

CREATE (e6) – [:Has_Task] -> (t7)

CREATE (e6) – [:Has_Task] -> (t3)

CREATE (e6) – [:Has_Task] -> (t9)

CREATE (e7) – [:Has_Task] -> (t5)

CREATE (e7) – [:Has_Task] -> (t8)

CREATE (e16) – [:Has_Task] -> (t5)

CREATE (e16) – [:Has_Task] -> (t3)

CREATE (e17) – [:Has_Task] -> (t9)

CREATE (e18) – [:Has_Task] -> (t3)

CREATE (m2) – [:Leads_Task] -> (t4)

CREATE (m4) – [:Leads_Task] -> (t4)

CREATE (m2) – [:Leads_Task] -> (t8)

CREATE (m4) – [:Leads_Task] -> (t8)

CREATE (m2) – [:Leads_Task] -> (t5)

CREATE (m4) – [:Leads_Task] -> (t5)

CREATE (m1) – [:Leads_Task] -> (t1)

CREATE (m3) – [:Leads_Task] -> (t1)

CREATE (m1) – [:Leads_Task] -> (t2)

CREATE (m3) – [:Leads_Task] -> (t2)

CREATE (m1) – [:Leads_Task] -> (t3)

CREATE (m3) – [:Leads_Task] -> (t3)

CREATE (m1) – [:Leads_Task] -> (t6)

CREATE (m3) – [:Leads_Task] -> (t6)

CREATE (m1) – [:Leads_Task] -> (t7)

CREATE (m3) – [:Leads_Task] -> (t7)

CREATE (m1) – [:Leads_Task] -> (t9)

CREATE (m3) – [:Leads_Task] -> (t9)

![image](https://user-images.githubusercontent.com/99159437/162148678-bafaf408-a252-42ae-bbce-b5d979928a6d.png)

## Querries 
### At this point, our graph is complete, however, we need to demonstrate its usefulness by performing some basic querries. 
#### All employees led by "Caroline Susan"
MATCH (m:Manager) – [:Leads_Task] –> (t:Task) <- [:Has_Task] – (e:Employee)
WHERE m.Name = "Caroline Susan"
RETURN DISTINCT m.Name, e.Name
![image](https://user-images.githubusercontent.com/99159437/162149331-2c461cdf-1f69-46d8-a8e0-4d9163b6aaa8.png)

#### All employees aged over 40
MATCH (m:Manager) – [:Leads_Task] –> (t:Task) <- [:Has_Task] – (e:Employee)
WHERE e.Age > "40"
RETURN distinct e.Name as Employee, e.Age as Employee_Age
![image](https://user-images.githubusercontent.com/99159437/162150297-6546c41b-013d-474d-92d7-53ba9bede4e2.png)


#### All tasks and managers of "Jackie Shaw"
MATCH (m:Manager) – [:Leads_Task] –> (t:Task) <- [:Has_Task] – (e:Employee)
WHERE e.Name = "Jackie Shaw"
RETURN m.Name as Manager, e.Name as Employee, t.Type as Task
![image](https://user-images.githubusercontent.com/99159437/162150502-cc9b5732-9b66-4d73-bbb0-fbfb9f074200.png)
MATCH (m:Manager) – [:Leads_Task] –> (t:Task) <- [:Has_Task] – (e:Employee)
WHERE e.Name = "Jackie Shaw"
RETURN m as Manager, e as Employee, t as Task
![image](https://user-images.githubusercontent.com/99159437/162150675-b55d5697-fd5b-4d00-81e9-940689d0d897.png)

#### All employees with a female manager
MATCH (m:Manager) – [:Leads_Task] –> (t:Task) <- [:Has_Task] – (e:Employee)
WHERE m.Sex = "F"
RETURN e.Name as Employee, m.Name as Manager, m.Sex as Manager_Gender
![image](https://user-images.githubusercontent.com/99159437/162150790-062f61fb-8936-461f-9e7f-95853ca26324.png)

#### All employees with a female manager who work on a task that involves development
MATCH (m:Manager) – [:Leads_Task] –> (t:Task) <- [:Has_Task] – (e:Employee)
WHERE m.Sex = "F" and t.Type CONTAINS 'Development'
RETURN e.Name as Employee, t.Type as Task, m.Name as Manager, m.Sex as Manager_Gender
![image](https://user-images.githubusercontent.com/99159437/162150899-4c8c32b6-0d27-473b-9b66-82f3e3f0c9f4.png)
