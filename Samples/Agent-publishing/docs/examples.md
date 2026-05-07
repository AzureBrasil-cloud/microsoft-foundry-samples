# Examples

This page shows practical publishing scenarios for Microsoft Foundry agents in Microsoft Teams and Microsoft 365 Copilot.

The goal: Help you choose the right publishing path, avoid common mistakes, and validate the result with less guesswork.

## Example 1: Publish for personal testing 🧑‍💻

Use this path to validate the experience before involving others.

### Good fit:
- Validating agent behavior
- Checking metadata
- Testing authentication

### Flow:
1. Open your agent in Foundry.
2. Test it in the panel.
3. Select the active version.
4. Click **Publish** → **Publish to Teams and Microsoft 365 Copilot**.
5. Review or create the Azure Bot Service.
6. Choose **Just you** and publish.

### Expected result ✅
- Available for you immediately.
- Shows in your personal agent area.

* * *

## Example 2: Publish for the organization 🏢

For agents ready for broader internal use.

### Good fit:
- Company-wide assistants
- Internal support agents
- Production-ready deployments

### Flow:
1. Prepare and validate the agent.
2. Select the active version.
3. Fill in metadata.
4. Choose **People in your organization**.
5. Submit for admin approval.

### Expected result ✅
- Approved by admin.
- Appears in the organizational catalog.

* * *

## Example 3: Download and customize 💾

For more control over the package.

### Good fit:
- Advanced packaging review
- Manual upload in Teams

### Flow:
1. Open the publish experience.
2. Choose **Download & customize**.
3. Download and apply customizations.
4. Upload manually in Teams.

### Expected result ✅
- A distributable package.

* * *

## Example 4: Internal pilot 🏢

For testing with a small team before full rollout.

### Suggested approach:
1. Start with **Just you**.
2. Validate behavior.
3. Move to **People in your organization**.
4. Admin approval and restricted access.

* * *

## Example 5: Releasing a new version 🔄

For updates like bug fixes and new tools.

### Flow:
1. Update the agent.
2. Test again.
3. Re-run the publish flow.
4. Validate the new behavior.

* * *

## Pre-publish checklist 📝

- Agent works in Foundry test panel
- Right version is active
- **Microsoft.BotService** is registered
- Metadata is final and user-friendly
- No secrets in visible fields

* * *

## Post-publish checklist ✅

- Publish action completed successfully
- Admin approval is visible
- Agent appears in the right location

* * *

## Common mistakes 🚫

- Publishing before testing
- Forgetting the active version
- Missing Azure provider registration
- Treating metadata as internal notes
- Assuming organization publish is immediate

* * *

## Suggested rollout model 📈

1. Personal publish
2. Technical validation
3. Small-group pilot
4. Organization publish
5. Governance review