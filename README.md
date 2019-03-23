<h1>Manual Git</h1>
<p>Git es una tecnología que se usa para el versionamiento de código,que facilita el trabajo de varias personas en un proyecto.</p>

 <img src="/img/git-logo.png" alt="logo" width="200"
         height="80">

<h2>Set up inicial</h2>

* 1. Primero necesitamos tener git instalado en nuestra computadora, por esto descargamos la versión que esté disponible desde la web https://git-scm.com/downloads

 <img src="/img/git-download.png" alt="logo" width="600" height="300">

* 2. Para instalar damos doble clic en el ejecutable descargado y le damos "siguiente siguiente" en todo

 <img src="/img/git-install.png" alt="logo" width="600" height="400">

* 3. Terminada la instalación ahora podemos abrir la consola de git más conocida como git bash. Para esto damos clic derecho desde cualquier lugar del escritorio.
 <img src="/img/git-bash-open.png" alt="open" width="600" height="400">

* 4. Configuramos las credenciales ejecutando el código en la consola/terminal abierto.

<code> git config --global user.name "Nombre Apellido" </code>

<code> git config --global user.email "micorreo@dominio.com" </code>

 <img src="/img/git-bash-setting.png" alt="setting" width="600" height="400">


<h2>Empezando un proyecto con Git</h2>

* 1. <b>Crear nuestro repositorio remoto</b>  en la web de Github o Gitlab
Según la nomenclatura "progra1-nombre_apellido-detalle"
https://github.com/new

<img src="/img/git-hub-create.png" alt="setting" width="600" height="400">


* 2. <b>Iniciemos el repositorio local</b> (Estado Untracked) (solo se realiza una vez por proyecto) Clic derecho dentro de la carpeta del proyecto (En este ejemplo la carpeta se llama "Git_Project" y contiene archivos de texto con código) y seleccionamos "Git Bash" o desde cmd ingresamos a la ruta del proyecto y ejecutamos <code>git init</code>.</p>

<img src="/img/git-bash-project.png" alt="setting" width="600" height="400">

<code> git init</code>

* 3. <b>Enlazamos nuestro repositorio remoto con el local </b> (la url se obtiene de la página del Set Up Inicial) Para esto abrimos nuestro gitbash y lanzamos el código.

<img src="/img/git-hub-remote-link.png" alt="setting" width="600" height="300">

<code> git remote add origin https://github.com/miusuariogithub/progra1-nombre_apellido-ejemplo1.git</code> 

<img src="/img/git-remote-add.png" alt="remote" width="500" height="300">

<h2>Trabajando un proyecto</h2>

<img src="/img/git-stages.svg" alt="stages" width="600" height="400">

Al trabajar con git existen distintas etapas o stages que pasa nuestro código. En este caso los siguientes pasos permitirán publicar nuestro código en el repositorio de Github creado.

* 1. <p>Abrimos la consola GitBash desde dentro del proyecto que queremos trabajar. Ejecutaremos el comando que pase al estado de Stagged nuestros archivos</p>

<img src="/img/git-add.png" alt="stages" width="300" height="150">

<code> git add .  </code>

* 2. Seguido "Commiteamos" nuestro proyecto - Estado Snapshot

<img src="/img/git-commit.png" alt="stages" width="500" height="300">

<code> git commit -m "[ADD] Comentario descriptivo" </code>

* 3. "Pusheamos" nuestro proyecto al repositorio remoto que configuramos

<img src="/img/git-push.png" alt="stages" width="500" height="300">

<code>  git push origin master  </code>

* 4.  <b>Listo 😎 </b> Repetimos estos pasos cada vez que modifiquemos o agreguemos algún archivo a nuestro proyecto.


<h2>Descargando un proyecto de otros Propietarios</h2>

<p>Ahora intentemos descargar nuestro u otro proyecto en otra computadora donde no lo tengamos en nuestro disco local.</p>

<p> Descarguemos el proyecto de <b>Netflix</b>  😎 https://github.com/Netflix/spectator-cpp</p>

<img src="/img/git-landing-project.png" alt="stages" width="500" height="300">

* 1. <p>Entramos a la url https://github.com/Netflix/spectator-cpp y copiamos la url para "Clonar el proyecto" damos clic en Clone or Download </p>

<img src="/img/git-clone.png" alt="stages" width="300" height="150">

* 1. <p>Creamos una carpeta donde queremos que se descargue el proyecto y desde allí abrimos la consola de gitbash y ejecutamos</p>

<code>git clone https://github.com/Netflix/spectator-cpp.git</code>
<img src="/img/git-clone-netflix.png" alt="stages" width="300" height="150">

* 2. <p>Listo descargamos el proyecto. Ahora podemos modificarlo y publicarlo en un nuevo repositorio.</p>

<img src="/img/git-clone-done.png" alt="stages" width="300" height="150">

* 3. <p>Ahora necesitamos crear un nuevo repositorio en nuestra cuenta de Github. Para esto sigamos todos los puntos escritos en la sección de <b>"Empezando un proyecto con Git"</b>. Recordemos realizarlo dentro de la carpeta donde descargamos el proyecto.</p>

Creando el Repositorio remoto
<img src="/img/git-netflix-create-repo.png" alt="stages" width="300" height="150">

Iniciando Git desde la carpeta donde se descargó
<img src="/img/git-init-netflix.png" alt="stages" width="300" height="150">

Publicando el repo (<b>Considerar que se cambio en este caso origin por origins</b>)
<img src="/img/git-netflix-publish.png" alt="stages" width="300" height="150">


* 4. <b>Listo 😎 logramos descargar una repo de Netflix y publicar una versión propia </b>


