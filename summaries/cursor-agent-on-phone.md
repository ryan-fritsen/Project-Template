# Cursor Agent from your phone

A short reminder for starting, watching, and reviewing Cursor agents away from the desk. Follow-up questions and answers go in [Questions](#questions).

Checked against the Cursor docs on October 9, 2026.

## Which app to open

**iPhone or iPad.** Install [Cursor](https://apps.apple.com/app/cursor/id6767085653) from the App Store. It needs iOS 26 or iPadOS 26, and the interface is English. Sign in with your Cursor account (SSO if your organization requires it), pick a repository and branch, then send a task.

**Android, or any phone browser.** There is no Android app yet. Open [cursor.com/agents](https://cursor.com/agents) in Chrome and tap **Install App** so it sits on the home screen.

Agents you start on the phone also show up in the desktop Agents window and at [cursor.com/agents](https://cursor.com/agents). Agents you start on the desktop or the web show up in the phone inbox.

## Before the first run

- Use a paid plan that includes Cloud Agents: Start, Pro, Pro+, Ultra, Teams, or Enterprise. A free account can sign in and cannot start an agent.
- Connect source control on the web first (GitHub, GitLab, Bitbucket, or Azure DevOps). The phone cannot connect it. If the repo list is empty, connect it at [cursor.com](https://cursor.com), then pull down on the inbox to refresh.
- Use Privacy Mode, not Privacy Mode (Legacy). Cloud Agents need cloud data storage. Cursor does not train on your code.
- The first Cloud Agent run asks you to set a spend limit. Runs are billed at the selected model's API rate.

Cloud environments, secrets, and MCP servers are set up on the web. The phone uses whatever is already configured.

## What to do from the phone

1. Send a task. The agent keeps running after you lock the phone.
2. Watch the chat, or come back later. Pull down on the inbox if the thread looks behind.
3. Send a follow-up while it is still running.
4. Review the pull request: diffs, commits, checks, comments, and deployments.
5. From the pull request you can squash-merge, mark ready, update the branch, toggle auto-merge, publish, close, or change reviewers. You can also ask the agent to fix a failing check or address review comments.

On iPhone you also get a push notification when a turn finishes, Live Activities for up to eight agents (enable them in iOS Settings → Cursor), voice dictation, and Design Mode for photos, camera shots, and drawing on images.

## What the phone does not do

The app is for directing and reviewing agents. It is not an editor.

- There is no editor, terminal, or file browser. Changed files show up in the diff.
- Connecting GitHub or GitLab, secrets, environments, MCP setup, rules, skills, billing, and admin stay on [cursor.com/agents](https://cursor.com/agents) or the dashboard.
- Cloud agents take time to start. Each run sets up an environment before it writes code. That delay is the same on the web.

## Keep directing a computer session

Remote Control hands a desktop agent to your phone while tools still run on that computer. It needs Cursor 3.9.8 or later, the Agents Window, and a computer that stays awake and online.

1. On the computer, turn on Remote Control under Settings → Agents.
2. In the agent input, run `/remote-control`, then send the next message.
3. Open that session from the phone inbox and keep sending follow-ups.

On Teams and Enterprise, an admin enables this under Dashboard → Cloud Agents → Self-Hosted. Repository files and secrets stay on the computer. Tool calls stop if the computer sleeps or goes offline.

To move a local conversation into a cloud agent instead, use **Move to Cloud** on the desktop. Uncommitted files stay on the computer.

## Other ways to start one from a phone

These use the other app, not the Cursor app:

- **Slack or Microsoft Teams:** mention `@cursor` with a prompt. A later mention in the same thread is a follow-up.
- **GitHub:** comment `@cursor` on a pull request or issue.
- **Linear:** assign the issue to Cursor, or mention `@Cursor` in a comment.

## Questions

Answers to follow-up questions will be added here.

## Sources

- [Cursor for iOS](https://cursor.com/docs/cloud-agent/mobile)
- [Mobile app help](https://cursor.com/help/ai-features/mobile-app)
- [Cloud Agents](https://cursor.com/docs/cloud-agent)
