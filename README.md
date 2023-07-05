# actividadGit
**Trabajo de git sistema operativos** 

investigacion basica de git

¿que es Git y para que se utiliza?

Git es un sistema de control de versiones distribuido, lo que significa que un clon local del proyecto es un repositorio de control de versiones completo. Estos repositorios locales plenamente funcionales permiten trabajar sin conexión o de forma remota con facilidad. 

2)¿Cuales son las principales caracteristicas de Git?

Fuerte apoyo al desarrollo no lineal, por ende rapidez en la gestión de ramas y mezclado de diferentes versiones. Git incluye herramientas específicas para navegar y visualizar un historial de desarrollo no lineal. Una presunción fundamental en Git, es que un cambio será fusionado mucho más frecuentemente de lo que se escribe originalmente, conforme se pasa entre varios programadores que lo revisan.
 
 Gestión distribuida. Al igual que Darcs, BitKeeper, Mercurial, SVK, Bazaar y Monotone, Git le da a cada programador una copia local del historial del desarrollo entero, y los cambios se propagan entre los repositorios locales. Los cambios se importan como ramas adicionales y pueden ser fusionados en la misma manera que se hace con la rama local.


Los almacenes de información pueden publicarse por HTTP, FTP, rsync o mediante un protocolo nativo, ya sea a través de una conexión TCP/IP simple o a través de cifrado SSH. Git también puede emular servidores CVS, lo que habilita el uso de clientes CVS pre-existentes y módulos IDE para CVS pre-existentes en el acceso de repositorios Git.


Gestión eficiente de proyectos grandes, dada la rapidez de gestión de diferencias entre archivos, entre otras mejoras de optimización de velocidad de ejecución.

3) ¿Qué es un sistema de control de versiones?

Los sistemas de control de versiones son software que ayudan a realizar un seguimiento de los cambios realizados en el código a lo largo del tiempo. A medida que un desarrollador editar el codigo, el sistema de control de versiones toma una instantanea de los archivos. Despues, guarda esa inranranea de forma permanente para que se pueda recuperar mas adelante si es necesario. Sin control de versiones, los desarrolladores tienen la tentación de mantener varias copias de código en su equipo. Esto es peligroso porque es fácil cambiar o eliminar un archivo en la copia incorrecta del código, lo que podría perder trabajo. Los sistemas de control de versiones resuelven este problema administrando todas las versiones del código, pero presentando al equipo una sola versión a la vez.

4) ¿Cuál es la diferencia entre Git y otros sistemas de control de versiones?

Los llamados sistemas de control de versiones fueron creados con el fin de detectar cambios en los documentos o archivos y se encargan de guardar todas las versiones anteriores, incluyendo el registro de fecha y hora, así como el identificador del usuario de un archivo para que los datos puedan ser recuperados y restaurados en cualquier momento. De esta forma, es posible determinar qué usuario ha realizado cambios en un punto determinado. Los objetivos generales de este tipo de sistemas consisten en coordinar el acceso compartido de varios usuarios a los archivos y permitir el desarrollo simultáneo de varias bifurcaciones o branches.
Generalmente, los sistemas de control de versiones se utilizan para el desarrollo de software, para aplicaciones de oficina y para gestores de contenido. Dos de los más conocidos son Apache Subversion (SVN) y Git, los cuales pueden ser instalados internamente en el servidor propio o externamente en el servidor de algún proveedor de alojamiento web. 

b)Instalación y configuración de Git:

Investiga cómo instalar Git en diferentes sistemas operativos (Windows, macOS, Linux).

	WINDOWS:
	Descargue e instale Git para Windows. Una vez instalado, Git está disponible
desde el símbolo del sistema o PowerShell. Se recomienda seleccionar los valores predeterminados durante la instalación, a menos que haya una buena razón para cambiarlos.
Git para Windows no se actualiza automáticamente. Para actualizar Git para Windows, descargue la nueva versión del instalador, que actualiza Git para Windows y conserva toda la configuración.
macOS:
macOS 10.9 (Mavericks) y versiones posteriores instala Git la primera vez que intenta ejecutarlo desde el terminal. Aunque este método es una manera sencilla de obtener Git en un sistema, no permite el control sobre la frecuencia con la que se aplican las actualizaciones o correcciones de seguridad.
En su lugar, se recomienda instalar Git a través de Homebrew y usar Homebrew herramientas para mantener Git actualizado. Homebrew es una excelente manera de instalar y administrar código abierto herramientas de desarrollo en un Equipo Mac desde la línea de comandos.
Instale Homebrew y ejecute lo siguiente para instalar la versión más reciente de Git en un equipo Mac:
> brew install git


Para actualizar la instalación de Git, use la opción de actualización de Homebrew:
> brew upgrade git
Linux: 
Use el sistema de administración de paquetes nativo de la distribución de Linux para instalar y actualizar Git. Por ejemplo, en Ubuntu:

