## Guia com comandos básicos do git :desktop_computer:



- Git init: git init **é um comando único que você usa durante a configuração inicial de um novo repositório**. A execução desse comando cria um novo subdiretório . git no diretório de trabalho atual. Essa ação também vai criar uma ramificação principal.

- Git add: O comando git add **adiciona uma alteração no diretório ativo à área de staging**. Ele diz ao Git que você quer incluir atualizações a um arquivo específico no próximo commit. No entanto, git add não tem efeito real e significativo no repositório — as alterações não são gravadas mesmo até você executar git commit .

- Git commit:  comando git commit **captura um instantâneo das mudanças preparadas do projeto no momento**. Os instantâneos com commit podem ser considerados versões "seguras" de um projeto, o Git nunca os altera, a menos que você peça a ele.

- Git Clone:  A partir dele, você clona um código de um repositório para a sua máquina para então começar a trabalhar nele. Pode ser um projeto de uma pessoa da sua empresa, um projeto de colegas da faculdade ou **até mesmo uma aplicação open-source** para a qual você julgou interessante colaborar.

- Git Status: Esse comando esclarece quais arquivos foram alterados e faz uma comparação com relação à ramificação principal.

- Git branch: 

- O **comando “git branch”** cria novas branches. Mas também pode funcionar como uma forma de verificar as ramificações já existentes. 

  Depois de criar uma, você precisa de um “push” para subir essa ramificação. Assim:

  “git push -u <remote> <nome-da-branch>”.

  Por sua vez, para deletar uma branch, use:

  git branch -d <nome-da-branch>



- Git merge: Depois de programar em uma branch, você tem que fazer uma conjunção dela com outras para de fato subir as alterações. É só colocar o nome da branch que desejamos mesclar com a principal depois do termo **merge**.

- Git checkout: 

- O objetivo dele é fazer a pessoa programadora mudar de branch. Você pode usar o “git branch” para saber quais existem e depois trocar de uma para outra. 

  É importante destacar que é preciso fazer um checkout para a master branch quando queremos captar as mudanças de outra ramificação.

- Git Revert: 

  Permite desfazer algum commit e recuperar uma versão saudável, seja localmente, seja remotamente. 

  Para usá-lo, é preciso primeiro executar um “git log -- oneline” para obter o número do hash. Com o hash, então, é possível digitar: **“git revert 'nº do hash'”.**

- Git rm: O git rm é um comando muito útil para remover arquivos do git e parar de monitorá-los, ou seja, de associá-los ao repositório. 

- Git pull: Esse comando traz para a sua máquina todas as mudanças que foram realizadas na plataforma. Ou seja, é uma forma de atualizar a sua versão da aplicação com o que foi alterado remotamente.

- Git stash: O **stash** serve para criar uma pilha de alterações que serão enviadas posteriormente para o repositório. É uma boa forma de guardar algumas mudanças em espera enquanto você muda de branch para trabalhar em outros aspectos do sistema. É ideal para sistemas grandes, com muitas ramificações que demandam essa flexibilidade da pessoa programadora. Exemplo: “git stash”

- Git config: O **config** é um comando inicial para vincular o trabalho no repositório com sua conta no github. Assim, é configurado com o nome e com o e-mail. 

- Git reset: O **reset** é outra forma de voltar ao último estado saudável do seu sistema, uma alternativa ao revert. Funciona assim: “git reset --hard HEAD~1”.

- Git push: O **push** serve para subir as alterações de uma ramificação para um certo repositório. Ele entrega todos os commits e a mensagem. Exemplo: “git push”.