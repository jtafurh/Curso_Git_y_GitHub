# Curso Git y GitHub

1. [¿Por qué usar un sistema de control de versiones como Git?](#1-¿por-qué-usar-un-sistema-de-control-de-versiones-como-gita-name"clase1"a)
2. [¿Que es Git?](#2-¿que-es-git-a-name--"clase2"a)
3. [Instalando Git y Git Bash en windows](#3-instalando-git-y-git-bash-en-windowsa-name"clase3"a)
4. [Instalar Git en Mac](#4-instalar-git-en-maca-name"clase4"a)
5. [Instalar Git en Linux](#5-instalando-git-en-linuxa-name"clase5"a)
6. [Editor de código, archivo binarios y de texto plano](#6-editor-de-código-archivo-binarios-y-de-texto-planoa-name"clase6"a)
7. [Introducción a la linea de comandos](#7-introducción-a-la-linea-de-comandosa-name"clase7"a)
8. [Crea un repositorio de Git y haz tu primer commit](#8-crea-un-repositorio-de-git-y-haz-tu-primer-commita-name"clase8"a)
9. [9. Analizar cambios en los archivos de tu proyecto con Git](#9-analizar-cambios-en-los-archivos-de-tu-proyecto-con-gita-name"clase9"a)

## 1. ¿Por qué usar un sistema de control de versiones como Git?<a name="clase1"></a>

Usar un sistema de control de versiones nos ayuda a que cuando tengamos que guardar los cambianos realizados en un archivo, y no perder las versiones anteriores de estos, no tengamos que hacerlo en distintos archivos como *archivo_v1, archivo_v2, etc.* sino que guardaremos un solo archivo que tendrá un historial con los cambios realizados, cuando y quien los hizo, ademas de permitirnos acceder a versiones anteriores del archivo.

>Git fue creado por **Linus Torvalds**, el mismo creador de Linux.

### Comando para Git
- `git init` Inicia un repositorio en la carpeta del proyecto.
- `git add <archivo.txt>` Le indica al control de versiones de git que se va agregar un archivo.txt, lo coloca en "Staging Area" 
- `git commit -m "mensaje de descripción"` Almacena definitivamente los cambios del archivo a la base de datos del sistema, aquí se puede agregar un mensaje de descripción.
- `git add .` Agrega todos los archivos que presenten cambios.
- `git status` Nos muestra el estatus de la base de datos, para saber si hay cambios por agregar.
- `git show` Nos muestra todos los cambios históricos hechos, lineas de código, cuando y quien los hizo.
- `git log archivo.txt` Muestra la historia entera de un archivo.
- `git push` Envía el repositorio local a un repositorio remoto
- `git pull` Trae un repositorio remoto a un repositorio local

### ¿Que es un repositorio?
Un repositorio es una base de datos donde se guardan los datos de cualquier archivo.

-----------------------

## 2. ¿Que es Git? <a name = "clase2"></a>
Es un sistema de control de versiones muy popular creado por **Linus Torvalds**, el mismo creador de Linux.

### ¿Que es un sistema de control de versiones?
Es un software que registra los cambios realizados a un archivo o conjunto de archivos a lo largo del tiempo.

Dicho sistema nos permite recuperar archivos del proyecto, regresar a versiones anteriores de este, comparar los cambios realizados a lo largo del tiempo, ver quien realizo los cambios y cuando fueron hechos.

-----------------------

## 3. Instalando Git y Git Bash en windows<a name="clase3"></a>

Descargamos Git desde la [pagina oficial de Git](https://git-scm.com/downloads)

### Instalación
- La casilla de Git Bash debe estar seleccionada\
![](/images/img_git_bash.png)
- Seleccionar la opción de usar git desde la linea de comando nativa y desde git bash\
![](/images/git_command_line.png)
-  Seleccionar OpenSSL library\
![](/images/opnenSSL.png)
- Seleccionar la primera opción de Checkout Windows-stile\
![](/images/checkout_windows.png)
- Seleccionar use MinTTY\
![](/images/use_minTTY.png)
- Seleccionar las tres opciones\
![](/images/config_extra.png)
- instalar y finish

### Para abrir
- Windows > Git Bash

----------------

## 4. Instalar Git en Mac<a name="clase4"></a>

Descargamos Git desde la [pagina oficial de Git](https://git-scm.com/downloads)

- Abrir el instalador de mac
- En el archivo hacer: Click derecho > open > open
- Instalar

En la terminal de mac:
- Para acceder a información de git 

        git
- Para ver la version de git instalada

        git --version

----------------

## 5. Instalando Git en Linux<a name="clase5"></a>

- Realizar un update (Actualiza la lista de paquetes que se pueden instalar) como administrador

        sudo apt-get update

- Comando para instalar git 

        sudo apt-get install git

----------------

## 6. Editor de código, archivo binarios y de texto plano<a name="clase6"></a>


### Editores de código

- Atom https://atom.io/
- Sublime Text https://www.sublimetext.com/
- Visual Studio Code https://code.visualstudio.com/

### Tipos de archivos
- **Archivos de texto (.txt):** Texto plano normal y sin nada especial. Block de notas y editores de texto.
- **Archivos RTF (.rtf):** Texto de diferentes tamaños, estilos y colores. Se distorsiona al abrirlo en editores de texto avanzados.
- **Archivos de Word (.docx):** Texto de diferentes tamaños, colores e imágenes. Al ser código binario se distorsiona al abrirlo en un editor de código.

> Git solo soporta archivos de texto plano.

----------------

## 7. Introducción a la linea de comandos<a name="clase7"></a>

- `pwd` Nos muestra la ruta de carpetas en la que te encuentras ahora mismo.
- `mkdir` Nos permite crear carpetas (por ejemplo, mkdir Carpeta-Importante).
- `touch` Nos permite crear archivos (por ejemplo, touch archivo.txt).
- `rm` Nos permite borrar un archivo o carpeta (por ejemplo, rm archivo.txt). Mucho cuidado con este comando, puedes borrar todo tu disco duro.
- `cat` Ver el contenido de un archivo (por ejemplo, cat nombre-archivo.txt).
- `ls` Nos permite cambiar ver los archivos de la carpeta donde estamos ahora mismo. 

  Podemos usar uno o más argumentos para ver más información sobre estos archivos (los argumentos pueden ser `-- + el nombre del argumento` o `- + una sola letra` o shortcut por cada argumento).
  - `ls -a` Mostrar todos los archivos, incluso los ocultos.
  - `ls -l` Ver todos los archivos como una lista.
- `cd` Nos permite navegar entre carpetas.
  - `cd /`** Ir a la ruta principal:
  - `cd` o `cd ~`** Ir a la ruta de tu usuario
  - `cd carpeta/subcarpeta`** Navegar a una ruta dentro de la carpeta donde estamos ahora mismo.
  - `cd ..` (cd + dos puntos)** Regresar una carpeta hacia atrás.

  Si quieres referirte al directorio en el que te encuentras ahora mismo puedes usar cd . (cd + un punto).
- `history` Ver los últimos comandos que ejecutamos y un número especial con el que podemos repetir su ejecución.
- `! + número`** Ejecutar algún comando con el número que nos muestra el comando history (por ejemplo, !72).
- `clear` Para limpiar la terminal. También podemos usar los atajos de teclado `Ctrl + L` o `Command + L`.

>Recuerda que podemos descubrir todos los argumentos de un comando con el argumento `--help` (por ejemplo, `cat --help`).

------------

## 8. Crea un repositorio de Git y haz tu primer commit<a name="clase8"></a>
### Haciendo commit
- Nos situamos en la carpeta del proyecto `nuevo`
- Comando `git init` para iniciar un repositorio que guardara el historial de cambios del proyecto.
- Automáticamente se crea una capeta oculta llamada `.git`
  ![](/images/git_init.png)
- Creamos los archivos archivo.txt, archivo_2.txt y archivo_3.txt y los modificamos 
- Comando `git status` para ver los cambios que faltan agregar al repositorio
  ![](/images/git_status.png)
- Comando `git add <archivo.txt>` para agregar un archivo en especifico al stedsh
  ![](/images/git_status_2.png)
- Comando `git add .` para agregar todos los archivos disponibles al stedsh
  ![](/images/git_add_todo.png)
- Comando `git rm --cached archivo.txt` retira el archivo agregado del stedsh
  ![](/images/git_cached_archivo.png)
- Comando `git commit -m "Este es un mensaje"` para confirmar que agregue los cambios al repositorio y va acompañado de un mensaje (Colocar un mensaje es una buena practica para tener un seguimiento de los cambios que se han realizado)
  ![](/images/git_commit.png)

### Configurar GIT

Es importante configurar los datos para saber quien esta haciendo los cambios.
Si no configuramos los datos nos enviara variables por defecto de windows

- Comando `git config` nos muestra todas las configuraciones disponible de GIT
- Comando `git config --list` muestra la configuración por defecto o información de los datos ya configurados. 
- Comando `git config --list --show-origin` muestra el lugar (ruta) donde esta guardada la configuración
- Comando `git config --global user.name "Tu nombre"` para cambiar el nombre de usuario
(--global, se va a cambiar la configuración global de todos los usuarios)
-- Comando `git config --global user.email "Tu correo"` para configurar el correo del usuario
  ![](/images/git_config.png)

### Haciendo cambios a los archivos
- Después de realizar cambios revisamos el status comando `git status` y nos mostrara los archivos modificados
  ![](/images/git_estatus_cambios.png)
- Realizamos un "commit" para agregar los cambios al repositorio

### Ver la historia de los archivos
- Comando `git log <archivo.txt>` Para ver los cambios
  - Se muestra el nombre de quien hizo los cambios y cuando fueron hechos
  ![](/images/git_log.png)
  - Se muestra`tag` es el código interno para nombrar los cambios
  ![](/images/tag_name.png)

---

## 9. Analizar cambios en los archivos de tu proyecto con Git<a name="clase9"></a>
### Cambios de los archivos
- Comando `git show archivo.txt` muestra:
  1. El cogido de registro del ultimo commit
  2. La rama en la que estamos 
  3. Nombre que colocamos como mensaje al commit
  4. Realiza un diff, que es comparara la version anterior con la nueva y mostrara la diferencia 
  5. Indicador dentro de la base de datos de git donde están los cambios
  6. Las versiones existentes
  7. Indicador de cuantos bits cambiaron
  8. Muestra el contenido del archivo 
        - En color `-rojo` el contenido eliminado 
        - En color `+verde` el contenido agregado
      ![](/images/git_show.png)
- Si realizamos un `commit` sin un mensaje, se abrirá un GNU nano y nos pedirá ingresar un mensaje.
### Comparando versiones de un mismo archivo
- Comando `git diff <"versión_anterior"> <"versió_nueva">` podemos hacer una comparación entre dos versiones distintas.
---

## 10. ¿Qué es el staging y los repositorios? Ciclo básico de trabajo en Git<a name="clase10"></a>

---

## 11. ¿Qué es un Branch (rama) y cómo funciona un Merge en Git<a name="clase11"></a>

---

## 12. Volver en el tiempo en nuestro repositorio utilizando reset y checkout<a name="clase12"></a>

---

## 13. Git reset vs. Git rm<a name="clase13"></a>

---
