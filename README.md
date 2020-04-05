# SpringBootAuth

https://auth0.com/blog/implementing-jwt-authentication-on-spring-boot/

spring.jpa.hibernate.ddl-auto=update

curl http://localhost:8080/tasks

curl -H "Content-Type: application/json" -X POST -d '{
    "description": "Buy some milk(shake)"
}'  http://localhost:8080/tasks

curl -H "Content-Type: application/json" -X PUT -d '{
    "description": "Buy some milk"
}'  http://localhost:8080/tasks/1

curl -X DELETE http://localhost:8080/tasks/1

curl -H "Content-Type: application/json" -X POST -d '{
    "username": "admin",
    "password": "password"
}' http://localhost:8080/users/sign-up

curl -i -H "Content-Type: application/json" -X POST -d '{
    "username": "admin",
    "password": "password"
}' http://localhost:8080/login

curl -H "Content-Type: application/json" \
-H "Authorization: Bearer xxx.yyy.zzz" \
-X POST -d '{
    "description": "Buy watermelon"
}'  http://localhost:8080/tasks

curl -H "Authorization: Bearer xxx.yyy.zzz" http://localhost:8080/tasks