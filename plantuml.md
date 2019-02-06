---
layout: default
---

# PlantUML

_Code:_

```;
@startuml
class Car

Driver - Car : drives >
Car *- Wheel : have 4 >
Car -- Person : < owns

@enduml
```

_Result:_

![PlantUML example](/assets/img/plantuml.png)

(Source: [plantuml.com](http://plantuml.com/class-diagram))
