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
- No puedo crear otra replica mientras hay una en curso.
  - ![image](https://github.com/DavidJGG/AWS-notes/assets/60149403/0f5e38af-4462-4537-95cd-9dc1cd0f175e)



![image](https://github.com/DavidJGG/AWS-notes/assets/60149403/1facbfda-e53b-4fa9-97a6-b4721b045a4e)

