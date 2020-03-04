# Estudo sobre comando do Git e Github

## \* PALESTRA - conceitos SOBRE GIT E GITHUB

## \* Configuração Inicial

- **Comando**

- » git config --global user.name "Eduardo Alexandre"
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
- » git add . **Adiciona os 2 arquivos ou mais, prontos para serem commitados**
