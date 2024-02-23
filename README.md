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
**Relación maquinas - usuario**
💎
> :shipit: Diego Alejandro Arévalo Guevara. 20 de febrero de 2024.
