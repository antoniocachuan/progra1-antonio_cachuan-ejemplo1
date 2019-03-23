<h1>Manual Git</h1>
<p>Git es una tecnología que se usa para el versionamiento de código,que facilita el trabajo de varias personas en un proyecto.</p>

 <img src="/img/git-logo.png" alt="logo" width="200"
         height="80">

<h2>Set up inicial</h2>

* 1. Primero necesitamos tener git instalado en nuestra computadora, por esto descargamos la versión que esté disponible desde la web https://git-scm.com/downloads

 <img src="/img/git-download.png" alt="logo" width="600" height="400">

* 2. Para instalar damos doble clic en el ejecutable descargado y le damos "siguiente siguiente" en todo

 <img src="/img/git-bash-open.png" alt="logo" width="600" height="400">

* 3. Terminada la instalación ahora podemos abrir la consola de git más conocida como git bash. Para esto damos clic derecho desde cualquier lugar del escritorio.
 <img src="/img/git-bash-open.png" alt="open" width="600" height="400">

* 4. Configuramos las credenciales ejecutando el código en la consola/terminal abierto.

<code> git config --global user.name "Nombre Apellido" </code>

<code> git config --global user.email "micorreo@dominio.com" </code>

 <img src="/img/git-bash-setting" alt="setting" width="600" height="400">


<h2>Empezando un proyecto con Git</h2>

* <b>Crear nuestro repositorio </b>  en la web de Github o Gitlab
Según la nomenclatura "progra1-nombre_apellido-detalle"
https://github.com/new

* <b>Iniciemos el repositorio </b> (Estado Untracked) (solo se realiza una vez por proyecto) Clic derecho dentro de la carpeta del proyecto y seleccionamos "Git Bash" o desde cmd ingresamos a la ruta del proyecto y escribimos:</p>

> git init

* <b>Enlazamos nuestro repositorio remoto con el local </b> (la url se obtiene de la página del Set Up Inicial, también se lanza desde el gitbash) 

> git remote add origin https://github.com/miusuariogithub/progra1-nombre_apellido-ejemplo1.git



<h2>Trabajando un proyecto</h2>
Luego del git init nuestros archivos están en estado Tracked

- Pasamos al estado Stagged nuestros archivos
> git add .

- "Commiteamos" nuestro proyecto - Estado Snapshot
> git commit -m "[ADD] First commit"

- "Pusheamos" nuestro proyecto al repositorio remoto
> git push origin master

- Listo 😎 (Repetimos estos pasos cada vez que modifiquemos o agreguemos algún archivo)



