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
