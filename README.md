# Wordpress + Mysql

## Start:
1. На ноде node01 создать папку:\
`sudo mkdir /mnt/data`\
`sudo chmod 777 /mnt/data`
2. `kubectl apply -k deploy/`
3. Необходимо создать базу данных для wordpress:\
`kubectl exec -it <mysql-pod-name> -- bash`\
`mysql -u root -pmysql12345`\
`create database wordpress;`\
`exit`
4. Пробросить порт 10.0.2.21:30080
5. http://localhost:30080/