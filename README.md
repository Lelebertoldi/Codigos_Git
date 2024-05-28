
# Treinamento DIO de Git e GitHub

## Lins úteis

- [Formatação GitHub](https://docs.github.com/pt/get-started/writing-on-github/working-with-advanced-formatting/organizing-information-with-tables)

- [Configuração Git](https://git-scm.com/docs)


## Comandos Principais Git




|Código | Resultado|
|---|---|
|git config --global user.name + "user name" | cria username|
|git config --global user.email + email | criar email de usuário|
|git config --global user.name | verifica usuario|
|git config --global user.email | verifica email|
|git config --global init.defaultBranch + nome da branch | muda nome da branch padrao (padrao main ou master)|
|git config init.defaultBranch | retorna o nome da branch padrao|
|git config --global --list | mostra todas as configuraçoes globais|
|git clone + URL | adiciona repositorio do GitHub (pede token, gerar token em GitHub - Developer Settings)|
|git clone + URL + nome de novo diretorio | cria nova pasta e clona o repositorio nela|
|git config --global credential.helper + store ou cache | store salva suas credenciais no PC, cache nao salva|
|git config --global credential.helper | retorna se credencial esta salva ou nao (store ou cache)|
|git config --global --show-origin credential.helper | mostra local de armazenamento das credenciais |
|mkdir + nome da pasta | cria novo repositorio (make diretory)|
|cd + nome da pasta | entra na pasta (tab ajuda a completar nome da pasta)|
|cd .. | volta para pasta anterior|
|git init | inicia git na pasta (cria repositorio git local)|
|touch + nome do arquivo (base - README.md) | cria arquivo vazio|
|git status | mostra o status dos arquivos|
|git config | mostra toda a configuração|
|ctrl + L ou clear | limpa terminal|
|ls | lista todo o conteudo do local|
|cat config | mostra arquivo responsavel pelas configuraçoes do repositorio (cat exibe conteudo)|
|git remote -v | mostra os repositorios remotos que esta vinculado |
|git remote add + nome do repositorio remoto (padrao origin) + URL | conecta repositorio local com repositorio remoto|
|git clone + URL + --branch + nome da branch + --single-branch | clona apenas a branch especifica (sem nome da branch ele clona a branch main)|
|git add + nome do arquivo | adiciona arquivo existente ao git|
|git commit -m"nome do commit"| cria comit (prepara para enviar para remoto)|
|git remote add origin + URL |registra o repositório remoto e adiciona o endereço em “origin”|
|git log | mostra commit pronto |
|git push -u origin main ou master|encaminha as mudanças commitadas para o GitHub|



### Observações

- **quando o local termina em (main), esta no repositorio principal, quando termina em (GIT_DIR!) esta dentro do diretorio**

- **a pasta .git fica oculta**



