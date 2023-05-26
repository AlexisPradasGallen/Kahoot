# DIAGRAMA DE CLASES
## Kahoot
Tiene tres clases la clase professor, la clase alumno y la clase partida.

```mermaid
sequenceDiagram
    Profesor->>Partida: Iniciar Partida
    Partida->>Profesor: Codigo
    Profesor->>Alumno: Mostrar Codigo
    Alumno->>Profesor: Ingresar Codigo
    loop Cada Pregunta
    Partida->>Profesor: Pregunta
    Profesor->>Alumno: Mostrar pregunta
    Partida->>Profesor: Respuestas
    Profesor->>Alumno: Mostrar repuestas
    Partida->>Alumno: Temporizador
    Alumno->>Partida: Contestacion
    Partida->>Alumno: Solucion y puntos
    Partida->>Profesor: Tabla clasificacion
    Profesor->>Alumno: Mostrar tabla clasificacion
    end
    Partida->>Profesor: Tabla clasificacion
    Profesor->>Alumno: Mostrar tabla clasificacion

```

# DIAGRAMA DE ACTIVIDADES
## UML de login
Como acceder en una pagina web como si ya estas logeado como si no  
```mermaid
flowchart
    A[Entrar a la pagina] --> B{Existe usuario?}
    B --> |Acceso| C[Acceder a mi cuenta] 
    B --> |Registro| D[Crear usuario] 
    D --> B
```


# DIAGRAMA DE ESTADOS
## UML de estados
Cuales son los pasos para hacer un burpee

```mermaid
stateDiagram-v2
    state "Tumbarse" as tumbado
    state "Levantarse" as levantado
    state "Saltando" as saltando

    [*] --> pie
    pie --> tumbado: tumbarse
    tumbado --> levantado: levantarse
    levantado --> saltando: saltar
    saltando --> [*]
```

