# AWS-notes

## Creacion de RDS read replica para un RDS for PostgreSQL 16.1
- m5d.large
- 100 GB de storage

### Comportamiento observado:

- Al solicitar la read replica el cluster pasa a un estado backing-up
- 9 minutos despues el cluster pasa a un stado avaiable, pero la replica aun sigue en creating.
- 25 minutos despues la replica esta lista
- A las replicas se les puede poner un tamaño de maquina diferente.
- El storage debe de ser identico
  ![image](https://github.com/DavidJGG/AWS-notes/assets/60149403/961abad9-bd8a-41b7-b0ff-87e0ecd761f7)

- No puedo crear otra replica mientras hay una en curso.  (Puedo crear replicas simultaneas, si y solo si el cluster tiene un estado available)
  ![image](https://github.com/DavidJGG/AWS-notes/assets/60149403/0f5e38af-4462-4537-95cd-9dc1cd0f175e)







