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

- git show 9bb39a6c14c0c3ce478ccf926aae143b8a2f9204

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
