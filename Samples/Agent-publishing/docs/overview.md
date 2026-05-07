# Overview 📘

This guide explains how to publish AI agents built in Microsoft Foundry to Microsoft Teams and Microsoft 365 Copilot.

The goal is to give you a practical path from agent creation to controlled distribution inside your organization, without turning the documentation into a giant wall of text.

This repository is focused on the Foundry publishing flow through the portal experience. It is meant for architects, developers, IT admins, and technical teams that want to operationalize internal AI agents in Microsoft 365 surfaces.

## What this covers ✅

This guide focuses on:

- preparing the Azure and Microsoft 365 environment ⚙️
- configuring the agent correctly before publishing 🤖
- selecting the active version 🔄
- publishing to Teams and Microsoft 365 Copilot 🚀
- understanding approval and governance 🔐
- validating the agent after release ✅

## What this does not cover 🚫

This guide does not go deep into:

- full SDK-based agent development
- advanced Teams app engineering
- Copilot Studio-only scenarios
- custom proxy apps built outside the standard Foundry publish flow

## Why publish from Foundry 💡

Publishing from Microsoft Foundry allows you to take an agent that already works in the Foundry environment and expose it in places where users already spend their day, especially Microsoft Teams and Microsoft 365 Copilot.

That reduces friction. Instead of asking users to access another portal, the agent becomes available inside the tools they already know.

## High-level architecture 🏗️

```text
Microsoft Foundry
   │
   ├─ Agent instructions
   ├─ Knowledge
   ├─ Tools / actions
   ├─ Model configuration
   │
   ▼
Publish flow in Foundry
   │
   ├─ Active version selected
   ├─ Azure Bot Service created or reused
   ├─ Metadata completed
   │
   ▼
Microsoft 365 app package
   │
   ├─ Microsoft Teams
   └─ Microsoft 365 Copilot
         │
         ▼
Microsoft 365 admin approval and access policies
         │
         ▼
End-user access