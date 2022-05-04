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
---
# Literature

* wikipedia
* http://users.ece.utexas.edu/~perry/work/papers/swa-sen.pdf
* https://www.goodreads.com/book/show/296981.Object_Oriented_Software_Engineering
* https://thevaluable.dev/fighting-software-entropy/
