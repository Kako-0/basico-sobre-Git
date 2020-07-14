#Git Course
Aprendendo a usar o git e o github.

#Comandos essenciais para usar o Git
    
1. > git init
    Após criar um diretório para o seu projeto, usando o terminal com o path desse diretório, digite essa linha de comando para criar um novo repositório do git a partir desse diretório. 

2. > git status
    Esse comando serve para lhe informar como está o seu repositório, reportando os arquivos que acabaram de ser criados (_untracked_), adicionado (_unmodified_), modificados ou removidos (_modified_).

3. > git add --all 
ou 
> git add <nome-do-arquivo.extensão>
    Usado para adicionar os arquivos que criou para a área _staged_, área que deixa os arquivos pronto para dar o commit.

4. > git commit -m "mensagem"
    Esse comando salva os arquivos em seu repositório local junto com uma mensagem de commit. É importante, sempre colocar uma mensagem pertinente as modificações que você fez a fim de entendimento posterior de terceiros e até mesmo o seu.

5. > git log
    Usado para mostrar o histórico de alterações dos arquivos do repositório, informando: O hash do commit, o autor, a data de modificação e a mensagem do commit.
    Outro jeito de ver o histórico seria com:
    > git shortlog
    Onde este, mostra os autores, quantos commits fizeram e quais foram esses commits.

6. > git show <hash-do-commit>
    Com esse comando você poderá ver, a partir das hashs vistas no comando log, as modificações feitas naquele commit.