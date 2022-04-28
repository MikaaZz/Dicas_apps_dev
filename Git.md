# Git

Dicas e comandos para trabalhar com - GIT

## Git comandos:

### Historico:

- git lag : Mostrar todos commits

- git lag -p <file> : Mostrar mudanças de arquivo especifico

- git blame <file> : Mostrar quem e quando alterou arquivo

### Atualizar e Publicar:

- git remote -v: Lista todos os controles remotos configurados atualmente

- git remote show <remote>: Mostrar infos sobre um controle remoto

- git remote add <shortname> <url>: Adiciona um novo repositorio remoto, denominado <remote>

- git fetch <remote>: Baixar as alterações mas nao marcar/integrar direto no HEAD

- git pull <remote> <branch>: Baixar as alterações e marcar/integrar direto no HEAD

- git push origin <branch>: Publicar alterações locais remotamente

- git branch -dh <remote/branch>: Excluir filial no controle remoto

- git push --tags: Publicar tags



### Mudançãs Locais:

- git status: Arquivos alterados no diretorio de trabalho

- git diff: Mudanças em arquivos rastreados

- git add . : Adiciona todas as mudanças

- git add . -p <file>: Adiciona mudanças no <file>

- git commit -m "": Confirma todas as alterações locais em arquivos rastreados

- git commit: Confirma alterações previamente preparadas

- git commit --amend: Mude o ultimo commit



### Branches:

- git branch -av: Lista todas as branchs existentes

- git checkout <branch>: Mudar ramo HEAD

- git checkout <new-branch>: Cria uma nova branch com base

- git checkout --track <remote/branch>: Cria branch nova com o local

- git branch -d <branch>: Deleta branch

- git tag <tag-name>: Marca o commit atual com uma tag



### Desfazer:

- git reset -hard HEAD: Descarta todas as mudanças locais em seu diretorio de trabalho

- git checkout HEAD <file>: Descarta as alterações locais em arquivo especifico

- git revert <commit>: Reverte um commit (produzindo novo commit com mudanças contrarias)

- git reset -hard <commit>: Redefine o ponteiro HEAD para um commit anterior... e descarta todas as alterações desde entao.

- git reset <commit>: ... e preserva todas as mudançãs não planejadas

- git reset -keep <commit>: ...e preserva as mudançãs locais não comprometidas



### Fundir e Rebase:
- git merge <branch>: Funda <branch> em seu HEAD atual

- git rebase <branch>: Rebase seu HEAD atual em <branch>
- git rebase --abort: Aborta um rebase

- git rebase --continue: Continua um rebase apos resolver conflitos

- git mergetool: Usa a ferramente de fusão configurada para resolver conflitos

- git add <resolved-file> , - git rm <resolved-file>: Use o editor para resovler conflitos manualmente e (após resolver) marca o arquivo como resolvido
