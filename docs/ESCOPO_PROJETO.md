# Escopo do Projeto de TCC

## 1. Identificação do Projeto
- **Nome do Projeto:** Assistente de Voz para Estudos com Foco em Privacidade  
- **Autor:** Ary Façanha        
- **Orientador:** Profª Clarissa Castellã Xavier  
- **Data:** --

---

## 2. Introdução e Visão Geral
Este projeto propõe o desenvolvimento de um assistente de voz offline para apoiar os estudos de estudantes de cursos técnicos e superiores.  
O sistema permitirá interação por voz, consulta de materiais acadêmicos em PDF e geração automática de flashcards para revisão.  

O diferencial do sistema está no foco em **segurança e privacidade**: todo processamento será realizado localmente, sem dependência de servidores externos, garantindo confidencialidade e proteção dos dados do usuário.

---

## 3. Objetivos do Projeto
- Desenvolver um assistente de estudos baseado em voz, que funcione offline.  
- Permitir importação de materiais acadêmicos em PDF e realizar busca local com auxílio de modelos de linguagem.  
- Gerar flashcards automáticos a partir das respostas obtidas.  
- Garantir privacidade por design, com todo processamento sendo local e dados protegidos por criptografia.  

---

## 4. Escopo do Projeto

### Entregáveis
- Aplicativo funcional (desktop ou web) com entrada por voz.  
- Módulo de importação e indexação de PDFs.  
- Geração de flashcards automáticos.  
- Documentação técnica e manual do usuário.  

### Requisitos
**Funcionais:**  
- Importar e indexar arquivos PDF.  
- Transcrever perguntas do usuário por voz.  
- Responder perguntas com base no conteúdo importado.  
- Gerar e exportar flashcards automáticos.  
- Reproduzir respostas também em áudio.  

**Não Funcionais:**  
- Todo processamento deve ser realizado localmente.  
- O sistema deve responder em até 5 segundos a perguntas curtas em hardware padrão.  
- Interface simples e intuitiva para estudantes.  

### Exclusões
- Integração com serviços externos de nuvem.  
- Suporte multilíngue além de português/inglês.  
- Funcionalidades avançadas de rede social ou compartilhamento.  

---

## 5. Recursos Necessários
- **Equipe:** 2 desenvolvedores, 1 pesquisador/testador, orientador acadêmico.  
- **Tecnologia:** Python (FastAPI, Whisper, Llama.cpp, Piper), React, SQLite/ChromaDB, Libsodium.  
- **Infraestrutura:** Computadores pessoais com capacidade de execução de modelos locais.  

---

## 6. Cronograma
- **Fase 1:** Pesquisa e planejamento (1 mês).  
- **Fase 2:** Desenvolvimento dos módulos principais (2 meses).  
- **Fase 3:** Integração e testes (1 mês).  
- **Fase 4:** Documentação final e apresentação (2 semanas).  

---

## 7. Premissas
- O sistema será utilizado por estudantes como ferramenta de apoio ao estudo.  
- Haverá disponibilidade de modelos de linguagem e reconhecimento de voz em versão compacta para execução local.  
- O grupo terá acesso a bibliografia acadêmica em PDF para testes.  

---

## 8. Restrições
- Prazo limitado ao semestre letivo.  
- Orçamento restrito a tecnologias e ferramentas open source.  
- Necessidade de funcionamento offline.  

---

## 9. Riscos e Planos de Contingência
- **Risco:** Baixo desempenho em hardware limitado.  
  - *Mitigação:* uso de modelos quantizados de menor tamanho.  
- **Risco:** Dificuldades de integração entre módulos STT, LLM e TTS.  
  - *Mitigação:* desenvolvimento modular e integração incremental.  
- **Risco:** Usuários finais terem dificuldade de uso inicial.  
  - *Mitigação:* interface simplificada e manual de utilização.  

---

## 10. Critérios de Aceitação
- O sistema deve importar PDFs, aceitar perguntas por voz e gerar respostas por texto e áudio.  
- O sistema deve criar flashcards automáticos exportáveis para Anki (CSV ou .apkg).  
- O processamento deve ocorrer localmente, sem envio de dados externos.  
