# Product brief

## Description

GreenTick is a WhatsApp Business platform. Teams connect a WhatsApp Business account, then manage contacts, templates, broadcasts, live chat, automations, and a Developer API from the dashboard at dashboard.greentick.ai.

## Primary audience

Two readers, with equal weight:

- People running WhatsApp for a business: marketers and support teams using the dashboard.
- Developers and operators connecting other software through the Developer API, webhooks, and Google Sheets.

Assumption: English is the only docs language for this site. Super-admin screens (all accounts, change owner) stay out of the docs.

## Jobs to be done

1. Create an account, connect WhatsApp, and reach the first successful send or reply.
2. Run the core dashboard loop: contacts, approved templates, broadcasts, and live chat.
3. Authenticate to `https://api.greentick.ai/v1`, send a template, and receive signed webhooks.

## Motivation

WhatsApp is the channel. GreenTick is the place to connect the business number, get templates approved, message customers, and let other tools do the same through an API key.
