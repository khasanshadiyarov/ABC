# Research Promotion
Research promotion is an activity diagram, which is used as a blueprint to promote a research in order to increase public awareness of it. This takes into account research publishing, audience identification and engagement via creating multimedia resources and progressively reaching out a wider audience.

---

## Contents
- [Introduction](#research-promotion)
- [Diagram](#diagram)

## Diagram
```plantuml
@startuml
start
repeat :Prepare the Research;
repeat while (Ready for Promotion) is (No)
->Yes;
if (Accessible Personal Source) then (Yes)
    :Deploy on Personal Source;
else (No)
endif
if (Publishing Required) then (Yes)
    :Find a Publisher;
    repeat :Publish the Research;
    backward:Evaluate and Adapt the Research;
    repeat while (Guidelines are Met) is (No)
    ->Yes;
else (No)
endif
repeat :Identify the Audience;
:Prioritize Key Groups;
repeat while (Reachable Groups) is (No)
->Yes;
if (Multimedia Resources) then (Yes)
    repeat :Clarify Multimedia Resources;
    repeat while (Creation is Feasible) is (No)
    ->Yes;
    :Create Multimedia Resources;
else (No)
endif
:Promote the Outputs Online;
repeat :Monitor the Outputs;
backward:Evaluate and Adapt the Outputs;
repeat while (Satisfactory Impact) is (No)
->Yes;
if (Research Potential Reached) then (No)
    fork
        :Reach Out to a Wider Audience;
    fork again
        :Engage in Networking and Collaboration;
    endfork
else (Yes)
endif
end
@enduml
```

#diagram