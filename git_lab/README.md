# Configuraçao
`git config --global user.name "<nome>"` Define nome de quem commita

`git config --global user.email "<email noreplay>"` Define email de quem esta commitando

`git init` Cria um repositorio git 

`git branch -M main` Define main com a branch defealt    

`git remote add origin <caminho do repositorio>` Vincula com o github    

# Comandos basicos
---
`git init` para definir a pasta como repositorio git

`git add <pasta ou arquivo>` para colocar em staged 

`git commit -m <arquivo>` para commitar e salvar a alteraçao

`git status` verifica o status da pasta e mostra mudanças e possiveis açoes (restore, remove, add)

`git restore --staged <arq>` retira o arquivo da area de staged

`git restore <arq>` recupera a versão commitada do git repository

`git log` traz os logs de alterações dos arquivos
> Apresenta uma arvore com as modificaçoes      
> `git log --oneline --graph --all`     

`git commit --amend` permite editar a mensagem do ultimo commit realizado

`git checkout <hash>` permite momentaneamente voltar para o ponto de salvamento anterior

`git branch` mostras as ramificaçoes existentes do codigo

`git branch <nome da ramificaçao>` cria uma ramificaçao do codigo, isso isola as alteraçoes de outras ramificaçoes

`git branch -d <branch>` para deletar, mas com o **d** minusculo ele verificara se a impacto, com **D** maiusculo ele deleta sem verfiicação

`git branch -b <branch>` cria a branch e ja muda a ramificaçao para ela

`git checkout <nome da ramificaçao>` direciona seu ambiente de codigo para essa ramificaçao

`git checkout` mostra em qual ramificaçao voce esta

`git merge <branch>` realiza o merge da branch com a main (a main sempre ira existir, sendo a principal do programa "*produção*")

`git reset --hard <hash>` **EVITAR AO MAXIMO**, pois ele retorna a um ponto anterior do commit e deleta sem recuperação os commits posteriores a ele

#### Publicaçao e Atualização do repositorio local

`git push -u origin <branch para o qual fara o push>` Publica no repositorio

`git push --set-upstream origin feature-2` Faz a publicação 
na a feature-2 (caso nao exista ele cria)
> `-u` == `--set-upstream`

`git push origin --all` Faz publicaçao de todas as branchs

`git pull `