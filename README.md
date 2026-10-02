# 🤖 Sistema de Agente de Triagem & RAG com Google Gemini

Este projeto implementa uma solução completa de atendimento inteligente e **Service Desk** utilizando **Agentes de IA** e **RAG (Retrieval-Augmented Generation)** com a API do **Google Gemini** e o **LangChain**.

## 🎯 Funcionalidades Principais

- **Triagem Inteligente de Chamados:** Classifica as mensagens recebidas em `AUTO_RESOLVER`, `PEDIR_INFO` ou `ABRIR_CHAMADO`, atribuindo nível de urgência e retornando dados estruturados via `Pydantic`.
- **Busca Semântica (RAG):** Processa e indexa documentos em PDF (Políticas Internas da Empresa) utilizando o banco vetorial **FAISS**.
- **Respostas Fundamentadas:** O modelo responde estritamente com base nos documentos carregados, citando o documento e a página de origem das informações.
- **Proteção contra Alucinações:** Caso a informação não esteja nos documentos fornecidos, o sistema responde "Não sei".

## 🛠️ Tecnologias Utilizadas

- **Linguagem:** Python
- **Modelos de IA:** Google Gemini (`gemini-2.5-flash`, `models/gemini-embedding-001`)
- **Orquestração de LLMs:** LangChain
- **Banco Vetorial:** FAISS
- **Processamento de PDFs:** PyMuPDF

## 🚀 Como Executar o Projeto

1. Clone o repositório:
   ```bash
   git clone [https://github.com/SEU-USUARIO/agente-rag-gemini.git](https://github.com/SEU-USUARIO/agente-rag-gemini.git)
   cd agente-rag-gemini
