# AWS-notes

## Creacion de RDS read replica para un RDS for PostgreSQL 16.1
- m5d.large
- 100 GB de storage

### Comportamiento observado:

- Al solicitar la read replica el cluster pasa a un estado backing-up
- 9 minutos despues el cluster pasa a un stado avaiable, pero la replica aun sigue en creating.
- 
- A las replicas se les puede poner un tamaño de maquina diferente.
- El storage debe de ser identico
- No puedo crear otra replica mientras hay una en curso.
