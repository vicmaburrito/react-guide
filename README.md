# react-guide

# 27 Febrero:

  > SI HAY ALGUNA DUDA, FAVOR DE ABRIR UN ISSUE EN ESTE REPOSITORIO CON LA PREGUNTA

  # [DUDAS? AQUI](https://github.com/vicmaburrito/react-guide/issues/new)

# ¿Qué es React?:

React es una biblioteca de JavaScript desarrollada por Facebook que se utiliza para construir interfaces de usuario interactivas y reutilizables. A diferencia de Vanilla JavaScript, que a menudo se centra en manipular el DOM directamente, React se basa en un enfoque de "componentes", lo que significa que divides tu interfaz de usuario en partes más pequeñas y reutilizables  lo que facilita la creación de aplicaciones modulares y mantenibles.

React utiliza el DOM (Document Object Model) para manipular y actualizar la interfaz de usuario. React se basa en el concepto de "virtual DOM", que es una representación en memoria de la estructura del DOM. Cuando hay cambios en el estado de la aplicación, React compara el virtual DOM actual con una versión anterior, determina las diferencias y luego actualiza solo las partes necesarias en el DOM real.
## Porque se usa y que es node_modules, npm y yarn a rasgos generales:


La carpeta "node_modules" es el directorio donde se almacenan las bibliotecas y dependencias de un proyecto Node.js que se instalan a través de herramientas como npm (Node Package Manager) o yarn. Estas herramientas descargan las bibliotecas desde repositorios remotos y las colocan en la carpeta "node_modules" para que el proyecto pueda acceder a ellas. Es importante tener esta carpeta en el archivo ".gitignore" para evitar subirla al repositorio, ya que generalmente es bastante grande y puede generarse de nuevo fácilmente con las dependencias especificadas en el archivo "package.json".

### porque son remotas las librerias?:
 Porque estan alojadas en repositorios externos y pueden ser llamados usando npm(node package modules) o yarn.

Tanto npm (Node Package Manager) como Yarn son gestores de paquetes para JavaScript que permiten instalar, compartir y gestionar las dependencias de un proyecto. Ambos se utilizan comúnmente en proyectos de Next.js y otros proyectos basados en JavaScript o Node.js.

# TODO 27 de Febrero:

> Instalar nvm (node version manager)
bash
    $ curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.3/install.sh | bash


> Comprobar la instalacion
bash
$ nvm --version


> Visualizar que versiones tenemos instaladas localmente

bash
$ nvm ls

>Instalar la version

bash
$ nvm install 18.17.0


> Usar la version
bash
$ nvm use 18.17.0


# Probar requests:

## Que son los HTTPS REQUEST
### Leer ↓
> [HTTPS request](https://developer.mozilla.org/es/docs/Web/HTTP/Methods)

## Probar en su consola bash o PowerShell

### GET REQUEST:

> bash:
bash
curl https://jsonplaceholder.typicode.com/posts/1


>powershell:
powershell
Invoke-WebRequest -Uri "https://jsonplaceholder.typicode.com/posts/1"


### POST Request:

> bash:
bash
curl -X POST -H "Content-Type: application/json" -d '{"title":"foo","body":"bar","userId":1}' https://jsonplaceholder.typicode.com/posts

>powershell
powershell
Invoke-WebRequest -Uri "https://jsonplaceholder.typicode.com/posts" -Method POST -Headers @{"Content-Type"="application/json"} -Body '{"title":"foo","body":"bar","userId":1}'


### PUT Request:
> bash:
bash
curl -X PUT -H "Content-Type: application/json" -d '{"id":1,"title":"foo","body":"bar","userId":1}' https://jsonplaceholder.typicode.com/posts/1

> powershell:
powershell
Invoke-WebRequest -Uri "https://jsonplaceholder.typicode.com/posts/1" -Method PUT -Headers @{"Content-Type"="application/json"} -Body '{"id":1,"title":"foo","body":"bar","userId":1}'


### DELETE REQUEST:

> bash:
bash
curl -X DELETE https://jsonplaceholder.typicode.com/posts/1


> powershell:
powershell
Invoke-WebRequest -Uri "https://jsonplaceholder.typicode.com/posts/1" -Method DELETE


## Async-Await
### Leer ↓
[Async y Await](https://www.aluracursos.com/blog/asyncawait-en-javascript-que-es-y-cuando-usar-programacion-asincrona)



## Server Side y Client side
### Leer ↓
[Javascript Server y Client side](https://www.cloudflare.com/es-es/learning/serverless/glossary/client-side-vs-server-side/)


## Por mirar:

> Si deseas desarrollar la aplicación en local siguiendo los pasos del video de abajo, es un extra. De lo contrario, no hay problema; el objetivo es familiarizarse con la terminología, estructura y definición de un proyecto de React.

[Primera Web con React](https://youtu.be/pFyAu4R684s?si=l71wBG_lEXCcIP4g)


## Extra: 
> Leer e interactuar con la documentacion original:

[Aprende React](https://es.react.dev/learn)