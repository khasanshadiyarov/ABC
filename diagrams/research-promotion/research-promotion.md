# Research Promotion Diagram
Research promotion diagram is an activity diagram, which is used as a blueprint to promote a research in order to increase public awareness of it. This takes into account research publishing, audience identification and engagement via creating multimedia resources and progressively reaching out a wider audience.

---

## Contents
- [Introduction](#research-promotion)
- [Diagram](#diagram)

## Diagram
```plantuml
@startuml
start
repeat :Prepare a Research;
repeat while (Ready for Promotion) is (No)
->Yes;
if (Accessible Personal Source(s)) then (Yes)
    :Deploy the Research;
    note right
        Publication source 
        controlled by the author.
    endnote
else (No)
endif
if (Publishing Required) then (Yes)
    :Find a Publisher;
    repeat :Publish the Research;
    backward:Adapt the Research;
    repeat while (Guidelines are Met) is (No)
    ->Yes;
else (No)
endif
repeat :Identify the Audience;
:Prioritize Key Groups;
repeat while (Reachable Groups) is (No)
->Yes;
while (Possible Multimedia Resource) is (Yes)
    if (Feasible Creation) then (Yes)
        :Create the Resource;
        note right
            Multimedia resource 
            with promotion value.
        endnote
    else (No)
    endif
endwhile (No)
:Promote the Outputs;
note right
    Research outputs and 
    its additional resources.
endnote
repeat :Monitor the Outputs;
backward:Adapt the Outputs;
repeat while (Satisfactory Impact) is (No)
->Yes;
while (Research Potential Reached) is (No)
    fork
        :Reach Out to a Wider Audience;
    fork again
        :Engage in Networking and Collaboration;
    endfork
endwhile (Yes)
end
@enduml
```

#diagram