# Comandos GIT
Os Tipos se resumem em feat, fix, refactor, style, chore, doc e test
#### feat são quaisquer adições ao código. Enquanto elas podem alterar parte do código já existente, o foco dela é a implementação de features novas ao ecossistema.
#### fix: refere-se às correções de bugs. Caso seu time trabalhe com issues ou com Jira, é possível com smart commits associar seu commit a uma issue e alterar seu estado com keywords como resolve, fix, solves. Em geral, essas marcações devem vir na descrição ou no footer.
refactor refere-se a quaisquer mudanças que atinjam o código, porém não alterem sua funcionalidade. Alterou o formato de como é processamento em determinada parte da sua tela, mas manteve a mesma funcionalidade? Declare como refactor.
Alterações referentes a formatações de código, semicolons, trailing spaces e lint em geral são em style.
Em uma das equipes com que trabalho, decidimos por criar novos dois tipos e ignorar o tipo chore porque ele não passava a ideia que precisávamos e passamos a utilizar outros dois: env e project. Vale notar que esses dois tipos fogem das especificações do conventional commit. Em project, todo o escopo de versões e pacotes ficam inseridos nele, por exemplo:
## Configurações
#### Listar
sh
git config --list

#### Editar
sh
git config --global user.name "99039091"
git config --global user.email alexsandro.nunes@sop.ce.gov.br

#### Salvar usuário e senha permanente
sh
git config --global credential.helper cache

## Branch
#### Criando uma nova branch localmente
sh
git branch <nome-do-branch>

#### Criando uma branch remoto
sh
git push origin <nome-do-branch>

#### Verificar todas branch remoto
sh
git fetch --all

#### Listando branch
sh
git branch

#### Deletando branch
sh
git branch -d <nome-do-branch>

#### Mudar branch
 sh
git checkout <nome-do-branch>

## Merge
#### Fundir uma branch para outra
 sh
git merge <nome-do-branch>

## Log
#### Consultar log simples
 sh
git log

#### Consultar reflog simples
 sh
git reflog
git reflog  show HEAD

#### Mostrar em apenas uma linha
 sh
git log --stat
git log -p
git log --oneline

## Criar Chave SSH Windons
####
 sh
ssh-keygen