# Reto 2 // Diego Arévalo
Solución del reto dos de Programación Orientada a Objetos
## Diagrama de Clases UML para un gimnasio.
**Relación usuario - gimnasio**
```mermaid
classDiagram
    User --> Gym
    class Gym{
      +Name
      +Direction
      +Machines
      +collect_money()
    }
    class User{
        +pay()
    }
```
**Relación gimnasio - partes gimnasio**
```mermaid
classDiagram
    User --> Gym
    Gym *-- Name
    Gym *-- Direction
    Gym *-- Machines

    class Gym{
      +Name
      +Direction
      +Machines
      +collect_money()
    }
    class User{
        +pay()
    }
    class Name{
        +Gym gym
    }
    class Direction{
        +Gym gym
    }
    class Machines{
        +Gym gym
        +Machines types
    }
```
**Relación entre máquinas**
```mermaid
classDiagram
    treadmill --|> Machines
    elliptical --|> Machines
    kettlebells --|> Machines
    battle_ropes --|> Machines
    chest_press --|> Machines
    dumbbells --|> Machines
    leg_press --|> Machines
    bench_press --|> Machines
    weight_bench --|> Machines
    chest_pull --|> Machines    

    class Machines{
        +Gym gym
        +Machines types
    }
    class treadmill{
        +form
        +to_exercise(gym)
    }
    class elliptical{
        +form
        +to_exercise(gym)
    }
    class kettlebells{
        +form
        +to_exercise(gym)
    }
    class battle_ropes{
        +form
        +to_exercise(gym)
    }
    class chest_press{
        +form
        +to_exercise(gym)
    }
    class dumbbells{
        +form
        +to_exercise(gym)
    }
    class leg_press{
        +form
        +to_exercise(gym)
    }
    class bench_press{
        +form
        +to_exercise(gym)
    }
    class weight_bench{
        +form
        +to_exercise(gym)
    }
    class chest_pull{
        +form
        +to_exercise(gym)
    }
```

> :shipit: Diego Alejandro Arévalo Guevara. February 20, 2024.
