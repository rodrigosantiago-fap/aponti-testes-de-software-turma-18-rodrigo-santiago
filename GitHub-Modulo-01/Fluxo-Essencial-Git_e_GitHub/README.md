1. Criar um ## Repositório
O repositório (ou "repo") é a pasta onde o Git vai rastrear as alterações do seu projeto.

No GitHub (Remoto)
Acesse o GitHub e clique no botão "+" (no canto superior direito) -> New repository.

Dê um nome ao repositório, escolha se será Public ou Private e clique em Create repository.

Na sua Máquina (Local)
Abra o terminal na pasta do seu projeto e junte o seu código local ao GitHub:

Bash
# Inicializa o Git na pasta local
git init

# Adiciona os arquivos para serem salvos
git add .

# Cria o primeiro ponto de salvamento
git commit -m "Primeiro commit"

# Conecta o seu Git local ao repositório do GitHub (mude o link para o seu)
git remote add origin https://github.com/seu-usuario/seu-repositorio.git

# Envia o código para o GitHub
git push -u origin main
2. Utilizar Commits
Um commit é como um "checkpoint" ou uma foto do estado atual do seu código. Sempre que fizer uma alteração importante, faça um commit.

Bash
# 1. Veja o que mudou no projeto
git status

# 2. Adicione as mudanças para a "fila de salvamento" (Staging Area)
git add nome-do-arquivo.txt   # Para um arquivo específico
git add .                    # Para todos os arquivos modificados

# 3. Salve a alteração com uma mensagem explicativa
git commit -m "Adiciona funcionalidade de login"
3. Trabalhar com Branches
Branches (ramos) servem para você desenvolver novas funções sem mexer ou estragar o código principal que já está funcionando (main).

Bash
# Criar uma nova branch e já entrar nela
git checkout -b nova-funcionalidade

# Para ver em qual branch você está trabalhando
git branch

# Para voltar para a branch principal
git checkout main

# Para enviar a sua nova branch para o GitHub
git push origin nova-funcionalidade
4. Abrir Pull Requests (PR)
O Pull Request é o momento em que você avisa ao time (ou a si mesmo) que terminou uma tarefa na sua branch e quer juntá-la à branch principal (main).

Vá até a página do seu repositório no GitHub.

Um botão amarelo costuma aparecer automaticamente: "Compare & pull request". Clique nele.

Adicione um título e uma descrição breve do que você fez.

Clique em Create pull request.

Se estiver tudo certo (e sem conflitos), clique em Merge pull request para juntar o código.

5. Resolver Conflitos
Um conflito acontece quando duas pessoas (ou você em branches diferentes) mudam a mesma linha do mesmo arquivo e o Git não sabe qual versão escolher.

Como resolver:
Ao tentar dar um git merge ou atualizar o código, o Git vai avisar que há um conflito.

Abra o arquivo conflitante no seu editor de código (como o VS Code).

Você verá marcações como estas direto no texto:

Plaintext
<<<<<<< HEAD
Meu código lindo que fiz na minha branch.
=======
Código que um colega alterou e já estava na main.
>>>>>>> main
Ação: Apague as linhas de marcação (<<<<<<<, =======, >>>>>>>) e escolha qual texto deve ficar (ou combine os dois).

Salve o arquivo e finalize no terminal:

Bash
git add .
git commit -m "Resolve conflito no arquivo X"
git push origin sua-branch
🚀 Resumo do Fluxo Diário
Se estivesse trabalhando em equipe ou em um projeto organizado, seu dia a dia seria exatamente assim:
git checkout -b minha-tarefa ➔ Cria código ➔ git add . ➔ git commit -m "Mapeia dados" ➔ git push origin minha-tarefa ➔ Abre Pull Request no GitHub.
