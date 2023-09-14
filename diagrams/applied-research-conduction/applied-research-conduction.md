# Applied Research Conduction Diagram
Applied research conduction diagram is an activity diagram, which is used as a blueprint of conducting an applied research. The diagram does not limit the freedom of choice and defines more the abstract actions to be performed. Expanding the diagram with additional actions is not prohibited.

---

## Contents
- [Introduction](#applied-research-conduction)
- [Diagram](#diagram)

## Diagram
```plantuml
@startuml
start
repeat :Define the Purpose;
    if (Problem Solving) then (Yes)
    (No) elseif (Practice Improvement) then (Yes)
    else (No)
    endif
repeat while (Purpose Clarified) is (No)
->Yes;
repeat :Select the Design;
    if (Qualitative) then (Yes)
    (No) elseif (Quantitative) then (Yes)
    (No) elseif (Multimethod) then (Yes)
    else (No)
    endif
repeat while (Design Clarified) is (No)
->Yes;
:Identify the Study Site;
:Describe the Problem;
while (Existing Solution) is (Yes)
    :Review the Literature;
    :Evaluate Satisfaction;
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
    repeat :Evaluate Feasibility;
    backward:Optimize Terms;
    repeat while (Feasible Research) is (No)
    ->Yes;
endfork
fork
    :Define Logistics;
fork again
    repeat :Plan the Logistics;
    repeat while (Feasibility Aligned) is (No)
    ->Yes;
endfork
repeat :Write the Research Proposal;
repeat while (Proposal Approved) is (No)
->Yes;
:Collect Data;
repeat :Optimize the Data;
repeat while (Data Meets the Design) is (No)
->Yes;
:Analyze the Data;
:Interpret the Research Findings;
:Write the Final Report;
:Prepare a Presentation Plan;
:Present the Results;
if (Further Actions Needed) then (Yes)
    fork
        :Monitor the Research;
    fork again
        :Pursue the Research;
    endfork
    end
else (No)
    stop
endif
@enduml
```

#diagram