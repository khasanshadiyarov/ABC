# Literature Review Conduction Diagram
Literature review conduction diagram is an activity diagram, which is used as a blueprint of conducting a literature review. The diagram does not limit the freedom of choice and defines more the abstract actions to be performed. Expanding the diagram with additional actions is not prohibited.

---

## Contents
- [Introduction](#literature-review-conduction-diagram)
- [Diagram](#diagram)

## Diagram
```plantuml
@startuml
|Collect|
start
:Select a Type;
note right
    * Narrative;
    * Systematic;
    * Meta-analysis.
endnote
repeat :Set Up Collecting System;
repeat while (Enough Functionality) is (No)
->Yes;
|#gainsboro|Write|
:Define a Preliminary Title;
:Define Objectives;
|Collect|
:Define Feasibility Terms;
repeat :Evaluate Feasibility;
backward:Optimize Terms;
repeat while (Feasible Review) is (No)
->Yes;
:Identify Keywords;
:Select a Structure;
note right
    * Chronological;
    * Thematic;
    * Methodological;
    * Theoretical.
endnote
while (Available Database) is (Yes)
    fork
        :Search Database;
    fork again
        :Select Literature;
    endfork
endwhile (No)
:Organize Sources;
note right
    Sources reflects 
    the structure.
endnote
if (Flood) then (Yes)
    :Filter Literature;
(No) elseif (Gap) then (Yes)
    :Source Literature;
else (No)
endif
:Study Literature;
|Write|
repeat :Structure an Outline;
repeat while (Satisfactory Outline) is (No)
->Yes;
:Summarize Findings;
fork
    :Identify Gaps;
fork again
    while (Fillable Gap) is (Yes)
        :Fill Gap;
    endwhile (No)
endfork
:Cite Sources;
:Write the Review;
repeat :Edit and Proofread;
repeat while (Mistakes Found) is (Yes)
->No;
|Monitor|
:Seek Feedback;
|Write|
:Finalize and Format;
|Monitor|
if (Stand-Alone Paper) then (No)
    :Incorporate Into Project;
else (Yes)
endif
if (Further Actions Needed) then (Yes)
    fork
        :Monitor Review;
    fork again
        :Sustain Review;
    endfork
    end
else (No)
    stop
endif
@enduml
```

#diagram