# Guia Fundamental do GitHub: Da Teoria à Prática :computer:   
![GitHub - Marcos-Vitor123/git-e-github: Curso da Alura - formação](https://repository-images.githubusercontent.com/422031746/245484d7-7c89-4aed-92e4-e5cc6341ef9e)








Este é um projeto modelo estruturado como um README.md profissional. Ele serve tanto como um guia prático para iniciantes quanto como um exemplo de documentação limpa, organizada e visualmente atraente para o seu portfólio.

## Índice
1. Objetivo
2. Tecnologias Utilizadas
3. Estrutura das Pastas
4. Guia de Comandos e Execução
5. Dicas Rapidas

## Objetivo
O principal objetivo deste projeto é desmistificar o uso do **_Git e do GitHub_** para novos desenvolvedores. Ele centraliza os conceitos essenciais de controle de versão, fluxos de trabalho colaborativos e boas práticas de documentação, permitindo que qualquer pessoa entenda como subir e gerenciar seus códigos de forma profissional.

## Tecnologias Utilizadas
#### Abaixo estão as principais ferramentas e linguagens abordadas neste guia para estruturar e validar os conceitos de desenvolvimento:

TECNOLOGIA|FINALIDADE|NÍVEL DE CONHECIMENTO
----------|----------|----------------------------------------------------------
Git | Controle de versão local e histórico de alterações | Básico
GitHub	    |Hospedagem de código na nuvem e colaboração        |	Básico
Markdown	  |Formatação e estilização desta documentação	      |Básico
Python	    |Linguagem de script utilizada no exemplo prático	  |Básico
---------------------------------------------------------------------------------

## Estrutura das Pastas
Uma estrutura de diretórios organizada é fundamental para a manter um projeto de software. Veja como este repositório está desenhado:



## Guia de Comandos e Execução
### 1. Comandos do Terminal (Navegação Local)
Antes de mexer com código, você precisa saber se mover no terminal do seu sistema operacional:

~~~bash
Bash
# Criar uma pasta para o projeto
mkdir meu-projeto-github
# Entrar na pasta criada
cd meu-projeto-github
# Verificar o caminho atual do diretorio
pwd
~~~

### 2. Comandos Git (Controle de Versão)
Aqui está o fluxo clássico para iniciar um repositório e enviar suas alterações para o GitHub:

~~~bash
Bash
# Inicializar o repositorio git local
git add + (nome do arquivo) ou  git add .
# Grava as alterações localmente com uma mensagem descritiva
git commit -m +(Mensagem descritiva) ex: "Inicializamos o projeto"
# Conecta o seu repositório local ao repositório remoto no GitHub
git remote add origin + https://github.com/seu-usuario/seu-repositorio.git
# Envia os arquivos para branch principal (main) no GitHub
git branch -m main
git push -u origin main
~~~

### 3. Código em Python (Exemplo Prático)
Para testar a execução do projeto, incluímos um script simples em src/main.py que simula uma saudação ao ambiente Git:

~~~Python
# src/main.py

def saudar_dev(nome):
    print(f"Olá, {nome}! Bem-vindo ao mundo do controle de versão.")
    print("Seu ambiente Python e Git está funcionando perfeitamente!")

if __name__ == "__main__":
    usuario = input("Digite seu nome de desenvolvedor: ")
    saudar_dev(usuario)
~~~
### como executar o script

~~~Bash
python src/main.py
~~~

### Dicas rapidas Git e Github
Principais comandos do **_git_** [Clique aqui](https://github.com/rodrigosantiago-fap/aponti-testes-de-software-turma-18-rodrigo-santiago/blob/main/GitHub-Modulo-01/Exercicio-PROJETO-GITHUB/dicas%20de%20git.pdf)

### Site do GitHub
Clique [aqui](https://github.com/?locale=pt-br) para acessar a página do **GitHub**.

### Link pra baixar Git
Clique [aqui](https://git-scm.com/install/) para acessar a página do **_Git_** e baixar o app **_Gitbash_**.

## Autor
Desenvolvido por Seu Rodrigo Santiago

**GitHub:** [@rodrigosantiago-fap](https://github.com/rodrigosantiago-fap)

**LinkedIn:** [Rodrigo Santiago](https://www.linkedin.com/feed/)

**Email:** rodrigo2026fap@gmail.com
