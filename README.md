**CONTROLE DE VERSÕES DO CÓDIGO**

    git config --global user.name "Nome do usuario"
    git config --global user.email e-mail@exemplo.com
        - identificação, para que possa sinalizar o autor das mudanças realizadas no repositório.

**REPOSITÓRIO GIT**

- Local onde as informações e os objetos do projeto serão mantidos

    git init - Inicia um repositório git na raiz do projeto

    STAGE
        - Nele são adicionadas as alterações do código
        - Este é apenas um intermediário, as alterações ainda não estão adicionadas ao repositóro
            git add <arquivo>
            git add .

    git comiit - Adiciona os arquivos ao repositório
            git commit -m "Mensagem"
                - O parãmetro *-m* permite escrever uma mensagem que descreve o que foi feito
                - O commit irá gerar um código e este códgo identifica a versão
    git diff - Mostra as mudanças feitas no arquivo

    BRANCH
        - Ramificação do projeto principal
        - Pode ser usada para realizar testes, de forma que não irá afetar o progeto principal
            * Libs
            * Frameworks
            * Novas funcionalidades
        git branch <nome>
    git checkout master
            - descarta a branch e retorna para a versão principal

**VINCULO AO GITHUB**

    $ git remote add origin https://meu-endereco.com/meu-projeto.git
        - Vincula o repositório local ao remoto
    git remote -v
        - Retorna os repositórios remotos vinculados

    git rm --cached script.js - Remove o arquivo script.js do stage;

**Desvincular um repositório remoto**

	git remote rm <nome>
