---
marp: true
theme: default  
_class: lead


---

# Front Matter
<!-- _paginate: false -->
a dot com

---
<!-- paginate: true -->


# Outline

* Item 1
* Item 2
* Item 3

---

# Nice to Meet You!

* Life: 45 yo, married + 3 kids, live in Shoham, Yoga.
* Work: 
    * Current: 2 yrs @ [At-Bay](https://at-bay.com) as a Software Architect (...what's that?)
    * Overall: ~15 yrs in the industry, mostly in startups, but fallen a couple of times to the corporate hands
    * Fun time 1: Does Tech Due Diliginces for a couple of VCs
    * Fun time 2: Contributor to the [Dapr](https://dapr.io) open source project
    * Fun time 3: this thing
* Formal: 
    * B.Sc in Biotechnology & Environmental Science from Tel-Hai College 
    * M.Sc in Biochemistry from Weizmann Institute of Science
    * Ph.D studies in Biophysics (I didn't complete) from Weizmann


---

# What We'll Talk About


* *Software architecture*
    * origin
    * theory
    * in practice 
* The oh-so-boring SaaS company
* The *relational database* as the greatest invention in industrial software engineering
* Where the relational database *fails*
* Q & A

---

# Software Architecture

## Wikipedia 
* "Software architecture refers to the fundamental <span style="color:blue;">structures</span> of a software <span style="color:blue;">system</span> and the <span style="color:purple;">discipline</span> of creating such structures and systems." 
* "Each <span style="color:blue;">structure</span> comprises software <span style="color:red;"> elements</span>, <span style="color:red;"> relations </span> among them, and <span style="color:purple;">properties</span> of both elements and relations."

* system:
    * structures: 
        * element <-- relation --> element

---

# Software Architecture
## Static Analysis of a System

* "Software architecture is about making fundamental structural choices that are <span style="color:red;">costly to change once implemented</span>" (wikipedia, this time getting it right)
* What's costly to change (over time):
    * Programming Language (changing/adding mostly breaks common tools) --> "element"
    * <span style="color:blue">Data Model</span> (breaks everything if done wrong) --> "property of an element"
    * Runtime Environment (on-prem vs cloud x/y/z) --> "structure+system"
    * Contracts (APIs) --> "relations"

---

# Software Architecture

## System Design
* "Fighting" the windmills of **complexity** as software obeys the 2nd law of thermodynamics (complexity never decreases) ![bg right:40% 80%](complexity.webp)

* But what is complex? ("This part of the codebase doesn’t *feel* right!")
* When do you surrender to the evil called "management"?
* The humanity! (You care about people not losing their minds)
---
# Software Architecture
## Evaluation

Also know as **reviewing things**:
* High Level Design Review - system
* Code Reviews - quality
* Security Reviews - security safety
* Test Review - code safety
* Data Modeling Review - correct abstraction/database performance
* DevOps Review - environment/deployment
* SRE Review - gauges

Long Story Short - Make sure stuff alines with your company *vision* on how software is being made

---
# Software Architecture
## Evolution
* Fun/easy stuff is to do *NEW* things
* NotSoFun/hardest stuff is to evolve *OLD* things
* Read about: "evolutionary architecture" 
---

# The Oh-So-Boring SaaS Company

* Capture *Data*
* Do something over *Data*
* Arrange the *Data* nicely
* Ask for money from customers/advertisers
![bg right:40% 80%](whats.png)
![bg right:40% 80%](insta.jpeg)
---

# The Data Model

## Data Model == Database Tables

* It is how you model the business entities

* It is the single most important element in the system design of a SaaS

* It is the only effort worth investing BEFORE writing a single line of code (atypical for a startup to do)

* Still, it is ever evolving with the business needs, but once in use, *it is hard to change*

---
# Data Model - Implementation
Usually, we're talking about a *Relational Database* 

### Popular RDBs
* PostgreSQL, MySQL, Oracle, SQL Server
---
# Relational Databases
The founding father of the relational model is *Edgar F. Codd*

* Based on his work published in 1970 (yes, 52 yo technology) while he was working for IBM
* He won the Turing Award in 1981 for this work
* He applied Relational Algebra and proposed such an algebra as a basis for database query languages
* Five primitive operators: selection, projection, Cartesian product (also called the cross product or cross join), set union, set difference.


![bg right:40% 80%](Edgar_F_Codd.jpeg)

---

# Relational Databases - Basics

* The relational model means that the *logical data structures*—the data tables, views, and indexes—are separate from the *physical storage structures*
* Use a declarative language to apply operations over the logical representation and don't mind the physical aspects

* Ability to create meaningful information by joining of tables

* To ensure that data is always accurate and accessible, relational databases follow certain integrity rules

* Relational databases are transactional—they guarantee the state of the entire system is consistent at any moment

---

# Relational Databases - Example




---
# Literature

* wikipedia
* http://users.ece.utexas.edu/~perry/work/papers/swa-sen.pdf
* https://www.goodreads.com/book/show/296981.Object_Oriented_Software_Engineering
* https://thevaluable.dev/fighting-software-entropy/
* [E.F. Codd paper](https://www.seas.upenn.edu/~zives/03f/cis550/codd.pdf)