# 🤖 Agente IA WhatsApp Pro

**Automação Comercial Humanizada & Inteligente (24/7)**

![Status](https://img.shields.io/badge/Status-Production-green)
![AI Engine](https://img.shields.io/badge/AI-LLM_Integrated-blueviolet)

O **Agente IA WhatsApp Pro** é uma solução enterprise para atendimento automatizado que transcende chatbots tradicionais. Utilizando Modelos de Linguagem (LLMs) de última geração, o sistema entende contexto, interpreta mídias (áudio, imagem e documentos) e realiza agendamentos complexos de forma natural.

## 🧠 Capacidades Cognitivas

*   **Processamento Multimodal:** Analisa fotos enviadas por clientes (ex: comprovantes, produtos) e transcreve áudios em tempo real.
*   **Contexto Persistente:** Lembra preferências do cliente e histórico de conversas anteriores.
*   **Agendamento Inteligente:** Conecta-se à agenda da empresa para verificar disponibilidade e marcar reuniões sem conflitos.
*   **Humanização Adaptativa:** Ajusta o tom de voz (formal, amigável, técnico) conforme a marca da empresa.

## 🏗️ Arquitetura da Solução

O sistema opera em uma arquitetura de microsserviços orientada a eventos:

1.  **Ingestion Layer:** Webhooks do WhatsApp Business API recebem mensagens.
2.  **Reasoning Engine:** O core da IA processa a intenção do usuário e decide a ação (Responder, Agendar, Escalonar).
3.  **Action Layer:** Executa funções externas (consultar banco de dados, enviar e-mail via Formspree, atualizar CRM).

## 🚀 Configuração Rápida (Formspree)

Para ativar o módulo de contato / lead generation no site estático:

1.  Crie um form em [formspree.io](https://formspree.io).
2.  No arquivo `index.html`, atualize a constante:
    ```javascript
    const FORMPSREE_ENDPOINT = 'https://formspree.io/f/seu_id_aqui';
    ```

## 🔒 Privacidade e Conformidade

Este projeto segue rigorosamente a LGPD.
*   **Política de Privacidade:** Disponível em `/politica-privacidade/index.html`.
*   **Dados:** Todo processamento de IA é efetuado com mascaramento de dados sensíveis (PII).

---
*Desenvolvido por [MatheusOBS](https://github.com/MatheusOBS) - Transformando conversas em conversão.*
