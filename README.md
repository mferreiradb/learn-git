**CONTROLE DE VERSÕES DO CÓDIGO**

- identificação, para que possa sinalizar o autor das mudanças realizadas no repositório.

    		git config --global user.name "Nome do usuario"
	
    		git config --global user.email e-mail@exemplo.com

**REPOSITÓRIO GIT**

- Local onde as informações e os objetos do projeto serão mantidos

	- Iniciar um repositório git na raiz do projeto

 			git init

 *STAGE*
 
- Nele são adicionadas as alterações do código

- Este é apenas um intermediário, as alterações ainda não estão adicionadas ao repositóro

	- Adicionar um arquivo determinado ao `stage`
	
        	git add <arquivo>
		
	- Adicionar todos os arquivos ao `stage`
	
        	git add .
        
- Adiciona os arquivos ao repositório
        
		git commit -m "Mensagem"
	
	- O parãmetro `-m` permite escrever uma mensagem que descreve o que foi feito
	- O commit irá gerar um código e este códgo identifica a versão


- Mostra as mudanças feitas no arquivo
    
		git diff

- Cria uma nova branch e altera para a criada

		git checkout -b [nome da branch]

- "Puxa" uma branch

		git merge [nome da branch]

*BRANCH*

- Ramificação do projeto principal

- Pode ser usada para realizar testes, de forma que não irá afetar o progeto principal

	- Mostrar todas as branchs
    
    		git branch

- Altera para a branch nomeada

		git checkout [nome da branch]

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
