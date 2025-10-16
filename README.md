# ESTUDANDO GIT E GITHUB
#Repositório Criado para estudos e práticas de Git e GitHub
<img align="left" width="59" height="300" alt="83b91c4c-2dbc-4a04-a6a8-9211806c43df" src="https://github.com/user-attachments/assets/65877a9e-e45d-4e11-854f-0b1210a291f8" />


=======================
# COMANDOS BASICOS DO GIT 

# ⚙️ Configurações Locais 

### Listar todas as configurações
git config --list

### Verificar o usuário
git config --global user.name

### Verificar o e-mail
git config --global user.email

### Configurar seu nome
git config --global user.name "<seu_nome>"

### Configurar seu e-mail
git config --global user.email "<seu_email>"

### Configurar seu editor padrão
git config --global core.editor "<seu_editor>"

# 📁 Repositório Local

### Criar um repositório local
git init

### Clonar um repositório remoto
git clone <url_do_repositório>

### Verificar status dos arquivos
git status

### Adicionar arquivo para o staged
git add <nome_do_arquivo>

### Adicionar todas as mudanças de uma vez
git add .

### Comitar com mensagem
git commit -m "<mensagem_do_commit>"

# 🌿Trabalhando com Branches
### Listar todas as branches
git branch

### Criar nova branch
git branch <nome_da_branch>

### Mudar para outra branch
git checkout <nome_da_branch>

### Criar e mudar para nova branch
git checkout -b <nova_branch>

### Deletar uma branch
git branch -d <nome_da_branch>

# 🧾Logs
### Ver todos os commits
git log

### Ver commits com mais detalhes
git log --decorate

### Ver commits de uma pessoa específica
git log --author="<nome_da_pessoa>"

### Ver em ordem alfabética quem fez commits e quantos
git shortlog

### Ver só a quantidade de commits por pessoa
git shortlog -sn

### Ver graficamente os commits nas branches
git log --graph

### Ver modificações de um commit específico
git show <hash_do_commit>

# 🔍 Diferenças (Diff)
### Ver mudanças antes de commitar
git diff

### Ver só os nomes dos arquivos modificados
git diff --name-only

# 🔄 Desfazendo Coisas
### Desfazer última mudança antes do staged
git checkout <nome_do_arquivo>

### Remover arquivo do staged
git reset HEAD <nome_do_arquivo>

### Voltar para um commit (mantendo arquivos modificados)
git reset --soft <hash_do_commit>

### Voltar para um commit (apagando arquivos do staged)
git reset --mixed <hash_do_commit>

### Voltar para um commit (apagando tudo, até as alterações)
git reset --hard <hash_do_commit>

### Apagar um commit específico (sem perder histórico)
git revert <hash_do_commit>

# 📦 Stash (Guardar Mudanças Temporariamente)
### Guardar alterações não commitadas
git stash

### Listar os stashes
git stash list

### Aplicar stash mais recente
git stash pop

### Apagar todos os stashes
git stash clear

# 🌐 Repositórios Remotos
### Conectar repositório local com remoto
git remote add origin <url_do_repositório>

### Ver endereço do repositório remoto
git remote -v

### Alterar o endereço do repositório remoto
git remote set-url origin <url_do_repositório>

### Enviar tudo para o repositório remoto
git push -u origin <nome_da_branch>

### Baixar tudo do repositório remoto
git pull origin <nome_da_branch>

# 🧩Merge e Conflitos
### Mesclar branch atual com outra
git merge <nome_da_branch>

### Abortar merge com conflito
git merge --abort

# 🧰 Outros Comandos Úteis
### Ver as diferenças entre branches
git diff <branch_1> <branch_2>

### Limpar arquivos não versionados
git clean -f

### Ver arquivos não rastreados
git ls-files --others --exclude-standard

=====================

