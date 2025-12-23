**Agente de Voz Telegram (n8n)**

Este projeto é um workflow do n8n que conecta um bot do Telegram a um agente de IA, permitindo interação por mensagens de texto e mensagens de voz. 

O bot entende o que o usuário escreve ou fala e responde em texto ou áudio, de forma automática.

**O que o workflow faz**

•Recebe mensagens de um bot do Telegram

•Identifica se a mensagem é:

-Texto

-Voz (quando o usuário responde a um áudio)

•Se for voz:

-Baixa o áudio

-Transcreve para texto (PT-BR)

•Envia o texto para um AI Agent

•Retorna a resposta:

-Em texto, ou

-Em áudio (voz gerada por IA)

**Pré-requisitos**

•n8n (cloud ou self-hosted)

•Bot do Telegram configurado

•Credenciais no n8n:
-Telegram
-OpenAI

**Como usar**

1-Importe o arquivo .json no n8n

2-Configure as credenciais de Telegram e OpenAI

3-Ative o workflow

4-Envie mensagens para o bot no Telegram

**Tipos de interação**

•Texto

-Envie uma mensagem normal para o bot

-Ele responderá em texto

•Voz

-Responda (reply) a uma mensagem de voz

-O bot irá:

Transcrever o áudio

Processar com IA

Responder em texto ou áudio

**Observações importantes**

•O workflow vem desativado ao importar → é necessário ativá-lo

•O fluxo de voz depende de responder a uma mensagem de áudio

•A voz gerada usa TTS (texto para fala)

**Personalização**

•Você pode facilmente alterar:

-A mensagem inicial de resposta

-O prompt do agente de IA

-O modelo de IA utilizado

-O idioma da transcrição

-O tipo de resposta (somente texto ou áudio)
