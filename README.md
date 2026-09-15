# Práctica: Manejo de Repositorio Local y GitHub

### Datos del estudiante
- **Nombre completo:** Renata Marreros
- **Matrícula:** 2630582
- **Nombre de la práctica:** Creación y vinculación de repositorio local con GitHub

### 1. Objetivo de la práctica
El objetivo es aprender a crear un repositorio local con Git, entender para qué sirve cada comando y lograr sincronizarlo con un repositorio remoto en GitHub.

### 2. Descripción del procedimiento realizado
Primero configuré Git con mi nombre y correo. Después creé una carpeta de trabajo en mi PC, dentro de ella creé los archivos de texto `datos.txt` y `notas.txt`. Luego inicialicé Git en esa carpeta para convertirla en repositorio local, agregué los archivos al área de preparación y realicé el primer commit. Finalmente vinculé mi repositorio local con GitHub y sincronicé los cambios.

### 3. Comandos de Git utilizados y su función
- `git config --global user.name "Ali"` : Sirve para identificar quién hace los commits. Es como mi firma.
- `git config --global user.email "ali@gmail.com"` : Registra mi correo para vincular los commits a mi cuenta de GitHub.
- `git init` : Crea la carpeta oculta .git y convierte mi carpeta normal en un repositorio.
- `git add .` : Manda mis archivos al área de staging, los prepara para ser guardados.
- `git commit -m "mensaje"` : Guarda una versión de mis archivos con un mensaje que explica qué hice.
- `git remote add origin URL` : Conecta mi repo local con el repo que creé en GitHub.
- `git push -u origin main` : Sube mis archivos locales a GitHub.
- `git pull` : Baja los cambios que están en GitHub a mi computadora.

### 4. Cómo se creó el repositorio local
Lo creé desde PowerShell con `mkdir` para hacer la carpeta y entré con `cd`. Dentro de ella ejecuté `git init`. Con esto Git empieza a rastrear todos los cambios que haga en esa carpeta.

### 5. Cómo se vinculó el repositorio local con GitHub
Primero creé un repositorio vacío en GitHub sin README. Copié la URL que me dio y en mi terminal usé `git remote add origin [URL]`. Con `git remote -v` verifiqué que sí se vinculó.

### 6. Sincronización Local → GitHub
Esta sincronización se hace cuando quiero subir lo que hice en mi PC a la nube. Se usa el comando `git push`. En mi caso usé `git push -u origin main` para subir mi primer commit. Después de eso ya podía ver mis archivos en la página de GitHub.

### 7. Sincronización GitHub → Local
Es el proceso inverso, cuando hay cambios en GitHub y los quiero bajar. Se usa `git pull origin main`. Esto sirve por si edito algo directamente en GitHub o si trabajo desde otra computadora.

### 8. Archivos contenidos en el repositorio
- `README.md`: Este archivo con toda la documentación de la práctica.
- `datos.txt`: Archivo con mis datos personales y la descripción de la práctica.
- `notas.txt`: Archivo de prueba para practicar el comando add y commit.

### 9. Conclusión personal
En esta práctica aprendí que Git no es solo guardar archivos, sino tener un control de versiones. Entendí la diferencia entre el área de trabajo, staging y el commit. Al principio me confundía el push y pull, pero ahora sé que push es subir y pull es bajar. Me servirá para futuros proyectos de programación.
