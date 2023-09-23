# Paper Promotion Diagram
Paper promotion diagram is an activity diagram, which is used as a blueprint to promote an academic paper in order to increase public awareness of it. This takes into account publishing, audience identification and engagement via creating multimedia resources and progressively reaching out a wider audience.

---

## Contents
- [Introduction](#paper-promotion)
- [Diagram](#diagram)

## Diagram
```plantuml
@startuml
|Publish|
start
repeat :Prepare Paper;
repeat while (Ready for Promotion) is (No)
->Yes;
if (Personal Source(s)) then (Yes)
    :Deploy Paper;
    note right
        The author's 
        personal source.
    endnote
else (No)
endif
if (Academic Publishing) then (Yes)
    :Find Publisher;
    repeat :Publish Paper;
    backward:Adapt Paper;
    repeat while (Guidelines are Met) is (No)
    ->Yes;
else (No)
endif
|#gainsboro|Promote|
repeat :Identify Audience;
:Prioritize Key Groups;
repeat while (Reachable Groups) is (No)
->Yes;
repeat :Collect Promotional Content;
fork
    :Paper Outputs;
fork again
    :Multimedia Resource;
    if (Feasible Creation) then (Yes)
        :Create Multimedia;
    else (No)
    endif
endfork
repeat while (Key Groups Targeted) is (No)
->Yes;
|Publish|
repeat :Publish Content;
backward:Adapt Content;
repeat while (Guidelines are Met) is (No)
->Yes;
|Promote|
:Promote Content;
|Monitor|
repeat :Monitor Engagement;
backward:Resolve Problem;
repeat while (Satisfactory Impact) is (No)
->Yes;
while (Paper Potential Reached) is (No)
    :Reach Out to Wider Audience;
    :Engage in Networking and Collaboration;
endwhile (Yes)
end
@enduml
```

#diagram