📚 Template Next.js para Teste de Tecnologia

Este ambiente foi configurado para ser a base de desenvolvimento do SIG-Manutenção, seguindo as diretrizes de desempenho e usabilidade exigidas na disciplina de Projeto Integrado I do curso de Sistemas e Mídias Digitais da UFC.

🛠️ Stack Tecnológico Frontend

Next.js (App Router): Framework moderno para renderização híbrida (SSR/SSG/ISR/CSR).

React: Biblioteca para construção de interfaces de usuário.

TypeScript: Adição de tipagem estática para código mais robusto e menos propenso a erros.

ShadCN/UI (Via Tailwind CSS): Biblioteca de componentes para garantir acessibilidade e design coeso.

💻 Configuração e Desenvolvimento Local

Siga estes passos para clonar o repositório e iniciar o ambiente de desenvolvimento.

1. Clonagem e Instalação de Dependências

Clone o repositório e navegue até a pasta:

# Se o projeto ainda não foi clonado:
# git clone [URL_DO_SEU_REPOSITORIO]

cd sig-manutencao-frontend # Ou o nome da pasta do seu projeto

# Instale as dependências. Recomendamos o 'npm' ou 'yarn'
npm install
# ou
yarn install


2. Rodando o Servidor de Desenvolvimento

Inicie o Next.js em modo de desenvolvimento. Isso permitirá que o código seja recompilado automaticamente a cada alteração (Hot Reloading).

npm run dev
# ou
yarn dev


O projeto estará acessível em http://localhost:3000.

💡 Estrutura de Arquivos Principal

O desenvolvimento das interfaces deve ser realizado primariamente na pasta app.

app/page.tsx: Componente principal, representando a página inicial.

app/layout.tsx: Estrutura de layout global (onde ficam a tipografia, componentes de tema e o _app.js do Next.js legado).

components/: Diretório para componentes reutilizáveis (e.g., botões, cards, barras de navegação).

styles/: Arquivos CSS globais ou de configurações de estilo.

🔗 Integração com o Backend

O Frontend se comunicará com o servidor API (Node.js/Express.js) através de chamadas HTTP (API RESTful), geralmente implementadas via fetch ou bibliotecas como Axios.

Certifique-se de que a API esteja rodando no endereço correto, conforme configurado nas variáveis de ambiente.

☁️ Deploy

A sugestão para o deploy contínuo é através da Vercel (dos criadores do Next.js), que oferece integração direta com o GitHub.