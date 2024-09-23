# Wordpress + Mysql

## Start:
1. `kubectl apply -k deploy/`
2. Необходимо создать базу данных для wordpress:\
`kubectl exec -it <mysql-pod-name> -- bash`\
`mysql -u root -pmysql12345`\
`create database wordpress;`\
`exit`
3. Пробросить порт 10.0.2.21:30080