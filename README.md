# Assistente de Voz para Estudos (Offline & Privado)

## Visão Geral
Este projeto tem como objetivo desenvolver um **assistente de voz para estudos**, com foco em **privacidade e segurança**.  
O sistema permite que estudantes façam perguntas por voz, obtenham respostas baseadas em seus materiais (ex.: PDFs de livros) e gerem automaticamente **flashcards** para revisão.

Todo o processamento ocorre **localmente**, sem envio de dados para servidores externos.  
Isso garante **privacidade por design** e torna a aplicação ideal para quem valoriza a segurança de seus dados acadêmicos.

---

## Funcionalidades Principais
- **Entrada por voz:** transcreve perguntas do usuário.  
- **Importação de PDFs:** indexa conteúdos para consulta offline.  
- **Respostas inteligentes:** utiliza modelo de linguagem pré-treinado (LLM) para responder perguntas com base no material do usuário.  
- **Resposta falada:** converte as respostas em áudio com TTS.  
- **Flashcards automáticos:** gera cartões de estudo prontos para exportação (CSV/Anki).  

---

## Privacidade e Segurança
- Todo processamento ocorre **no dispositivo local** (STT, LLM, TTS, RAG).  
- **Zero telemetria**: nenhum dado é enviado para terceiros.  
- **Criptografia em repouso** (XChaCha20-Poly1305) para materiais e índices.  
- **Senha derivada com Argon2id** para proteger chaves de criptografia.  
- **Consentimento explícito** para uso do microfone.  

---

## Tecnologias Utilizadas
- **Backend:** Python (FastAPI, WebSocket)  
- **STT (fala → texto):** Whisper.cpp ou Faster-Whisper  
- **LLM (respostas):** Llama.cpp (Llama 3) ou DeepSeek (quantizado)  
- **RAG (busca local):** Sentence-Transformers + ChromaDB/SQLite  
- **TTS (texto → voz):** Piper (pt-BR)  
- **Segurança:** Libsodium (XChaCha20-Poly1305, Argon2id)  
- **Frontend:** React (web) / React Native (mobile)  