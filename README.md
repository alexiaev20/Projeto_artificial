Este projeto é um MVP de um Agente de IA especializado em Gastronomia. A solução foca na aplicação prática de Inteligência Artificial através de uma arquitetura robusta, segura e escalável para modelos de negócio SaaS.

Tecnologias Utilizadas
Backend: Python 3.12+ com FastAPI (Assíncrono e de alta performance).

Orquestração de IA: LangChain (Gestão de prompts e contexto).

LLM: OpenAI GPT-3.5/4.

Segurança & Validação: Pydantic para sanitização de dados.

Monitoramento: Logging estruturado para auditoria de segurança.

Diferenciais de Engenharia & Segurança
Este protótipo foi construído com foco em padrões de Produção:

Prompt Hardening (Segurança de Prompt): Implementação de System Messages restritivas para evitar Prompt Injection e garantir que a IA atue estritamente no domínio definido.

Estratégia de Fallback: O sistema possui uma camada de resiliência que, em caso de falha na integração com a IA, entrega uma resposta de contingência, mantendo a disponibilidade do serviço.

Arquitetura Assíncrona: Utilização de async/await para garantir que o servidor não sofra bloqueios durante o tempo de resposta da LLM.

Logging e Auditoria: Rastreabilidade completa de erros e requisições para facilitar o debug e monitorar tentativas de uso indevido.

Como Executar o Projeto
Clone o repositório:

git clone https://github.com/seu-usuario/smart-chef-ai.git
cd smart-chef-ai
Crie e ative o ambiente virtual:



python -m venv venv
# Windows
.\venv\Scripts\activate
# Linux/Mac
source venv/bin/activate
Instale as dependências:

pip install fastapi uvicorn langchain-openai langchain-core pydantic
Inicie o servidor:

python main.py
Acesse a documentação interativa (Swagger): Acesse: http://127.0.0.1:8000/docs

🛠️ Próximos Passos (Roadmap)
[ ] Integração de RAG (Retrieval-Augmented Generation) para consulta de bases de dados privadas.

[ ] Implementação de Streaming de Tokens para melhoria da UX.

[ ] Adição de camada de Cache com Redis para otimização de custos.

[ ] Containerização com Docker.


Desenvolvido por Alexia Melo

