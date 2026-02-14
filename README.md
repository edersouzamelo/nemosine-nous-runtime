# 🧠 Nemosine Nous ©

## ⚙️ AME Hardened Baseline (v0.8.3-AME)

Este repositório passou a incluir uma Executable Minimal Architecture (AME) com hardening completo (H0–H6.1), executável, determinística e auditável, na qual o motor de linguagem (LLM) é explicitamente subordinado a um orquestrador externo.

Este baseline AME é:
- Executável (não apenas conceitual)
- Determinístico e não-agentic
- Auditável via registro estrutural append-only
- Persistente (registro em JSONL)
- Projetado como fundação arquitetural, não como produto final

IMPORTANTE:
A AME não é um agente autônomo, não decide fluxo e não governa o sistema.
Trata-se de uma arquitetura mínima executável hardened, usada como base técnica.

Estado AME hardened ancorado no tag: v0.8.3-AME

------------------------------------------------------------

## 🧪 PoC Oficial – API ChatGPT-4o (FastAPI + React)

Este repositório contém também a Prova de Conceito oficial do Sistema Cognitivo Modular Nemosine Nous, demonstrando comunicação direta entre:

- Backend FastAPI (Python)
- Frontend React
- API externa de linguagem (OpenAI ChatGPT-4o)
- Orchestrator determinístico
- Registro persistente de ciclos
- Isolamento seguro da API Key via .env

A PoC representa o fluxo cognitivo mínimo funcional do Nemosine Nous quando acoplado a um motor externo de linguagem.

Inclui endpoints estruturais adicionais:
- /chat
- /ame/last
- /ame/tail
- /ame/stats
- /health

------------------------------------------------------------

## 🚀 Tecnologias Utilizadas — Backend

- Python 3.11
- FastAPI
- Uvicorn
- python-dotenv
- OpenAI / ChatGPT-4o API
- Registro persistente JSONL (append-only)

------------------------------------------------------------

## 🎨 Tecnologias Utilizadas — Frontend

- React
- Vite
- Axios
- CSS (Dark Theme personalizado)
- Painel técnico de inspeção de ciclos

------------------------------------------------------------

## 📁 Estrutura Geral do Projeto

nemosine-PoC-api-4o/
│
├── backend/
│   ├── ame/
│   │   ├── orchestrator.py
│   │   ├── registry.py
│   │   ├── motor_openai.py
│   │   ├── models.py
│   │   └── config.py
│   ├── data/
│   │   └── ame_cycles.jsonl
│   ├── main.py
│   ├── requirements.txt
│   └── .env (não incluído)
│
├── frontend/
│   ├── public/
│   ├── src/
│   └── package.json
│
└── README.md

------------------------------------------------------------

## ▶️ Como Rodar Localmente

1) Backend (FastAPI)

Comandos:
cd backend
pip install -r requirements.txt
uvicorn main:app --reload --port 8000

Criar arquivo .env:
OPENAI_API_KEY=your_key_here

------------------------------------------------------------

2) Frontend (React)

Comandos:
cd frontend
npm install
npm run dev

Acessar:
http://localhost:5173

------------------------------------------------------------

## 📄 Licença

Nemosine Nous © – Todos os direitos reservados.
Uso permitido apenas para fins de demonstração, estudo ou colaboração autorizada.

------------------------------------------------------------

## 👤 Autor

Edervaldo José de Souza Melo
Criador do Sistema Cognitivo Modular Nemosine Nous

INPI – Registro oficial: BR512025003335-4
GitHub: @edersouzamelo

------------------------------------------------------------

## 🤝 Contribuições

Sinta-se à vontade para abrir Issues ou Pull Requests.
Colaborações sérias, melhorias estruturais e análises técnicas são bem-vindas.

------------------------------------------------------------

## 📌 Status do Projeto

- Prova de Conceito funcional (FastAPI + React)
- AME hardened, executável, persistente e auditável
- Subordinação explícita do LLM ao Orchestrator
- Registro estrutural append-only
- Base arquitetural para evoluções futuras

------------------------------------------------------------

## 📬 Contato

Para parcerias, pesquisa, validação técnica ou uso institucional:
Email: edersouzamelo@gmail.com

------------------------------------------------------------

## 🛠️ Commit sugerido

git add README.md
git commit -m "Update AME baseline to v0.8.3-AME (persistent runtime)"
git push
