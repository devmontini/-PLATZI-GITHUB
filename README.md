# Hyperblog 💚

Un blog increíble para el[ curso de Git y Github](https://platzi.com/cursos/git-github/ " curso de Git y Github") de [Platzi](https://platzi.com/ "Platzi")

> UN curso donde aprendi a usar las herrmientas de git y github para el flujo de trabajo
>
> - FM

## En este curso vemos de todo

- Todos los comandos de Git
- El flujo de trabajo en Github
- ELas buenas prácticas
- Trucos
- Creado por el increíble Platzi Team
- Incluye ejemplos en Windows, Linux y Mac
- Disponible para todas las edades

\*\* IGNORAR LA PARTE DE ABAJO (NOTAS)

# git hub comands

    git init =  inicia un repo local de git (archivos locales, storage, repo local git)

    git add . / git add archivo.asd = me agrega los cambios al storage
    git rm --cached archivo.asd = git dejara de seguir tal archivo(!= add)
    git commit -m "asd" = me agrega los cambios al repo local
    git status = stado de los archivos u archivos
    git commit -am "asd" = "commit y add juntos"
    git show = me muestra el historial de cambios
    git log archivo.asd = me muestra el historial de un archivo
    git diff commit.A / git diff commit.A commit.B = compara 1 o 2 commits
    git reset commit.A --soft = vuelve un commit atras del git local
    git reset commit.A --hard = vuelve un commit atras de git y pc
    git merge ramavieja = me trae los cambios de ramavieja a esta
    git remote origin ssh/url = a donde voy a pushear

    git push = me sube al repo de github (en la rama de donde estoy trabajando)
    git fetch = me trae los cambios al repo local de github
    git merge = me trae los cambios a mi archivos locales
    git pull = es fetch y merge juntos (utilizar este)

    git branch = me muestra las ramas
    git branch nuevarama = crea nueva rama (desde donde estoy posicionado)
    git checkout nuevarama = me mueve a la rama nuevarama

# mensajes keys

    ssh-keygen -t rsa -b 4096 -C EMAIL = Creando nuestra llave privada
    luego el passphrase = contrasenia con espacios
    carpeta .ssh = ahi es donde estan nuestras llaves
    eval $(ssh-agent -s) = evaluar si nuestro pc compreuba keys
    cd ~/.algo/ = vamos a la capeta oculta
    ssh-add ~/.algo/idoculto = y lo agregamos al agentKeys

    luego copiar ID publica = y pegarla en nuestro perfil(llaves) de GIT
    git remote set-url origin SSH = cambia nuestro URL por uno con KEY
    git remote origin SSH = usar ese con keys y no el de URL al clonar
    git remote -v = y comprobar

# forma basica de trabajo

    git clone ssh = clona una rama
    git branch nuevarama = crea rama
    git checkout nuevarama = entramos a la nueva arama
    git pull origin main = traer de main (pedira nuestra pass de ssh)
    git pull origin rama = traer la rama que vamos a trabajar
    git add . / git add archivo.asd  = guardar en storage
    git commit -m "asd" = guardar en git local
    git pull origin main/rama = traer de github y comprobar todo ok
    git push orgin master/rama = y por ultimo subir

# CREATE PULL REQUEST

    create pull request = Comentear , reviews , asignar
    cancelar pull = comentar y arreglar
    confirmar request = comentar tips y aceptar

    Los reviews deben comprobar y aprobar los cambios
    *SQUASH Y REBASE MALAS PRACTICAS

    Luego podemos borrar las ramas = una practica opcional

# git VERSIONS tags logs grapash

    git log --graph = para ver las lineas de trabajo
    git log --graph --decorate --oneline = mas comprimido
    alias nombre="git log --graph" = da nombre a los comandos

    git tag -a v0.1 -m "Resultado primeras clases" 13beddb = nos crea tag
    git tag = nos muestra los tag
    git show-ref --tags = nos muestra relacion commit con el tag
    git push origin --tags = le enviamos los tags
    git tag -d nobre = borra el tag de desktop(no github)
    git push origin :refs/tags/dormido = borra el tag de github

# Manejo de ramas

    git branch -d rama = elimina rama git
    git branch -D rama = elimina rama todo
    git show-branch = la historia de vida de todas las ramas
    git show-branch --all = la historia de las ramas con mas datos
    gitk = software de git

# config git

    git config = ver las config de git
    git config --list = ver la data de git
    git config --list --show--original = ver los archivos de git
    git config --global user.name = cambiar usuario
    git config --global user.email = cambiar usuario

# movimiento de carpetas

    ~ = shorcut de nuestra carpeta home
    cd / cd dir:carpeta / cd . / cd.. = movimiento de carpetas
    ls / ls -al / ls -a / ls -l = lista directorios (a ocultos, l lista)
    clear / ctrl + c = limpiar linea de comandos
    pwd = donde estoy parado?
    mkdir = crear carpeta
    touch archivo.asd = crear archivo
    cat archivo.asd = me muestra conteido de archivo
    history = mi historial de cambios
    !id = voy al historial del id del archivo en el (history)
    *rm / rm archivo.asd = elimino archivo o carpetas donde estoy parado
    --help = algun comando y --help me muestra la info del mismo

# Colaboracions forks

    Watch = notificaciones
    Estrella = este prollegto me gusta
    Fork = Copia del estado actual del proy y clonarlo
    Git clone URL
    Git pull reques de ramas a rams entre repos\

    Git remote add upstream URL = nos agrega repo en repo
    git remote -v = nos muestra las fuentes de datos

    git pull upstream main/rama = nos trae la fuente de otra data

# DEPLOYMENT A UN SERVER

    primero servidor = servidor wwe.ejemplo.com
    git clone URL = cloanr primero repo
    Pull request y commits = y se actuializa
    PROTEJER .git - Cuidar
    PROBAR Travis CI  o JENKINS para manejar server FREE

# GIT IGNORE

    .gitignore = archivo para ignorar
    *.jpg = extenciones a ignorar
    LOS BINARIOS = no van en los repos

# README.MD

    Hacer un gran MD
    EDITOR MD online = editor de readme

# GITHUB PAGES

    crear repo usuario.github.io
    git clone URL
    git cd CARPETA
    vim index.html = crea archivo
    git status > add > commit
    git push origin master
    revisar repo
    ir a usuario.github.io (URLde github.pages)
    Ir al repo > Settings > GithubPages > Main Branch > Save
    *Y hacer lo mismo con todos los repos que quieras agregar

# GIT STASH

    Guardar en memoria y hacer comit mas tarde
    EJ:
    git stash = guardo estos cambios
    git stash list = me mmuestra los stash
    git stash pop = sttrae los cambios
    git stash branch RAMA = me lleva el stash a una rama (o rama nueva)
    git stash = para volver atras
    git stash drop = elimina los stash entonces recuperas
    * es bueno para probar cosas
    * cuando tienes mucho trabajo adelantado y queres reveer otras ramas

# GIT CLEAN

    quitar archivos no trakeados y .gitignore
    git clean --dry-run = me va a mostrar los archivos a borrar

# GIT CHERRY

    MALA PRACTICA mejor merge
    git cherry-pick IDcommit= me trae UN commit de otra rama

# GIT AMEND

    git commit -am "alalal" = commit realizado
    hacer cambio q olvidaste
    git commit --amend = te pega los cambios al commit anterior

# GREP y LOG

    Buscar en commits (log) y archivos(grep)
    git grep PALABRA = me muestra los lugars de donde esta
    git grep -n PALABRA = me muestra las lineas
    git grep -c PALABRA = cuantas veces la usamos
    git grep -c "<p>" = para etiquetas
    git log -S "PALABRA" = donde use las palabra en commit

# COMANDOS COLABORATIVOS

    git shortlog = log por persona
    git shortlog -sn = cantidad de commits
    git shortlog -sn --all = y los borrado tambien
    git shortlog -sn --all --no-merges = sin marges

    git config --global alias.stats "git shortlog -sn --all --no-merges"
    git stats = me muestra lo de arriba

    git blame ARCHIVO = ver quien cambio que cosa en tal archivo
    git blame -c ARCHIVO = se ve mejor
    git blame --help = manual del comando blame

    git blame ARCHIVO -L35,53 = quien vambio de tal linea a linea

    git branch = ves ramas actuales de
    git branch -r = ramas remotas en mi server
    git branch -a = Locales y remotas

    * github insigts desde el repo para ver que esta pasando (stats)

# Futuro con GIT y GITHUB

    continuar trabajando con todo lo aprendido
    APRENDER CICLO DE VIDA, MONITOREAR
    APRENDER > TRAVIS o JENKINS
    DEV OPS > AZURE
    GIT LAB > TODO ACA JUNTO
