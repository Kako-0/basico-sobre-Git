#Git Course
Aprendendo a usar o git e o github.

#Comandos essenciais para usar o Git
    
1. `git init`
    Após criar um diretório para o seu projeto, usando o terminal com o path desse diretório, digite essa linha de comando para criar um novo repositório do git a partir desse diretório. 

2. `git status`
    Esse comando serve para lhe informar como está o seu repositório, reportando os arquivos que acabaram de ser criados (_untracked_), adicionado (_unmodified_), modificados ou removidos (_modified_).

3. `git add --all`
ou 
`git add <nome-do-arquivo.extensão>`
    Usado para adicionar os arquivos que criou para a área _staged_, área que deixa os arquivos pronto para dar o commit.

4. `git commit -m "mensagem"`
    Esse comando salva os arquivos em seu repositório local junto com uma mensagem de commit. É importante, sempre colocar uma mensagem pertinente as modificações que você fez a fim de entendimento posterior de terceiros e até mesmo o seu.

5. `git log`
    Usado para mostrar o histórico de alterações dos arquivos do repositório, informando: O hash do commit, o autor, a data de modificação e a mensagem do commit.
    Outro jeito de ver o histórico seria com:
    `git shortlog`
    Onde este, mostra os autores, quantos commits fizeram e quais foram esses commits.

6. `git show <hash-do-commit>`
    Com esse comando você poderá ver, a partir das hashs vistas no comando log, as modificações feitas naquele commit.

7. `git diff <commit-1><commit-2>`
    Compara os dois commit e mostra as alterações feitas entre eles. Ao usar esse comando sem os parâmetros, ele mostra as modificações do último arquivo salvo.
    `git diff --name-only`
    Mostra apenas o nome dos arquivos modificados.

8. `git checkout <nome-do-arquivo.extensão>`
    Desfaz alterações feitas no arquivo ainda que está

9. `git reset`
    Esse comando possui três modos:
    `git reset --soft <hash-do-commit-anterior-ao-que-quer-ser-resetado>`
        Esse parâmetro reseta o arquivo no ponto antes de ser commitado.
    `git reset --mixed <hash-do-commit-anterior-ao-que-quer-ser-resetado>`
        Esse parâmetro reseta o arquivo no ponto antes de ser adicionado no estágio _staged_.
    `git reset --hard <hash-do-commit-anterior-ao-que-quer-ser-resetado>`
        Esse parâmetro é o mais bruto, já que apaga por completo o commit.
    Esse comando deve ser usado com bastante cuidado, visto que ele altera o histórico do repositório.