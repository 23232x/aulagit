# GIT E GITHUB

-- setando usuário:
git config --local user.name "23232x"
git config --local user.email "23232x@gmail.com"

# 1 INICIANDO O REPOSITÓRIO:

- git init.

# 2 ADICIONANDO O CONTEÚDO:

- git add index.html

# 3 FAZENDO O COMMIT:

- git commit - m "adicionando landing page"

# GIT STATUS:

- Possibilita ver o status dos arquivos.

# OBS:

- para cada alteração de arquivo -e necessário rodar o seguinte comando:

* git add pagina.html

- para criar o ponto na história usa-se o commit

* git commit -m "alteração pagina.html"

# VERIFICAR AS MUDANÇAS FEITAS NO PROJETO

- git log ( para pegar o identificador do commit, algo parecido com isso? 9bb39a6c14c0c3ce478ccf926aae143b8a2f9204)

# REVISAR PONTOS E VERIFICAR OQUE FOI FEITO:

-git show
Mostra as alteraçãoes

- git show 9bb39a6c14c0c3ce478ccf926aae143b8a2f9204
  para um commit especifico

# COMEÇANDO OUTRA VERSÃO DO PROJETO:

- uma branch: significa ramificação
  quando se esta na branch(ramificação) MASTER, pode-se criar ramificações alternaticas,

# CRIANDO NOVA BRANCH; (cada branch é uma nova linha do tempo)

- Cria-se nova branch para criar novas funcionalidades, ex, cliente pediu para adicionar carrinho de compras.
- para criar nova branch e acessa-la:
- 1 git branch nomeDaBranch
- 2 git checkout nomeDaBranch
- 3 git status (para certificar-se que realmente esteja na nova branch)
- 4 cria-se oque vc quiser, ex: touch card.html
- 5 git checkout master (volta para a branch MASTER)
- 6 git branch (possibilita ver todas as branch's, ou linhas do tempo)
- BRANCH MASTER : onde geralmente fica nosso projeto em produção

# UNINDO BRANCHS COM MERGE(unindo linhas do tempo)

- Na branch master rode o comando abaixo, onde branch é a que voce quer unir.
  git merge branchSecundaria.

# DELETAR BRANCH:

- git branch -D nomeDaBranch
- git branch - Para checar se a branch foi deletada.

# RESUMO

1 - git init: // inicia a linha do tempo(histórico)
2 - git add: // adiciona ou atualiza mudanças para irem para a linha do tempo.
3 - git commit: // adiciona um ponto na linha do tempo
4 - git log: // visualiza os pontos na linha do tempo(commit)
5 - git status : //informa o estado das alterações do nosso projeto.
6 - git show: // apresenta determinado ponto na história.

#### 2º PARTE - COLOCAR O PROJETO NA NUVEM

Explicação:
Primeiramente foi criado um reposiório local, agora vamos criar um repositório na nuvem, no gitHub.

1 - Crie um repositorio no gitHub.
2 -

- git remote add origin https://github.com/23232x/aulagit.git
  3 - git remote -v - para ver meus repositórios remotos.
  4 - Realize o primeiro 'Push'.
  è o carinha que vai empurrar nosso repositório local para meu repositório na nuvem, no gitHub

* git branch -M main
* git push -u origin main (somente da 1º vez, depois somento git push)
  Para Visualizar nossos arquivos no gitHub, acesse a aba <>code;

## ADD NOVOS ITENS APÓS O PRIMEIRO PULL

- 1 git add nome do arquivo.html
  OU
  git add . (vai adicionar todas as alterações que estivem dentro da pasta)
- 2 git commit -M "commitando tudo através do pontinho"
- 3 git push

## SALVAR USER.NAME, USER.EMAIL###

Para não ficar digitando sempre o usuário e senha do gitHub, utiliza-se o seguinte comando: Usuário e senha fica gravado

- git config credential.helper store
