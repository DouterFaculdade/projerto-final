# Comandos para adicionar este projeto ao repositório https://github.com/DouterFaculdade/api-vue.git

# 1. Inicialize o repositório (se ainda não estiver inicializado)
git init

# 2. Adicione o repositório remoto (se ainda não adicionou)
git remote add origin https://github.com/DouterFaculdade/api-vue.git

# 3. Adicione todos os arquivos para commit
git add .

# 4. Faça um commit com uma mensagem
git commit -m "Projeto clima Vue: primeira versão"

# 5. Envie para o branch principal (main ou master, conforme o repositório)
git branch -M main
git push -u origin main

# Se aparecer erro "non-fast-forward" ou "tip of your current branch is behind":
# O repositório remoto já tem commits que não estão no seu repositório local.
# Para resolver, faça um pull com rebase e depois tente o push novamente:

git pull --rebase origin main
git push -u origin main

# Se houver conflitos, resolva-os, faça git add nos arquivos corrigidos e continue o rebase:
# git add <arquivo>
# git rebase --continue

# Se aparecer "Invalid username or password" ou "Authentication failed":
# 1. Gere um Personal Access Token (PAT) no GitHub: https://github.com/settings/tokens
#    - Marque os escopos "repo" e "workflow" (ou apenas "repo" para projetos privados).
# 2. Use o token como senha ao fazer push:
#    - Quando o terminal pedir usuário, use seu nome de usuário do GitHub.
#    - Quando pedir senha, cole o token gerado.

# Alternativamente, configure o remote para já incluir o token (NÃO RECOMENDADO para ambientes compartilhados):
# git remote set-url origin https://<USUARIO>:<TOKEN>@github.com/DouterFaculdade/api-vue.git

# Recomenda-se usar um gerenciador de credenciais (credential manager) ou o GitHub CLI para facilitar o login:
# gh auth login
