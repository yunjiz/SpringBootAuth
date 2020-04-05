# SpringBootAuth

spring.jpa.hibernate.ddl-auto=update

curl http://localhost:8080/tasks

curl -H "Content-Type: application/json" -X POST -d '{
    "description": "Buy some milk(shake)"
}'  http://localhost:8080/tasks

curl -H "Content-Type: application/json" -X PUT -d '{
    "description": "Buy some milk"
}'  http://localhost:8080/tasks/1

curl -X DELETE http://localhost:8080/tasks/1