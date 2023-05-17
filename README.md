# Comandos Básicos de Git

### Configuración Inicial
```shell I'm tab B
git config --global user.name "tu_nombre" // Configura el nombre que se asociará con tus commits.
git config --global user.email "tu_email" // Configura el correo electrónico que se asociará con tus commits.
```

### Inicio de un Repositorio Git
```shell
git init // Inicia un nuevo repositorio git en tu directorio actual.
git clone [url] // Copia un repositorio git existente de la URL proporcionada.
```

### Agregar y Confirmar Cambios
```shell
git status // Muestra el estado de los archivos (sin seguimiento, modificados, preparados para commit).
git add [archivo] // Comienza a seguir un archivo para el próximo commit.
git add . // Añade todos los archivos nuevos o modificados al área de preparación.
git commit -m "mensaje del commit" // Graba los cambios en el repositorio con un mensaje descriptivo.
```

### Historial de Commits
```shell
git log // Muestra el historial de commits.
git log --oneline // Muestra el historial de commits en formato resumido.
```

### Ramas (Branches)
```shell
git branch // Lista todas las ramas en tu repositorio.
git branch [nombre_de_la_rama] // Crea una nueva rama.
git switch [nombre_de_la_rama] // Cambia a la rama especificada.
git switch -c [nombre_de_la_rama] // Crea una nueva rama y cambia a ella.
git merge [nombre_de_la_rama] // Combina la rama especificada con la rama actual.
```

### Interactuar con Remoto
```shell
git remote add origin [url] // Conecta tu repositorio local a un servidor remoto.
git remote set-url origin [https://github.com/username/repodeejemplo.git] // actualiza el origin de tu repositorio local
git push -u origin [nombre_de_la_rama] // Sube tus commits a la rama remota.
git pull // Actualiza tu repositorio local con el más reciente commit del repositorio remoto.
git fetch // Obtiene todos los cambios del repositorio remoto, pero no los aplica a tu trabajo actual.
```