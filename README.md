Iniciando Curso de Git para Iniciantes

1 - Como funciona
    Por que usar Git e GitHub? <br>
    Resposta: Ter uma forma fácil de gerenciar o código fonte da aplicação, do sistema, do produto. <br>
    Trabalhando em equipe. <br>
    <a href="https://www.alura.com.br/artigos/o-que-e-git-github">Link para aprofundamento</a> <br> <br>
    

    comendos básicos <br><br>
    git <br>
    commit <br>
    pull <br>
    push <br>

2 - Instalando o Git
    Acesse o site do git e baixe o instalador.
    <a href="https://git-scm.com/">Git</a>


3 - Configurando o Git
    git config --global user.name "Ederson Programador"
    git config --global user.email "edersonprogramadorfullstack@outlook.com"
    git config --global core.editor vscode

    git config user.name
    git config user.email
    git config --list

4 - Iniciando um Repositório
    cd
    ls
    dir
    mkdir
    cd ../

    git init

5 - Branch - README - Commit
    git status
    <!-- ^ Pode adicionar um arquivo por vez ou todos de uma vez com "git add -A" -->
    <!-- ~~ Criar arquivo README.md -->
    <!-- git add README.md adiciona somente esse arquivo -->
    git add README.md
    <!-- git add -A adiciona todos os arquivos -->
    git add -A
    git commit -m "Texto descritivo"
    git log

6 - Revertendo modificações
    git branch
    <!-- ^ com git commit -am você não precisa fazer o git add -A para alvar pois o mesmo já salva e envia. -->
    git commit -am "Adiciona e altera"
    git reset --soft
    git reset --mixed
    git reset --hard