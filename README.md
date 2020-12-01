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
-

##### PEGANDO UM PROJETO JÁ INICIADO, PARA TRABALHAR COM O TIME

1 - selecione o projeto e selecione a opção 'clone or download', copie o link "https://github...."

#### VOLTAR ARQUIVOS PARA UMA DETERMINADA LINHA DO TEMPO

1 - git log // para ver o momento que se squer voltar da linha do tempo(branc).
2 - git checkout commit ba1abf8af55d75e4a4e68397efdd4579dd9d889b -- arquivoRecuperar

## RECUPERAR ALGO DELETADO ##### (pesquisar mais formas de recuperar)

- git checkout -- arquivoDeletado

## APAGOU ARQUIVO, FAZENDO COMMIT E GIT PULL

- Mesmo deletando um arquivo e fazeno o commit e fazendo pull, é possivel restaurar um arquivo deletado.
  1 - git log : pegue o commit que o arquivo ainda existia.
  2- git checkout 17c9e5b2330f86112dfb04fae833a840da7a5bc1 -- arquivoDeletado (PRONTO- arquivo restaurado)

# RESUMO

git pull : tras os arquivos que estão remoto
git push: envia os arquivos que estão na máquina local para o servidor remoto.

1 - git init // inicia a linha do tempo(histórico)
2 - git add // adiciona ou atualiza mudanças para irem para a linha do tempo.
3 - git commit // adiciona um ponto na linha do tempo
4 - git log // visualiza os pontos na linha do tempo(commit)
5 - git status //informa o estado das alterações do nosso projeto.
6 - git show // apresenta determinado ponto na história.
7 - git branch // gerencia novas linhas do tempo
8 - git checkout //consegue sair e entrar de uma branch para outro
9 - git merge //unir linhas do tempo (branch's)
10 - git push // envia alterações locais para o repositório remoto.
11 - git pull // tras os arquivos atualizados da nuvem ou gitHub
12 - git clone //clonar para nossa máquina um repositório já iniciado, e que esta na nuvem.
13 - git pull // puxa os arquivos da nuvem, sincroniza com a nossa máquina os arquivos locais com a da nuvem, comando após o git clone.
14 - git checkout -b teste // cria uma nova brach e acessa ela(faz checkout).
15 - git commit -am "update sem o add" //adiciona e faz o commit
