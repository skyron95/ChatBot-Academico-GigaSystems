# ChatBot Académico – GigaSystems

## 1. Introducción
Este proyecto consiste en el desarrollo de un chatbot académico capaz de responder preguntas frecuentes relacionadas con trámites estudiantiles. El flujo se implementa en n8n y se conecta con una página web externa mediante un Webhook. El chatbot ofrece respuestas simples y automáticas a consultas como certificados, calificaciones, requisitos y tiempos de solicitud.

## 2. Alcance
Este documento describe únicamente el flujo del chatbot desarrollado en n8n. 
Incluye:
- Recepción de mensajes desde la página web mediante un Webhook.
- Procesamiento básico de la pregunta.
- Respuestas simples según las consultas académicas más comunes.
No abarca la construcción de la página web ni la gestión de bases de datos.

## 3. Arquitectura General
El sistema se compone de tres partes principales:

1. **Página Web del Chatbot**  
   Interfaz donde el usuario escribe su consulta. Esta página enviará la información hacia un Webhook.

2. **n8n (Chatbot Backend)**  
   Contiene el flujo que recibe la pregunta, la interpreta y genera una respuesta automática.  
   El flujo inicia con un nodo Webhook que actúa como punto de entrada.

3. **Respuesta al Usuario**  
   n8n envía una respuesta en formato JSON que la página web mostrará al usuario.
