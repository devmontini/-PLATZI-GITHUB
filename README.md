# config git

    git config
    git list
    git config --list --show--original
    git config --global user.name
    git config --global user.email

# git hub comands

    git init =  inicia un repo local de git (archivos locales, storage, repo local git)

    git add . / git add archivo.asd = me agrega los cambios al storage
    git rm --cached archivo.asd = git dejara de seguir tal archivo(!= add)
    git commit -m "asd" = me agrega los cambios al repo local
    git status = stado de los archivos u archivos
    git commit -am "commit y add juntos"
    git show = me muestra el historial de cambios
    git log archivo.asd = me muestra el historial de un archivo
    git diff commit.A / git diff commit.A commit.B = compara 1 o 2 commits

    git push = me sube al repo de github (en la rama de donde estoy trabajando)
    git fetch = me trae los cambios al repo local de github
    git merge = me trae los cambios a mi archivos locales
    git pull = es fetch y merge juntos (utilizar este)


    git branch nuevarama = crea nueva rama (desde donde estoy posicionado)
    git checkout nuevarama = me mueve a la rama nuevarama

# movimiento de carpetas

    cd / cd dir:carpeta / cd . / cd..
    ls
    ls -al
    ls -a
    ls -l
    clear / ctrl + c
    pwd
    mkdir
    touch
    cat
    history
    !id
    rm
    --help
