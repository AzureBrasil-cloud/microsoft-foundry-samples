# Troubleshooting 🛠️

This page lists the most common issues teams face when publishing Microsoft Foundry agents to Microsoft Teams and Microsoft 365 Copilot.

The idea is simple: save time, reduce guesswork, and help you isolate whether the issue is in Foundry, Azure, Microsoft 365 governance, or the final user experience.

## Troubleshooting Mindset 🧠

When something breaks, avoid changing ten things at once.

Check the flow in this order:

1. **Agent configuration** ⚙️
2. **Active version** ✅
3. **Azure requirements** 🔐
4. **Publish flow** 📤
5. **Admin approval** 📝
6. **User access** 🔑
7. **Runtime behavior in Teams or Microsoft 365 Copilot** 🔍

That order usually gets you to the real cause faster.

## Issue 1: Publish option is available, but publish fails 🚫

### Possible Causes ⚠️

- `Microsoft.BotService` is not registered in the subscription
- Missing Azure permissions
- Bot resource creation failed
- Invalid metadata
- Tenant-side constraints

### What to Check 🔍

- Confirm the **Azure subscription** is the expected one
- Verify `Microsoft.BotService` is registered
- Check whether the **Bot Service resource** was created
- Review any validation errors in the **publish dialog**
- Confirm the account has enough **access** to the project and related Azure resources