# Applied Research Conduction Diagram
Applied research conduction diagram is an activity diagram, which is used as a blueprint of conducting an applied research. The diagram does not limit the freedom of choice and defines more the abstract actions to be performed. Expanding the diagram with additional actions is not prohibited.

---

## Contents
- [Introduction](#applied-research-conduction)
- [Diagram](#diagram)

## Diagram
```plantuml
@startuml
|Prepare|
start
:Define Purpose;
note right
    * Problem Solving;
    * Practice Improvement.
endnote
:Select a Design;
note right
    * Qualitative;
    * Quantitative;
    * Multimethod.
endnote
:Identify Study Site;
|Research|
:Describe Problem;
|Prepare|
while (Existing Solution) is (Yes)
    :Review Literature;
    :Evaluate Satisfaction;
    if (Satisfactory Solution) then (Yes)
        stop
    else (No)
    endif
endwhile (No)
|#gainsboro|Research|
:Formulate Research Objectives;
:Formulate Research Hypotheses;
|Prepare|
:Define Feasibility Terms;
repeat :Evaluate Feasibility;
backward:Optimize Terms;
repeat while (Feasible Research) is (No)
->Yes;
|Research|
fork
    :Define Logistics;
fork again
    repeat :Plan Logistics;
    repeat while (Feasibility Aligned) is (No)
    ->Yes;
endfork
repeat :Write Research Proposal;
repeat while (Proposal Approved) is (No)
->Yes;
:Collect Data;
repeat :Optimize Data;
repeat while (Data Meets the Design) is (No)
->Yes;
:Analyze Data;
:Interpret Research Findings;
:Write Final Report;
repeat :Edit and Proofread;
repeat while (Mistakes Found) is (Yes)
->No;
|Monitor|
if (Presentation Needed) then (Yes)
    :Prepare Presentation Plan;
    :Present Results;
else (No)
endif
if (Further Actions Needed) then (Yes)
    fork
        :Monitor Research;
    fork again
        :Sustain Research;
    endfork
    end
else (No)
    stop
endif
@enduml
```

#diagram