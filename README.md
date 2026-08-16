# Hola programadores

# Primer Diagnóstico de Node.js

## Introducción

En este trabajo realicé un diagnóstico básico de mi entorno de desarrollo utilizando Node.js, npm, Git, Visual Studio Code y GitHub.

El objetivo fue comprobar que las herramientas estuvieran instaladas y aprender a utilizar el objeto `process` de Node.js para obtener información sobre el entorno y sobre el programa que se está ejecutando.

---

## 1. Herramientas utilizadas

Para realizar el trabajo utilicé:

- Node.js
- npm
- Git
- Visual Studio Code
- GitHub

### Node.js

Node.js es un entorno que permite ejecutar código JavaScript fuera del navegador.

Lo utilicé para ejecutar el archivo `diagnostico.js`.

### npm

npm es el gestor de paquetes de Node.js.

Lo utilicé para agregar un script que permite ejecutar el diagnóstico de una manera sencilla mediante:

`npm run diagnostico`

### Git

Git es un sistema de control de versiones.

Lo utilicé para guardar los cambios realizados en el proyecto mediante commits y para mantener un historial de los cambios.

### Visual Studio Code

Utilicé Visual Studio Code para crear y editar los archivos del proyecto y para trabajar con la terminal.

### GitHub

Utilicé GitHub para almacenar el repositorio de manera remota y entregar el proyecto.

---

## 2. Verificación de las herramientas

Primero abrí la terminal de Visual Studio Code y comprobé que las herramientas necesarias estuvieran instaladas.

### Node.js

Ejecuté:

`node --version`

El resultado fue:

`v24.15.0`

### npm

Ejecuté:

`npm --version`

El resultado fue:

`11.12.1`

### Git

Ejecuté:

`git --version`

El resultado fue:

`git version 2.54.0.windows.1`

Con estas pruebas comprobé que Node.js, npm y Git estaban instalados y disponibles desde la terminal.

---

## 3. Creación del proyecto

Creé una carpeta llamada:

`primer-diagnostico`

Dentro de esta carpeta trabajé con los siguientes archivos:

- `diagnostico.js`
- `package.json`
- `README.md`

La estructura final del proyecto quedó de la siguiente manera:

    primer-diagnostico/
    ├── diagnostico.js
    ├── package.json
    └── README.md

---

## 4. Creación de diagnostico.js

Creé el archivo `diagnostico.js`.

En este archivo realicé el diagnóstico utilizando el objeto incorporado `process` de Node.js.

El objeto `process` contiene información relacionada con el proceso de Node.js que está ejecutando el programa.

Utilicé diferentes propiedades de `process` para obtener la información solicitada en la actividad.

---

## 5. Versión de Node.js

Para obtener la versión de Node.js utilicé:

`process.version`

Esta propiedad permite conocer qué versión de Node.js está ejecutando el programa.

En mi computadora el resultado fue:

`v24.15.0`

---

## 6. Plataforma

Para conocer la plataforma utilicé:

`process.platform`

Esta propiedad permite conocer sobre qué plataforma se está ejecutando Node.js.

En mi computadora el resultado fue:

`win32`

Esto indica que el programa se está ejecutando en Windows.

---

## 7. Argumentos recibidos

Para obtener los argumentos recibidos desde la terminal utilicé:

`process.argv`

Esta propiedad contiene los argumentos que se pasan al programa cuando se ejecuta desde la línea de comandos.

Para comprobar su funcionamiento ejecuté:

`node diagnostico.js hola programadores`

El resultado permitió observar que `hola` y `programadores` fueron recibidos como argumentos por el programa.

También se puede observar que `process.argv` contiene información relacionada con la ejecución de Node.js y con la ubicación del archivo `diagnostico.js`.

---

## 8. Variable de entorno

La consigna también solicita mostrar una variable de entorno.

Para acceder a las variables de entorno utilicé:

`process.env`

En lugar de mostrar todas las variables de entorno, seleccioné una variable específica:

`process.env.OS`

`process.env` permite acceder a las variables de entorno disponibles en el sistema.

La variable `OS` contiene información sobre el sistema operativo.

En mi computadora el resultado fue:

`Windows_NT`

De esta manera pude mostrar una variable de entorno específica sin imprimir toda la información disponible en `process.env`.

---

## 9. Resultado del diagnóstico

Al ejecutar el programa obtuve un resultado similar a:

    Hola programadores
    === DIAGNÓSTICO DE NODE.JS ===
    Versión de Node.js: v24.15.0
    Plataforma: win32
    Argumentos recibidos: [...]
    Sistema operativo: Windows_NT

Con esto pude comprobar que el programa obtiene correctamente la información solicitada.

---

## 10. Creación de package.json

Utilicé el archivo `package.json` para guardar la configuración y la información del proyecto.

