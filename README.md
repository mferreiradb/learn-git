**CONTROLE DE VERSÕES DO CÓDIGO**

    git config --global user.name "Nome do usuario"
    git config --global user.email e-mail@exemplo.com
        - identificação, para que possa sinalizar o autor das mudanças realizadas no repositório.

**REPOSITÓRIO GIT**

- Local onde as informações e os objetos do projeto serão mantidos
	- Iniciar um repositório git na raiz do projeto

 			git init

 *STAGE*
 
    - Nele são adicionadas as alterações do código
    - Este é apenas um intermediário, as alterações ainda não estão adicionadas ao repositóro
        git add <arquivo>
        git add .

*git commit*
        
    - Adiciona os arquivos ao repositório
        git commit -m "Mensagem"
            - O parãmetro *-m* permite escrever uma mensagem que descreve o que foi feito
            - O commit irá gerar um código e este códgo identifica a versão

*git diff*
    - Mostra as mudanças feitas no arquivo
    
*git checkout -b [nome da branch]*

    - Cria uma nova branch e altera para a criada
	
*git checkout*

    - Altera a branch

*git merge [nome da branch]*

    - "Puxa uma branch"

*BRANCH*

    - Ramificação do projeto principal
    - Pode ser usada para realizar testes, de forma que não irá afetar o progeto principal
        * Libs
        * Frameworks
        * Novas funcionalidades
    git branch <nome>

*git checkout [nome da branch]*

    - Altera para a branch nomeada

**VINCULO AO GITHUB**

- Vincula o repositório local ao remoto

		git remote add origin https://meu-endereco.com/meu-projeto.git

- Retorna os repositórios remotos vinculados

		git remote -v

- Remove determinado arquivo do stage;

		git rm --cached script.js

- Desvincular um repositório remoto

		git remote rm <nome>

- Deletar branch local

		git branch -d <branch>

- Deletar branch remota
	
		git push origin --delete <branch>
