# Estudo sobre comandos do Git e Github

## \* PALESTRA - conceitos SOBRE GIT E GITHUB

## \* Configuração Inicial

- **Comando**

- » edudeveloper@Eduardo-MacBook-Pro  git config --global user.name "Eduardo Alexandre"
- » git config --global user.email "eduardotecnologo@hotmail.com"
- » git config --global color.ui true **//Colore as interações executadas**

## \* Os 3 estágios

- **Comandos**
- » mkdir pastaestudos **//Cria uma nova pasta**
- » cd pastaestudos
- » touch file.txt **Cria um arquivo .txt**
- » git init **//Inicia o git**
- » git status **Mostra o PRIMEIRO Estágio do git "Untracked files" arquivos ainda não versionados**
- » git add file.txt **SEGUNDO Estágio adiciona o arquivo file.txt para ser versionado**
- » git status **Mostra os arquivos que já podem ser commitados "Changes to be commited", pronto para o controle de versão**
- » git commit -m "meu primeiro commit" **Arquivo no TERCEIRO Estágio, agora o arquivo já está fazendo parte do controle de versão**

## \* Realizando os primeiro commit

- **Comandos**
- » mkdir pastaestudos **//Cria uma nova pasta**
- » cd pastaestudos
- » touch file.js **Cria um arquivo file.js**
- » file.js **Preparando para entrar no Primeiro Commit**
- » git commit -m "descrição do commimt" **Descrição sobre o commit realizado**
- » git log **Exibe toda a descrição do commit**
- » touch file.css **Cria um novo arquivo file.css**
- » git status **Irá mostrar os 2 arquivos criados para serem adicionados**
- » ▶ git add . **Adiciona os 2 arquivos ou mais, prontos para serem commitados**
- » **Sacada** git commit -a -m "descrição" **O -a substitui a função do **add** com esse comando vc adiciona e commita ao mesmo tempo**

## \* Verificando Logs

- **Comandos**
- » ▶ git log **Mostra os log do commit**
- » ▶
  » commit 7dc02b788xxxxxxxxxxxxxxxxxxa5fde0c (HEAD -> master, origin/master, origin/HEAD)
 - » Author: eduardotecnologo <eduardotecnologo@hotmail.com>
 - » Date:   Wed Mar 4 11:19:52 2020 -0300
 - »     Realizando os primeiro commit.

- » ▶ git log -p **Faz uma comparação, mostrando tudo o que foi alterado**
- » ▶ git log **Pasando o -2 vc limita em apenas os 2 ultimos commits**
- » ▶ git log --stat **Este mostra os logs mais as estatisticas de cada linha alterada**
 - » Readme.md | 17 +++++++++++++++--
 - » 1 file changed, 15 insertions(+), 2 deletions(-)

- » ▶ git log --pretty=oneline **Mostra apenas informações do que foi feito em apenas uma linha**
- » ▶ git log --pretty=format: "%h - %an, %arr : %s"**Mostra as informações formatadas de forma resumidas**
  - » Author: eduardotecnologo <eduardotecnologo@hotmail.com>
- » Date:   Wed Mar 4 10:51:39 2020 -0300
    - » Formatando texto.
- » ..skipping...
- » xxxxxxx - eduardotecnologo, 9 days agor : Realizando os primeiro commit.
- » xxxxxxx - eduardotecnologo, 9 days agor : Realizando os primeiro commit
- » xxxxxxx - eduardotecnologo, 9 days agor : Os 3 estágios
- » xxxxxxx - eduardotecnologo, 9 days agor : Formatando texto..
- » xxxxxxx - eduardotecnologo, 9 days agor : Formatando texto.
- » xxxxxxx - eduardotecnologo, 9 days agor : Formatando texto
- » xxxxxxx - eduardotecnologo, 9 days agor : Init

- » ▶ git log --since=2.days**Mostra as informações de commits realizados em d-2**

## \* Setando o .gitignore
- » touch .gitignore **Cria um arquivo .gitignore, neste arquivo vc adiciona todos os arquivos e pastas que vc deseja que o git ignora e não suba para o githube**

## \* Fluxo de commits
- » ▶ git reset HEAD arquivo.txt **Volta ao estágio anterior ao ultimo estágio antes de ser commitado**
 - » Untracked files:
- » ▶ git checkout xxxxxxxxxxxxxxxxxxxxxxxxxxxx **Cada commit tem um hash único, para voltar uma versão use o sguinte commit**
 - » detached from xxxxxxxx:
- » ▶ git brnach
- » ▶ ls **Você verá que seus commits voltaram a um versão anterior**
- » ▶ git reset HEAD~1 **Volta 1 commmit, com 2 volta 2 e assim qtos queizer**
- » ▶ git reset HEAD~1 --soft **Volta um commit mas matem o arquivo que foi criado para ser commitado com as alterações novamente**
- » ▶ git reset HEAD~1 --hard **Volta um commit e remove as alterações do arquivo (CUIDADO!!!)**

## \* Trabalhando com Branch
 - » ▶ edudeveloper@Eduardo-MacBook-Pro  ~/Documents/Git/GIT   master
 - » ▶ git checkout -b formcadastro **Criando uma nova branch**
 - » ▶ edudeveloper@Eduardo-MacBook-Pro  ~/Documents/Git/GIT   formcadastro
- » ▶ git checkout master **Volta pra branch master**