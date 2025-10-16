# ESTUDANDO GITHUB
me aprofundando em git e github

Repositório utilizado para estudos e práticas de 
Git e GitHub


Este é um repositório com os principais e mais importantes códigos que eu sei e aprendi por meio de cursos, leituras e estudo.

## Configurações locais

// listar todas configurações
git config --list

// verificar o usuário
git config --global user.name

// verificar email
git config --global user.email

// configurar seu nome
git config --global user.name "<seu_nome>"

// configurar seu e-mail
git config --global user.email "<seu_email>"

// configurar seu editor padrão
git config --global core.editor "<seu_editor>"

---

## Repositório local

// criar um repositório local
git init

// clonar um repositório remoto
git clone <url_do_repositório>

// verificar status dos arquivos
git status

// adicionar arquivo para o staged
git add <nome_do_arquivo>

// adicionar todas mudanças de uma vez
git add .

// comitar com mensagem
git commit -m "<mensagem_do_commit>"

---

## Trabalhando com branches

// listar todas as branches
git branch

// criar nova branch
git branch <nome_da_branch>

// mudar para outra branch
git checkout <nome_da_branch>

// criar e mudar para nova branch
git checkout -b <nova_branch>

// deletar uma branch
git branch -d <nome_da_branch>

---

## Logs

// ver todos commits
git log

// ver commits com mais detalhes
git log --decorate

// ver commits de uma pessoa específica
git log --author="<nome_da_pessoa>"

// ver em ordem alfabética quem fez commits e quantos
git shortlog

// ver só a quantidade de commits por pessoa
git shortlog -sn

// ver graficamente os commits nas branches
git log --graph

// ver modificações de um commit específico
git show <hash_do_commit>

---

## Diferenças (Diff)

// ver mudanças antes de commitar
git diff

// ver só os nomes dos arquivos modificados
git diff --name-only

---

## Desfazendo coisas

// desfazer última mudança antes do staged
git checkout <nome_do_arquivo>

// remover arquivo do staged
git reset HEAD <nome_do_arquivo>

// voltar para um commit (mantendo arquivos modificados)
git reset --soft <hash_do_commit>

// voltar para um commit (apagando arquivos do staged)
git reset --mixed <hash_do_commit>

// voltar para um commit (apagando tudo, até as alterações)
git reset --hard <hash_do_commit>

// apagar um commit específico (sem perder histórico)
git revert <hash_do_commit>

---

## Stash (guardar mudanças temporariamente)

// guardar alterações não commitadas
git stash

// listar os stashes
git stash list

// aplicar stash mais recente
git stash pop

// apagar todos os stashes
git stash clear

---

## Repositórios remotos

// conectar repositório local com remoto
git remote add origin <url_do_repositório>

// ver endereço do repositório remoto
git remote -v

// alterar o endereço do repositório remoto
git remote set-url origin <url_do_repositório>

// enviar tudo para o repositório remoto
git push -u origin <nome_da_branch>

// baixar tudo do repositório remoto
git pull origin <nome_da_branch>

---

## Merge e conflitos

// mesclar branch atual com outra
git merge <nome_da_branch>

// abortar merge com conflito
git merge --abort

---

## Outros comandos úteis

// ver as diferenças entre branches
git diff <branch_1> <branch_2>

// limpar arquivos não versionados
git clean -f

// ver arquivos não rastreados
git ls-files --others --exclude-standard
