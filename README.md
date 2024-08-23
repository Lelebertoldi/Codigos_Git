
# Treinamento DIO de Git e GitHub

---
> Anotações para uso pessoal sobre os comandos mais úteis do Git do conteúdo aprendido nas aulas da DIO 

## Lins úteis

- [Formatação GitHub](https://docs.github.com/pt/get-started/writing-on-github/working-with-advanced-formatting/organizing-information-with-tables)

- [Blog GitHub](https://github.blog/)

- [Configuração Git](https://git-scm.com/docs)

- [Editar README online](https://readme.so/pt)

- [Badges para GitHub](https://github.com/Ileriayo/markdown-badges)

- [Mais Badges para GitHub](https://dev.to/envoy_/150-badges-for-github-pnk)

- [Mais Badges para GitHub 2](https://github.com/digitalinnovationone/dio-lab-open-source/blob/main/utils/badges/badges.md)

- [Gerador de Badges](https://shields.io/)




## Comandos Principais do Git




|Código | Resultado|
|---|---|
|`git config --global user.name + "user name"` | cria username|
|`git config --global user.email + email` | criar email de usuário|
|`git config --global user.name` | verifica usuario|
|`git config --global user.email` | verifica email|
|`git config --global init.defaultBranch + nome da branch` | muda nome da branch padrao (padrao main ou master)|
|`git config init.defaultBranch` | retorna o nome da branch padrao|
|`git config --global --list` | mostra todas as configuraçoes globais|
|`git clone + URL` | adiciona repositorio do GitHub (pede token, gerar token em GitHub - Developer Settings)|
|`git clone + URL + nome de novo diretorio` | cria nova pasta e clona o repositorio nela|
|`git config --global credential.helper + store ou cache`| store salva suas credenciais no PC, cache nao salva|
|`git config --global credential.helper` | retorna se credencial esta salva ou nao (store ou cache)|
|`git config --global --show-origin credential.helper` | mostra local de armazenamento das credenciais |
|`mkdir + nome da pasta` | cria novo repositorio (make diretory)|
|`cd + nome da pasta` | entra na pasta (tab ajuda a completar nome da pasta)|
|`cd ..` | volta para pasta anterior|
|`git init` | inicia git na pasta (cria repositorio .git local)|
|`touch + nome do arquivo (base - README.md)` | cria arquivo vazio|
|`git status` | mostra o status dos arquivos|
|`git config` | mostra toda a configuração|
|`ctrl + L ou clear` | limpa terminal|
|`ls` | lista todo o conteudo do local|
|`cat config` | mostra arquivo responsavel pelas configuraçoes do repositorio (cat exibe conteudo)|
|`git remote -v` | mostra os repositorios remotos que esta vinculado |
|`git remote add + nome do repositorio remoto (padrao origin) + URL` | conecta repositorio local com repositorio remoto|
|`git clone + URL + --branch + nome da branch + --single-branch` | clona apenas a branch especifica (sem nome da branch ele clona a branch main)|
|`git diff`| mostra mudanças feitas antes de add|
|`git diff --staged`| mostra mudanças feitas após add, antes de commit|
|`git add + nome do arquivo ou .` | adiciona arquivo existente ao git, ou . para todos arquivos|
|`git commit -m"nome do commit"`| cria comit (prepara para enviar para remoto)|
|`git remote add origin + URL` |quando criar repositorio vazio no GitHub para apenas add os arquivos do pc|
|`git branch -M main` | quando repositorio nao é main, força a ser|
|`git log` | mostra commit pronto (Q para sair) |
|`git push -u origin main ou master`|encaminha as mudanças commitadas para o GitHub|
|`rm -rf .git (ou outro)` | remove repositorio git da pasta |
|`git restore + nome do arquivo` | restaura arquivo, descartando todas as mudanças locais feitas |
|`git commit --amend -m"nova mensagem"` | altera mensagem do commit anterior|
|`git commit --amend` | abre editor, apertar i para inserir, para sair esc:w(para escrever)q(pra sair) |
|`git reset --soft + log do commit` | volta o ultimo commit para area de preparação (antes de commit)|
|`git reset --mixed + log do commit` | volta o ultimo commit para arvore de trabalho (antes de add)|
|`git reset --hard + log do commit` |apaga completamente o commit|
|`git reset + nome do arquivo ou --staged + nome do arquivo`| reseta arquivo para antes de add |
|`git pull` | baixa atualizaçoes do arquivo remoto|
|`echo + "texto" > + local`| cria texto dentro do arquivo (local), tambem serve para add diretorio ou arquivo dentro de arquivo ou diretorio|
|`git checkout -b + nova branch` | cria e troca local do git para nova branch|
|`git checkout + branch`| muda para outra branch existente|
|`git branch -v` | lista o ultimo commit de cada branch|
|`git merge + nome da outra branch` | mescla outra branch com a branch aberta no git|
|`git branch`| lista as branches do repositorio, o * mostra qual esta aberta no git|
|`git branch -d + nome da branch` | deleta branch|
|`git fetch` | baixa alteraçoes do repositorio remoto sem mesclar com remoto atual|
|`git fetch origin main` | baixa alteraçoes do repositorio remoto sem mesclar com remoto atual|
|`git diff origin/main` | mostra diferenças do repositorio remoto baixado e repositorio atual|
|`git merge origin/main` |mescla os 2 arquivos|
|`git stash`| arquiva ultima modificaçao do arquivo antes do add, para usar em outra branch|
|`git stash list` | lista modificaçoes arquivadas|
|`git stash apply` | volta a modificaçao arquivada|
|`git stash pop`| exclui modificaçao arquivada mais recente da pilha|
|`git remote add upstream + URL`|adiciona a URL apenas para download (pull), mas nao para upload (push)|
|`git pull upstream main`| baixa do diretorio principal adicionado em upstream (ex: quando feito fork baixa da URL original, e nao da minha copia)|
|`git pull origin main`| baixa do diretorio principal adicionado em origin (ex: quando feito fork baixa da minha copia, e nao da URL original)|
|`git lfs install`|Instala o LFS (Large File Storage) (Precisa fazer o download do arquivo exe antes)|
|`git lfs uninstall`|desinstala o LFS (Large File Storage)|
|`git lfs track "*.mp4" (ou outra extensão de arquivos grandes)`|Adiciona a extensão de arquivo grande ao LFS para poder fazer upload de arquivos maiores|
|`git lfs untrack "*.mp4" (ou outra extensão de arquivos grandes)`|Remove a extensão de arquivo grande ao LFS para poder fazer upload de arquivos maiores|
|`git lfs migrate info`|No caso de erro do push no LFS, verifica arquivos do erro|
|`git lfs migrate import --include="*.mp4" (ou outra extensão de arquivos grandes)`|No caso de erro do push dizendo que o arquivo contém mais de 100mb|
|`git lfs clone + URL`|Clona arquivos grandes com maior velocidade|
|`git lfs pull`|Usar se o pull normal falhar em baixar os arquivos lfs, também aumenta velocidade de pull|
|`git diff --cached`|Compara as mudanças com o repositório local|
|`git reset HEAD~`|Reseta para antes do último commit, pode ser usado mais de uma vez para resetar varios commit na fila |

> [!IMPORTANT]
>- **Quando o local termina em (main), esta no repositorio principal, quando termina em (GIT_DIR!) esta dentro do diretorio**
>
>- **A pasta .git fica oculta**
>
>- **Quando entrar em log, diff ou algo parecido, apertar Q para sair**
>
>- **Para usar o editor Web do GitHub similar ao VSCode aperte a tecla . dentro do repositório**
>
>- **Branches são ramificações do projeto, assim podendo testar algo sem comprometer o arquivo original ou anterior, podendo voltar atrás, no log mostra todas as branches criadas ate o momento**






