# Git

Dicas e comandos para trabalhar com GIT

## Git comandos:

- Historico:
<br><br>
git lag : Mostrar todos commits
<br>
git lag -p <file> : Mostrar mudanças de arquivo especifico
<br>
git blame <file> : Mostrar quem e quando alterou arquivo

<br><br><br>

- Atualizar e Publicar:
<br><br>
git remote -v: Lista todos os controles remotos configurados atualmente
<br>
git remote show <remote>: Mostrar infos sobre um controle remoto
<br>
git remote add <shortname> <url>: Adiciona um novo repositorio remoto, denominado <remote>
<br>
git fetch <remote>: Baixar as alterações mas nao marcar/integrar direto no HEAD
<br>
git pull <remote> <branch>: Baixar as alterações e marcar/integrar direto no HEAD
<br>
git push <remote> <branch>: Publicar alterações locais remotamente
<br>
git branch -dh <remote/branch>: Excluir filial no controle remoto
<br>
git push --tags: Publicar tags

<br><br><br>

- Mudançãs Locais:
<br><br>
git status: Arquivos alterados no diretorio de trabalho
<br>
git diff: Mudanças em arquivos rastreados
<br>
git add . : Adiciona todas as mudanças
<br>
git add . -p <file>: Adiciona mudanças no <file>
<br>
git commit -a "": Confirma todas as alterações locais em arquivos rastreados
<br>
git commit: Confirma alterações previamente preparadas
<br>
git commit --amend: Mude o ultimo commit

<br><br><br>

- Branches:
<br><br>
git branch -av: Lista todas as branchs existentes
<br>
git checkout <branch>: Mudar ramo HEAD
<br>
git checkout <new-branch>: Cria uma nova branch com base
<br>
git checkout --track <remote/branch>: Cria branch nova com o local
<br>
git branch -d <branch>: Deleta branch
<br>
git tag <tag-name>: Marca o commit atual com uma tag

<br><br><br>

- Desfazer:
<br><br>
git reset -hard HEAD: Descarta todas as mudanças locais em seu diretorio de trabalho
<br>
git checkout HEAD <file>: Descarta as alterações locais em arquivo especifico
<br>
git revert <commit>: Reverte um commit (produzindo novo commit com mudanças contrarias)
<br>
git reset -hard <commit>: Redefine o ponteiro HEAD para um commit anterior... e descarta todas as alterações desde entao.
<br>
git reset <commit>: ... e preserva todas as mudançãs não planejadas
<br>
git reset -keep <commit>: ...e preserva as mudançãs locais não comprometidas

<br><br><br>

- Fundir e Rebase:
<br><br>
git merge <branch>: Funda <branch> em seu HEAD atual
<br>
git rebase <branch>: Rebase seu HEAD atual em <branch>
<br>
git rebase --abort: Aborta um rebase
<br>
git rebase --continue: Continua um rebase apos resolver conflitos
<br>
git mergetool: Usa a ferramente de fusão configurada para resolver conflitos
<br>
git add <resolved-file> , git rm <resolved-file>: Use o editor para resovler conflitos manualmente e (após resolver) marca o arquivo como resolvido
