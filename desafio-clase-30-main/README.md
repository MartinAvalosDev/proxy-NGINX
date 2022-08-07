# Desafio NGINX Y SERVIDORES CON BALANCE DE CARGA
## Alumno: Martin Alejandro Avalos

Desafío: Servidores - Nginx & PM2

Para probar la aplicación crear el archivo .env en base al .env_example

Configurar opcionalmente un puerto: 

```
app.js --port=8080
```

Comandos para ejecución de pruebas: 

```
node app.js --port PORT_NUMBER --mode fork
node app.js --port PORT_NUMBER --mode cluster

pm2 start app.js --name="SERVER_NAME" --watch -- PORT_NUMBER

pm2 start app.js --name="SERVER_NAME" --watch -i max -- PORT_NUMBER
```