> sudo apt-get install git

2)Explica los pasos para configurar tu nombre de usuario y dirección de correo electrónico en Git.

-Abrir la terminal.
-Verifica la configuración actual con el comando 
git config --global --list.
-Configurar el nombre de usuario con el comando 
git config --global user.name "Tu Nombre".
-Configurar la dirección de correo electrónico con el comando 
git config --global user.email "tucorreo@example.com".
-Verificar la configuración actualizada con el comando 
git config --global --list.

3.Comandos básicos de Git:
git add 
Mueve los cambios del directorio de trabajo al área del entorno de ensayo. Así puedes preparar una instantánea antes de confirmar en el historial oficial.
git commit
Confirma la instantánea preparada en el historial del proyecto. En combinación con git add, define el flujo de trabajo básico de todos los usuarios de Git.

git status
Muestra el estado del directorio en el que estás trabajando y la instantánea preparada. Lo mejor es que lo ejecutes junto con git add y git commit para ver exactamente qué se va a incluir en la próxima instantánea.

b)
El comando git log se utiliza para ver el historial de cambios en un repositorio Git. Muestra una lista cronológica de confirmaciones, con detalles como autor, fecha y mensaje descriptivo.
El comando git diff muestra las diferencias entre versiones de archivos en un repositorio Git. Puede mostrar diferencias entre el directorio de trabajo y el área de preparación, o entre confirmaciones específicas. Proporciona opciones para mostrar las diferencias de manera más compacta o detallada.


4.Trabajando con repositorios remotos:

a)
-Abrir una terminal y navegar hasta el directorio deseado.
-Obtén la URL del repositorio remoto.
Ejecutar git clone <URL> en la terminal, cambiando <URL> con la URL del repositorio.
-Tocar el Enter y Git comenzará a clonar el repositorio en tu directorio actual.
-Si es necesario, proporciona las credenciales de autenticación.
-Una vez completada la clonación, tendremos una copia local del repositorio remoto.

b)-git branch: Crear, listar o eliminar ramas.

git branch nombre-rama: Crea una nueva rama.
git branch: Lista las ramas existentes.
git branch -d nombre-rama: Elimina una rama.
-git checkout: Cambiar entre ramas o crear una nueva rama y cambiar a ella.
git checkout nombre-rama: Cambia a una rama existente.
git checkout -b nombre-rama: Crea y cambia a una nueva rama.
git checkout -- nombre-archivo: Descarta cambios en   un archivo.
-git merge: Fusionar cambios de una rama en otra.
git merge nombre-rama: Fusiona una rama en la rama actual.o d

5.Colaboración en Git: 

a)Investiga cómo trabajar en equipo en un repositorio remoto utilizando ramas y fusiones
Para poder colaborar en cualquier proyecto Git, necesitas saber cómo gestionar repositorios remotos. Los repositorios remotos son versiones de tu proyecto que están hospedados en Internet o en cualquier otra red,  Puedes tener varios de ellos, y en cada uno tendrás generalmente permisos de lectura en solitario o de lectura y escritura. Colaborar con otras personas implica gestionar estos repositorios remotos enviando y trayendo datos de ellos cada vez que necesite compartir su trabajo, 
Para ver los remotos que tienes configurados, debes ejecutar el comando git remote. Mostrará los nombres de cada uno de los remotos que tiene especificados. Si has clonado tu repositorio, deberías ver al menos origin (origen, en inglés) - este es el nombre que por defecto Git le da al servidor del que has clonado, En el día a día del trabajo con Git una de las cosas útiles que podemos hacer es trabajar con ramas. Las ramas son caminos que puede tomar el desarrollo de un software, algo que ocurre naturalmente para resolver problemas o crear nuevas funcionalidades. En la práctica permiten que nuestro proyecto pueda tener diversos estados y que los desarrolladores sean capaces de pasar

b) Explica qué son las solicitudes de extracción (pull requests) y cómo se utilizan para revisar y aprobar cambios.
Vamos a presentar un ejemplo simple de ramificar y fusionar, con un flujo de trabajo que se podría presentar en la realidad. Imagina que sigues los siguientes pasos:
Trabaja en un sitio web.
Creas una rama para un nuevo tema sobre el que quieres trabajar.
Realiza algo de trabajo en esa rama.
En este momento, recibe una llamada avisando de un problema crítico que tiene solución. Y sigues los siguientes pasos:
Vuelve a la rama de producción original.
Creas una nueva rama para el problema crítico y lo resuelves trabajando en ella.
Tras las pertinentes pruebas, fusionar (merge) esa rama y la envía (push) a la rama de producción.
Vuelve a la rama del tema en que andabas antes de la llamada y continúas tu trabajo.
