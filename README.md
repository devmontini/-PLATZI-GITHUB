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

    git push = me sube al repo de github (en la rama de donde estoy trabajando)
    git fetch = me trae los cambios al repo local de github
    git merge = me trae los cambios a mi archivos locales
    git pull = es fetch y merge juntos (utilizar este)


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
