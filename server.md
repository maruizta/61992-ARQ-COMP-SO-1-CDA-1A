# Iniciar un servidor en una red LAN

## Instalacion de dependencias
En este ejemplo usaremos nodejs para levantar un servidor. 
Asi que antes de comenzar nos aseguraremos de tener instalado nodejs, podemos seguir las instrucciones de supagina oficial. https://nodejs.org/es

- Ejecutamos el siguiente comando en el terminal para asegurarnos que tenemos nodejs instalado.
```shell
$ node --version
```
![alt text](./server/node.png)
- Ejecutamos el siguiente comando en el terminal para asegurarnos que tenemos npm instalado.
```shell
$ npm --version
```
![alt text](./server/npm.png)

## Creacion de un proyecto

- Creamos una carpeta con el comando `mkdir <project_name>` y nos dirigimos alli con `cd <project_name>`
![alt text](./server/project.png)

- Creamos un archivo index.html con `touch index.html`
![alt text](./server/touch.png)

- En html, todo lo que se pueda renderizar es un nodo. Desde etiquetas (h1, div, span, etc), text, numeros e incluso espacios. En este ejemplo usaremos h1, simplemente para que el texto se vea grande. Pero puede ser un texto simple. Y para ello usaremos nuestro editor favorito. 
![alt text](./server/h1.png)

## Levantar el servidor

- En la direccion o ruta de nuestro proyecto ejecutaremos el siguiente comando `npm install server`. Esto instalara las dependecias necesarias en una nueva carpeta llamada `node_modules` para leventar el servidor.
![alt text](./server/server.png)

- Iniciar el servidor con `npx serve`. Por defecto usa el puerto 300. Nos muestra una direccion **Local** que podemos abrir en el navegador de nuestro host. Pero para los demas miembros de nuestra LAN deben usar la direccion **Network**
![alt text](./server/serve.png)

- Mostrando nuestra pagina en el host
![alt text](./server/desktop.png)

- Mostrando nuestra pagina desde un dispositivo diferente. Usando la direccion **Network**
![alt text](./server/mobile.jpeg)

> [!WARNING]  
> Algunos navegadores pueden bloquear el acceso a direcciones no seguras (http)

> [!TIP]
> Los dispositivos externos podran acceder al servidor siempre y cuando todos esten conectados a la misma red.