# :mortar_board: AUTOMATION SERVICE CHOREOGRAPHY

[:rewind:back](../README.md)

Editing Status: :construction: (under construction))

Last Modification: 09.05.2021

---
## :three: Design Patterns in Software Development

### Introduction to the Gang of Four

Recurring pattern in software goes back to four gentlemen named Erich Gamma, Richard Helm, Ralph Johnson and John Vlissides - the so-called Gang of Four (GoF). They published in 1994 their famous book about "Design Patterns. Elements of Reusable Object-Oriented Software" [1].

In the context of my research, I use the format of design patterns to describe a concrete task to be solved and its solution. For this purpose, the four gentlemen mentioned have defined a scheme for the structure and description of software patterns. In the following, the used parts of this scheme are briefly explained.


Category  | Description
---       | ---
Name and Classification  | provides the Name and Classification of the given design pattern
Purpose                  | Defines the purpose of this pattern
Motivation               | Reason to use this pattern
Applicability            | describes the using context of this pattern
Structure                | describes the common structure of this pattern
Actors                   | Software entities that are involved within the pattern
Interaction              | Description of the interaction between the involved software entities
Consequences             | Pros and Cons of the application
Implementation           | Important information regarding the realization of this pattern
Practical Use            | Description of where the pattern is already used
Cross References         | References to other related patterns.


### Introduction to PLC Programming Standards

The possibilities of object-oriented programming in PLC runtimes is unfortunatelly strongly limited due to the requirement of hard realtime capabilities depending on the use case. 

Within the world of PLC programming two accepted international standards are available, first, the IEC 61131-3, second, the IEC 61499. 

**IEC 61499** focuses on a type of modeling language in relation to distributed automation functions. The modeling is differentiated into data and events. The standard itself only defines the modeling aspects, but no runtime aspects. Function Blocks represent functions that execute the incoming data when triggered by the associated event. 

**IEC 61131-3** specifies various programming languages for programmable logic controllers - graphical and textual languages, as well as continuous and state-descriptive languages. The languages are comparable to classic script languages and offer two types of source code structuring with the help of functions (FC) and function blocks (FB). Due to the demand for hard real-time requirements PLC programs are only conditionally or not at all changeable at runtime. 

**Higher Languages** in the last few years the automation suppliers offers integration possibilities of higher languages into classic PLC programs. Those capabilities allow the integration of higher language algorithms. Unfortunately, the freedom of software adaptability known from common object-oriented programming lanugages from the web service or desktop technology can be reached within PLC environments.

---
Summarized, the software in PLC runtime environments is more or less fixed in its compiled form. This can be attributed back to the strict requirements regarding realtime capabilities. This results in the need of flexible and adabtable software structures within the compiled PLC code.

For this reason I have been working for many years on the implementation of adaptive software structures based on the Pascal-like programming language Structured Text (SCL). For the description of such adaptive software structures I use the scheme of design patterns and have reduced the scheme of the GoF to the categories relevant for me, which are meaningful for a PLC program.

### Description Scheme of PLC Programming Patterns

The following base scheme of PLC Programming Pattern is used within my research: 

Category  | Description
---       | ---
Name                | Name of the PLC Programming Pattern
Purpose             | Describes the purpose of the PLC Programming Pattern
Use Case            | Describes the use case behind the pattern
Applicability       | Describes the usage context of the pattern
Structure           | Describes the structure of the pattern
Actors              | Introduce the involved software entities 
Interaction         | Describes the interaction between the entities
Consequences        | Pros and Cons of the pattern
Implementation      | Hints for implementation of the pattern
Cross References    | References to other related patterns.

## :hash: References

No. | Publication
--- | ---
1 | Design Patterns. Elements of Reusable Object-Oriented Software; Gamma, Helm, Johnson, Vlissides; 1994; Addison-Wesley; ISBN 0-201-63361-2

