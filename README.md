![Alt text](https://g.gravizo.com/source/mygraph1?https%3A%2F%2Fgithub.com%2Fssehoony%2Fgravizo%2Fmaster%2FREADME.md)
<details> 
<summary></summary>
mygraph1
@startuml;
actor User;
participant "First Class" as A;
participant "Second Class" as B;
participant "Last Class" as C;
User -> A: DoWork;
activate A;
A -> B: Create Request;
activate B;
B -> C: DoWork;
activate C;
C -> B: WorkDone;
destroy C;
B -> A: Request Created;
deactivate B;
A -> User: Done;
deactivate A;
@enduml
mygraph1
</details>
