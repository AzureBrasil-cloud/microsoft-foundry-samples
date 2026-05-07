# How to Create and Publish an AI Agent on Microsoft Teams | AzureBrasil

This guide explains step by step how to create, configure, and publish AI agents built in **Microsoft Foundry** directly to **Microsoft Teams** and **Microsoft 365 Copilot**.

The goal here is to provide a simple and practical path for you to publish agents created in Foundry efficiently, avoiding complications and ensuring the process is as straightforward as possible.

## What You'll Learn 📝

In this repository, we will guide you through the process of creating, configuring, and publishing your AI agents, covering everything from setting up your environment to post-publication governance. By following this process, you’ll be able to scale and use AI agents in Microsoft Teams efficiently.

### What’s Covered ⚙️

- **Preparing the Microsoft 365 and Azure environment**
- **How to configure the agent in Microsoft Foundry before publishing**
- **Selecting the active agent version**
- **Publishing to Microsoft Teams and Microsoft 365 Copilot**
- **Understanding admin approval and governance policies**
- **Validating the agent's behavior after publishing**

## Step 1: Access Microsoft Foundry 🔗

1. **Access the Microsoft Foundry portal**:
   - Go to the portal: [https://ai.azure.com](https://ai.azure.com)
   - If it's your first time, you'll need to create a project. Choose a name, select a region, and link an Azure subscription (or create a new one).

2. **Ensure the "New Foundry" toggle is enabled** before proceeding.

## Step 2: Create the Agent ⚙️

1. **Create the Agent**:
   - In **Microsoft Foundry**, click "Create Agent".
   - Choose a clear name that describes what the agent does (this name will be visible to users in Microsoft Teams).

2. **Configure the Agent**:
   - **Instructions**: Define the agent's behavior, tone, and objectives.
   - **Model**: Choose the language model to use (e.g., GPT-4o, GPT-4.1 Mini, etc.).
   - **Tools**: Define what the agent can access, such as web search, API calls, Fabric connections, and more.
   - **Knowledge**: Upload files and documents that the agent will use as its knowledge base.

3. **Test the Agent** 💡:
   - Use the live test panel on the right side of the screen to interact with the agent while configuring it. This will help you adjust the agent's behavior before publication.

## Step 3: Publish to Microsoft Teams ✅

1. **Save and Publish**:
   - After configuring and testing, click "Save" and then "Publish → Publish Agent".

2. **Choose Publishing Option**:
   - Select "Publish to Teams and Microsoft 365 Copilot".
   - Fill in the agent's details, including:
     - **Short description**: A line about what the agent does.
     - **Full description**: More context about its capabilities.
     - **Your name (creator)** and a related URL, if necessary.

3. **Choose Visibility**:
   - Decide whether the agent will be for **personal use**, **your organization**, or **public use** in Microsoft Teams.

4. **Configure Bot Service**:
   - If it's your first publication, click "Create a Bot Service" to create the Azure resource that manages the agent's deployment, authentication, and lifecycle.

5. **Admin Approval** ⚠️:
   - After publishing, admin approval will be required. Access the [Microsoft 365 Admin Center](https://admin.cloud.microsoft) to review and approve the request.

## Step 4: Admin Approval and Monitoring 🔎

1. **Admin Approval**:
   - In the admin center, define governance policies and who will have access to the agent:
     - Everyone in the organization
     - Specific groups
     - Individual users

2. **Monitor Performance 📊**:
   - After approval, use **Azure Bot Services** to monitor the agent's performance in the live environment, whether in Teams or 365 Copilot.

## Step 5: Using the Agent in Microsoft Teams ✅

1. **Access the Agent**:
   - Open **Microsoft Teams** and go to "Apps → Made for your organization". The agent will appear there, ready for installation.

2. **First Interaction**:
   - When opening the agent for the first time, Teams will request authentication to validate your identity. After authenticating, you can interact normally.

3. **Using in Group Chats and Channels** 💬:
   - You can also mention the agent in group chats and channels using `@AgentName`. This is especially useful for providing real-time support during team discussions.

## Updating the Agent 🔄

Any adjustments to the agent, whether it's behavior, files, or tools, can be made directly in Foundry without needing to repeat the entire publication process. If the version selector is set to "Always use latest" (default), the new version will automatically be served in Teams and Microsoft 365 Copilot.

## Best Practices 💡

- **Test thoroughly before publishing**: Test the agent’s behavior in the Foundry test panel before deploying it to your organization.
- **Secure your agents**: Implement proper authentication and follow RBAC principles to ensure only authorized users can access the agent.
- **Monitor performance**: Use **Azure Bot Services** to track the agent’s performance and ensure it’s functioning correctly.

## ⚠️ Cost Considerations

- **Be aware of tokens**: Using the agent generates token consumption in your Azure subscription. Keep track of the usage in the Azure portal to avoid unexpected charges at the end of the month.

## Official Resources 🔗

- **[Microsoft Foundry Overview](https://learn.microsoft.com/en-us/azure/foundry/)**: Introduction to Microsoft Foundry and how it can be used to create AI agents.
- **[Publish Agents to Microsoft Teams and Microsoft Copilot](https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/publish-copilot)**: Official guide on how to publish Foundry agents to Microsoft Teams.
- **[Create a Bot with Azure Bot Services](https://learn.microsoft.com/en-us/azure/bot-service/abs-quickstart?view=azure-bot-service-4.0)**: How to build bots that can be integrated with Microsoft Teams.

## Additional Documentation 📂

- **[Overview](docs/overview.md)** 📘: Publishing process, architecture, and environment setup.
- **[Examples](docs/examples.md)** 🧩: Practical publishing scenarios for different use cases.
- **[Troubleshooting](docs/troubleshooting.md)** 🛠️: Common issues and how to resolve them.