Dentro de `package.json` agregué un script llamado `diagnostico`.

El script ejecuta:

`node diagnostico.js`

Por este motivo puedo ejecutar el diagnóstico mediante:

`npm run diagnostico`

Esto permite repetir la ejecución del programa sin tener que escribir nuevamente todo el comando.

---

## 11. Prueba del script npm

Después de configurar `package.json`, ejecuté:

`npm run diagnostico`

La terminal mostró:

    > primer-diagnostico@1.0.0 diagnostico
    > node diagnostico.js

Después apareció la información correspondiente al diagnóstico.

Esto comprobó que el script de npm estaba correctamente configurado.

---

## 12. Prueba de argumentos

También realicé una prueba enviando argumentos desde la terminal.

Ejecuté:

`node diagnostico.js hola programadores`

El programa recibió los argumentos mediante:

`process.argv`

De esta manera comprobé que los datos escritos después del nombre del archivo son recibidos por el programa.

---

## 13. Uso de Git

Utilicé Git para controlar las diferentes versiones del proyecto.

Primero comprobé el estado del repositorio utilizando:

`git status`

Después agregué los cambios con:

`git add .`

Luego guardé los cambios mediante commits.

Para consultar el historial utilicé:

`git log --oneline`

---

## 14. Commits incrementales

Durante el desarrollo realicé diferentes commits para guardar los cambios de manera incremental.

El historial del proyecto quedó con commits como:

- `Agrega README del proyecto`
- `Completa diagnostico de Node.js`
- `cambios npm`
- `inicio con nmp`

Los commits incrementales permiten observar la evolución del proyecto y los cambios realizados durante el desarrollo.

---

## 15. GitHub

Después de realizar los cambios y commits, utilicé:

`git push`

para subir los cambios al repositorio remoto de GitHub.

El repositorio contiene los archivos principales del proyecto:

- `diagnostico.js`
- `package.json`
- `README.md`

---

## 16. Comandos utilizados

Durante el desarrollo utilicé los siguientes comandos.

### Comprobar Node.js

`node --version`

### Comprobar npm

`npm --version`

### Comprobar Git

`git --version`

### Ejecutar el diagnóstico

`node diagnostico.js`

### Ejecutar el diagnóstico con argumentos

`node diagnostico.js hola programadores`

### Ejecutar mediante npm

`npm run diagnostico`

### Comprobar el estado de Git

`git status`

### Ver el historial de commits

`git log --oneline`

### Agregar cambios

`git add .`

### Crear un commit

`git commit -m "mensaje del commit"`

### Subir cambios a GitHub

`git push`

---

## 17. Evidencia de ejecución

Como evidencia del trabajo realicé capturas de la terminal donde se pueden observar las diferentes pruebas.

Las evidencias incluyen:

1. La versión de Node.js.
2. La versión de npm.
3. La versión de Git.
4. La ejecución de `diagnostico.js`.
5. La prueba de argumentos.
6. La ejecución mediante `npm run diagnostico`.

Estas pruebas permiten comprobar que el entorno estaba correctamente configurado y que el programa funciona.

---

## 18. Archivos de la entrega

El proyecto contiene:

### diagnostico.js

Es el archivo principal del programa.

Se encarga de realizar el diagnóstico utilizando el objeto `process`.

### package.json

Contiene la configuración del proyecto y el script `diagnostico` utilizado para ejecutar el programa mediante npm.

### README.md

Contiene la documentación del proyecto, los pasos realizados, los comandos utilizados y una explicación del funcionamiento.

---

## 19. Qué aprendí sobre process

Durante el trabajo aprendí que `process` es un objeto incorporado de Node.js que permite obtener información relacionada con el proceso que está ejecutando el programa.

Las propiedades utilizadas fueron:

- `process.version`: permite obtener la versión de Node.js.
- `process.platform`: permite conocer la plataforma.
- `process.argv`: permite obtener los argumentos recibidos desde la terminal.
- `process.env`: permite acceder a las variables de entorno.
- `process.env.OS`: permite consultar específicamente la variable de entorno correspondiente al sistema operativo.

---

## 20. Conclusión

Con este trabajo pude comprobar que mi entorno de desarrollo estaba correctamente configurado.

También aprendí a utilizar el objeto `process` de Node.js y sus diferentes propiedades para obtener información del entorno de ejecución.

Además, aprendí a utilizar npm para crear un comando de ejecución, Git para controlar las versiones del proyecto y GitHub para almacenar y entregar el trabajo.

El diagnóstico final permite comprobar la versión de Node.js, la plataforma, los argumentos recibidos y una variable de entorno.

---

## Autor

Trabajo realizado como actividad práctica de diagnóstico de Node.js.

Hola programadores.