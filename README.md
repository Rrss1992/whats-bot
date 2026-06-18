# 🤖 WhatsApp Multi-Bot IA

Um bot de WhatsApp com múltiplas personalidades construído em Node.js. O sistema utiliza a inteligência artificial do Google Gemini para ler o contexto das mensagens e assumir diferentes personagens dentro de grupos.

## ✨ Funcionalidades (Features)

* **ValVal (O Viking):** Uma IA focada em Valheim. Responde dúvidas, dá dicas de construção, conta histórias nórdicas e possui um sistema integrado de *Web Scraping* para buscar e traduzir automaticamente as últimas atualizações da Steam.
* **Roketo (O Smurf Tóxico):** Um assistente focado em Rocket League. Mantém o tom de humor sarcástico, lê arquivos de "dossiê" local para zoar os amigos de forma personalizada e consulta a API do Tracker Network.
* **Nitro (O Agente Inteligente):** Um assistente geral de alta performance. Especialista em responder perguntas sobre atualizações, notícias e conhecimentos gerais, blindado contra tentativas de injeção de prompt e com formatação adaptativa para textos longos.
* **DJ YouTube:** Um sistema de busca integrado nativamente com o YouTube para encontrar vídeos e músicas rapidamente dentro do WhatsApp.
* **Proteções:** Inclui sistema Anti-Spam (Cooldown), tratamento de reconexão automática e blindagem contra *Prompt Injection*.

## 🛠️ Tecnologias Utilizadas

* **Node.js** (Linguagem base)
* **Baileys** (Conexão e roteamento do WhatsApp Web via Sockets)
* **Google Generative AI / Gemini** (Cérebros das personalidades)
* **RSS Parser** (Leitura de Feeds da Steam)
* **Play-dl** (Buscador do YouTube)
* **Express** (Servidor HTTP de suporte para hospedagem)

## 🚀 Como rodar o projeto localmente

### Pré-requisitos
* Node.js instalado na máquina.
* Uma chave de API gratuita do Google Gemini (Google AI Studio).

### Passo a passo

1. Clone este repositório no seu computador:
   ```bash
   git clone [https://github.com/SEU_USUARIO/SEU_REPOSITORIO.git](https://github.com/SEU_USUARIO/SEU_REPOSITORIO.git)

1. Entre na pasta do projeto e instale as dependências:
cd SEU_REPOSITORIO
npm install

2.Crie um arquivo chamado .env na raiz do projeto e configure suas variáveis de ambiente:
GEMINI_API_KEY=sua_chave_do_gemini_aqui
ID_GRUPO_VALHEIM=id_do_grupo_aqui@g.us
ID_GRUPO_ROCKET=id_do_grupo_aqui@g.us

3. Inicie o servidor:
npm start

4. O terminal exibirá um QR Code. Escaneie-o com o seu WhatsApp para conectar o motor do bot.