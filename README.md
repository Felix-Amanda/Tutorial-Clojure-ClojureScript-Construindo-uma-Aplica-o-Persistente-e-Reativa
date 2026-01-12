# Trabalho-em-Clojure-

1. Nome do Aluno: 
Amanda Cristina Roxo Felix

2. Link do Tutorial: 
https://profsergiocosta.notion.site/Tutorial-Clojure-ClojureScript-Construindo-uma-Aplica-o-Persistente-e-Reativa-2a5cce975093807aa9f0f0cb0cf69645

3. Descrição do Projeto: 
Este projeto é uma aplicação web de Lista de Tarefas (Todo App) construída em ClojureScript, utilizando uma abordagem funcional para o desenvolvimento. Ele representa uma solução full-stack, pois engloba tanto o servidor de backend (Clojure) para manipulação de dados quanto o front-end (ClojureScript) para composição de componentes reativos e estado imutável. 
O projeto está estruturado em três componentes principais para formar uma aplicação completa:

Frontend (ClojureScript): Responsável pela interface do usuário e pela camada de apresentação. Utiliza o paradigma funcional para gerenciar o estado imutável e renderizar a aplicação de forma reativa no navegador.

Backend (Clojure): Atua como o servidor de aplicação. É responsável por expor as endpoints necessárias para que o frontend realize operações de leitura, escrita e exclusão de dados.

Persistência de Dados (Banco de Dados/Simulação): Esta é a camada de dados do projeto. É responsável por armazenar permanentemente as tarefas, utilizando um mecanismo de persistência ou 
simulação (conforme o tutorial) para garantir que os dados sejam mantidos entre as sessões. É gerenciada exclusivamente pelo Backend.

3.1 Funcionalidades:
Adicionar novas tarefas.
Marcar tarefas como concluídas/incompletas (Toggle).
Excluir tarefas da lista.
Persistência de dados (geralmente usando localStorage ou equivalente, conforme o tutorial).

3.2 Tecnologias Utilizadas:
ClojureScript: Linguagem de programação.
Shadow-CLJS: Ferramenta de build e servidor de desenvolvimento para ClojureScript.
HTML/CSS: Estrutura e Estilização.
Node.js/NPM: Gerenciamento de dependências.

4. Instruções de Execução:  
Para que a aplicação funcione, é necessário ter o ambiente de desenvolvimento configurado e executar dois processos simultaneamente.

4.1 Pré-requisitos: 
Certifique-se de ter instalado no sistema:
Java Development Kit (JDK): Versão 8 ou superior.
Node.js e NPM: Para gerenciamento de dependências.
clj (Clojure CLI): A ferramenta oficial da linha de comando do Clojure.

4.2 Configuração e Inicialização: 
Siga os passos na sequência a partir do terminal.
  
   Clonar e Navegar:
Baixe o código-fonte do repositório Git e navegue para a pasta do projeto.
"git clone [https://github.com/Felix-Amanda/Trabalho-em-Clojure-.git](https://github.com/Felix-Amanda/Trabalho-em-Clojure-.git)
cd Trabalho-em-Clojure-"
   
   Instalar Dependências:
Instale as dependências do Node.js/NPM, que são necessárias para o Shadow-CLJS e outras ferramentas de front-end.
"npm install"
   
   Iniciar os Servidores (DOIS TERMINAIS):
A arquitetura full-stack requer dois processos paralelos. Abra duas janelas de terminal separadas na pasta raiz do projeto.
  
   Terminal 1: Backend (Clojure) - Servidor de Aplicação: Inicie o servidor que irá gerenciar a lógica de negócios e a persistência de dados.
"clj -M:run"
   
   Terminal 2: Frontend (Shadow-CLJS) - Servidor de Build: Inicie a ferramenta que compila o código ClojureScript para JavaScript e mantém uma conexão de hot-reloading para desenvolvimento em tempo real.
"npx shadow-cljs watch app"
   
   Acessar a Aplicação:
Após a inicialização bem-sucedida de ambos os servidores, o front-end estará disponível. Abra o seu navegador e acesse o endereço padrão:
"http://localhost:8000"

A aplicação estará funcional e pronta para uso.

