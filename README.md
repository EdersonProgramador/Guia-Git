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

7 - Trabalhando com diferentes Branches

    <!--^ Para visualizar em qual branch você está digite o comando abaixo -->
git branch
<!--^ Para criar um branch digite git branch + nome do novo branch, por exemplo o git brach teste -->
git branch teste
<!--^ Para trocar de branch utiliza-se o git checkout + o nome do branch-->
git checkout teste
<!--^ Para voltar para versão principal digite git checkout master -->
git checkout master

<!-- ^ Como deletar a branch atual -->

git branch -d NomeDaBranchAqui

<!-- ^ Para renomear a sua atual branch local, execute o comando branch com a opção -m , passando o novo nome.
 -->
git branch -m main


8 - Diferença entre arquivos

<!-- * Saber quais arquivos foram adicionados, alterado, ou deletados antes de comitar os arquivos. -->
git status
git diff
git diff --name-only
git checkout main -- Nome de um arquivo

9 - Criando um repositório no git Github

<!-- * Generating a new SSH key and adding it to the ssh-agent for windowns -->

<a href="https://docs.github.com/pt/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent#platform-windows">Generating a new SSH key</a>

Use git bach: Terminal específico para git.

ssh-keygen -t rsa -b 4096 -C "edersonprogramadorfullstack@outlook.com"


10 - Conectando o repositorio local ao remoto

<!-- ^ …or create a new repository on the command line -->

echo "# SitedePortif-lio" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/EdersonProgramador/mude-aqui-o-repositorio.git
git push -u origin main

<!-- ^ …or push an existing repository from the command line -->

git remote add origin https://github.com/EdersonProgramador/mude-aqui-o-repositorio.git
git branch -M main
git push -u origin main