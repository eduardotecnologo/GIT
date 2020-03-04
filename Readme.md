# Estudo sobre comando do Git e Github

## \* PALESTRA SOBRE GIT E GITHUB

## \* Configuração Inicial

- **Comando**

- » git config --global user.name "Eduardo Alexandre"
- » git config --global user.email "eduardotecnologo@hotmail.com"
- » git config --global color.ui true **//Colore as interações executadas**

## \* Os 3 estágios

- **Comando**
- » mkdir pastaestudos **//Cria uma nova pasta**
- » cd pastaestudos
- » touch file.txt **Cria um arquivo .txt**
- » git init **//Inicia o git**
- » git status **Mostra o PRIMEIRO Estágio do git "Untracked files" arquivos ainda não versionados**
- » git add file.txt **SEGUNDO Estágio adiciona o arquivo file.txt para ser versionado**
- » git status **Mostra os arquivos que já podem ser commitados "Changes to be commited", pronto para o controle de versão**
- » git commit -m "meu primeiro commit" **Arquivo no TERCEIRO Estágio, agora o arquivo já está fazendo parte do controle de versão**
