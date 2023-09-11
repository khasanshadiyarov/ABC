# Applied Research Conduction
Applied research conduction diagram is an activity diagram, which is used as a blueprint of conducting an applied research. The diagram does not limit the freedom of choice and defines more the abstract actions to be performed. Expanding the diagram with additional actions is not prohibited.

---

## Contents
- [Introduction](#applied-research-conduction)
- [Diagram](#diagram)

## Diagram
```plantuml
@startuml
start
:Define the Purpose;
if (Problem Solving) then (Yes)
(No) elseif (Practice Improvement) then (Yes)
else (No)
    stop
endif
:Select a Research Design;
if (Qualitative) then (Yes)
(No) elseif (Quantitative) then (Yes)
(No) elseif (Multimethod) then (Yes)
else (No)
    stop
endif
fork
    :Develop Data Collection Plan;
fork again
    :Collect Data Analytical Tools;
    if (Enough Tools) then (Yes)
    else (No)
        stop
    endif
endfork
:Identify the Study Site;
:Define and Describe the Problem;
while (Existing Solution) is (Yes)
    :Review Literature;
    :Evaluate Satisfactory;
    if (Satisfactory Solution) then (Yes)
        stop
    else (No)
    endif
endwhile (No)
:Formulate Research Objectives;
:Formulate Research Hypotheses;
fork
    :Define Feasibility Terms;
fork again
    :Evaluate the Feasibility;
endfork
if (Research is Feasible) then (Yes)
else (No)
    stop
endif
:Write a Research Proposal;
if (Proposal Approved) then (Yes)
else (No)
    stop
endif
fork
    :Define Logistics;
fork again
    :Plan the Logistics;
endfork
:Collect Data;
if (Data Meets the Design) then (Yes)
(No) elseif (Optimization Available) then (Yes)
    :Optimize the Data;
else (No)
    stop
endif
if (Enough Tools) then (Yes)
(No) elseif (Supplementation Available) then (Yes)
    :Supplement the Tools;
else (No)
    stop
endif
:Analyze Data;
:Interpret the Research Findings;
:Write the Final Report;
:Prepare Presentation Plan;
:Present Results;
if (Further Actions Needed) then (Yes)
    :Evaluation and Follow-Up;
    end
else (No)
    stop
endif
@enduml
```

#diagram