# Workflow n8n Telegram + AI

## Description
Ce workflow n8n permet de recevoir des messages Telegram et de générer automatiquement des réponses intelligentes grâce à un agent IA (OpenAI).  
Il permet également d’envoyer les réponses via Gmail et Telegram, et de gérer un contexte simple pour suivre les conversations.

## Fonctionnalités
- Détection des messages texte et vocaux sur Telegram  
- Transcription des messages vocaux en texte via OpenAI  
- Génération automatique de réponses professionnelles et personnalisées avec un agent IA  
- Envoi automatique des réponses via Telegram et Gmail  
- Gestion simple du contexte conversationnel

## Technologies utilisées
- [n8n](https://n8n.io)  
- [Telegram API](https://core.telegram.org/bots/api)  
- [Gmail API](https://developers.google.com/gmail/api)  
- [LangChain](https://www.langchain.com/) / OpenAI  
- Python (intégration et scripts)

## Outils
- n8n workflows  
- AI workflow automation

## Structure du workflow
- **Telegram Trigger** : reçoit les messages Telegram (texte ou voix)  
- **If** : vérifie si le message est vocal ou texte  
- **Get a file** et **Transcribe a recording** : récupèrent et transcrivent les messages vocaux  
- **Prepare Voice Message Data** : prépare les données pour l’IA  
- **AI Agent** : génère la réponse via LangChain et OpenAI  
- **Prepare Response** : prépare la réponse finale pour Telegram et Gmail  
- **Send a text message** : envoie la réponse sur Telegram  
- **Send a message in Gmail** : envoie la réponse par email
