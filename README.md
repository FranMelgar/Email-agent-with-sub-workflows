AI Mail Agent con Pinecone — n8n Workflows

Este proyecto implementa un sistema inteligente de envío de emails automatizados utilizando arquitectura RAG, OpenAI y Pinecone. Está compuesto por tres workflows conectados que permiten almacenar contactos, generar emails personalizados y enviarlos automáticamente.

⚙️ Arquitectura del sistema

El proyecto se divide en 3 workflows principales:

1️⃣ Mails to Pinecone

Obtiene datos desde Google Docs.

Divide el contenido en chunks.

Genera embeddings con OpenAI.

Indexa la información en Pinecone para búsquedas semánticas.

👉 Función: crear la base de conocimiento con contactos y emails.

2️⃣ Mail Agent Pinecone

Recibe mensajes desde un chat.

Un AI Agent interpreta la solicitud.

Busca direcciones de correo en Pinecone.

Genera emails personalizados automáticamente.

Llama a un workflow externo para realizar el envío.

👉 Función: inteligencia y automatización del proceso.

3️⃣ Send Mails Pinecone

Recibe datos desde el agente.

Genera asunto y contenido del email con IA.

Envía correos mediante Gmail API.

👉 Función: ejecución final del envío de emails.

🧩 Tecnologías utilizadas

n8n

OpenAI (GPT-4o / GPT-4o-mini)

Pinecone Vector Database

Embeddings OpenAI

Gmail API

Arquitectura RAG

AI Agents (LangChain)

✅ Casos de uso

Envío automático de emails personalizados

Automatización de outreach o marketing

Sistemas inteligentes de contacto empresarial

Agentes AI para gestión de comunicaciones

🚀 Requisitos

n8n configurado

API Key de OpenAI

Cuenta Pinecone activa

Credenciales Google Docs y Gmail

Documentos con contactos previamente cargados
