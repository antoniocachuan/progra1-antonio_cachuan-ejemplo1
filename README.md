#Manual Git
Git es una tecnología que se usa para el versionamiento de código,que facilita el trabajo de varias personas en un proyecto.

##Set up inicial

* Aqui necesitamos crear nuestro repositorio en la web de Github o Gitlab
Según la nomenclatura "progra1-nombre_apellido-detalle"
https://github.com/new

* Necesitamos tener git instalado en nuestra computadora (https://git-scm.com/downloads) "siguiente siguiente"

Ahora Digámosle a git quienes somos 
- Abrir la consola de git (conocida como gitbash o abrir cmd)
- Configuramos git con nuestras credenciales
> git config --global user.name "Nombre Apellido"
> git config --global user.email "micorreo@dominio.com"



##Trabajando un proyecto con Git

* Iniciemos el repositorio (solo se realiza una vez por proyecto) - Estado Untracked
- Clic derecho dentro de la carpeta del proyecto y seleccionamos "Git Bash"
-  desde cmd ingresamos a la ruta del proyecto y escribimos
> git init

* Enlazamos nuestro repositorio remoto con el local (la url se obtiene de la página del Set Up Inicial)
> git remote add origin https://github.com/miusuariogithub/progra1-nombre_apellido-ejemplo1.git



##Trabajando un proyecto
Luego del git init nuestros archivos están en estado Tracked

- Pasamos al estado Stagged nuestros archivos
> git add .

- "Commiteamos" nuestro proyecto - Estado Snapshot
> git commit -m "[ADD] First commit"

- "Pusheamos" nuestro proyecto al repositorio remoto
> git push origin master

- Listo 😎 (Repetimos estos pasos cada vez que modifiquemos o agreguemos algún archivo)



