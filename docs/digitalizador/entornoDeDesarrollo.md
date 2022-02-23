---
sidebar_position: 2
---

# Entorno de desarrollo

Es necesario tener los siguientes dependencias para empezar a realizar cambios en el código fuente, realizar pruebas automatizadas 
y realizar tareas de compilación.

## Control de versiones

### Git

Para el manejo de control de versiones es necesario git, para ello descarguelo desde el [siguiente enlace.](https://git-scm.com/downloads)

#### Github

Una vez descargado git puede estar interactuando con el repositorio [DigitalizadorGitHubRepo](https://github.com/fegarza/digitalizador).



## Python

Preferentemente tener instalado [Python   3.8.2.](https://www.python.org/downloads/release/python-382/)

Una vez instalado Python, se tendrá que corroborar si hay acceso al ejecutable de 
python desde las variables de entorno, para ello ejecute el siguiente comando:
```console
 > python --version
```
Si el resultado es el siguiente no habra que realizar ajustes:
```shell
 > python --version
 Python 3.8.2
```
De lo contrario habría que agregarlo.


## Visual studio code

Como entorno de desarrollo se recomienda utilizar visual studio code debido a la cantidad 
de extensiones y características que facilitan el trabajo a la hora de trabajar con Python.

### Extensiones obligatorias para VSCode

|Nombre|ID|Descripcion|
|------|--|-----------|
|Python| ms-python.python | Kit de desarrollo para python. |
|Task runner|sanaajani.taskrunnercode|Permite usar las tareas definidas en el archivo de configuracion de vscode del proyecto.|
|Python test explorer|littlefoxteam.vscode-python-test-adapter|Permite manejar las pruebas unitarias del proyecto.|

### Extensiones opcionales para VSCode

|Nombre|ID|Descripcion|
|------|--|-----------|
|Python docstring generator| njpwerner.autodocstring | Permite agregar comentarios para la documentacion del proyecto de forma sencilla.|
|Workspace | fooxly.workspace| Simplifica tu espacio de trabajo para acceder más rápido a los archivos deseados.|
| Markdown Preview | bierner.markdown-mermaid| Vista previa de archivos markdown.|

### Entorno virtual

Por medio del gestor de paquetes de python (pip), tendrá que instalar el manejador de entornos virtuales.
Ejecute el sigueinte comando en consola:

```console
 > pip install virtualenv
```
Dirijase a la carpeta en donde se encuentra el codigo fuente del proyecto desde consola:
```console
 > cd C:\Proyectos\digitalizador\
```
Ejecute el siguiente comando para crear un entorno virtual:
```console
 > virtualenv .env
```



## Base de datos

Es necesario una instancia SLQ Server y la base de datos de aduasism3.

