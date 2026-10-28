<!-- Claude: this file is the setup guide for people. Follow CLAUDE.md, not this file. When starting a new app, the start-app skill replaces this file with a README for the app. -->

# Build Android apps from your phone with Claude

Describe the app you want in the Claude app. Claude writes it, GitHub builds it, and a few minutes later you install it on your phone from a link. Ask for changes the same way; each new version installs over the old one and keeps your data.

Your code lives in your own GitHub repository, and it uses your own Claude subscription. No other service holds your login.

## What you need

- An Android phone.
- A **Claude Pro or Max** plan. Claude Code in the cloud isn't on the Free plan. (With an API key, see [Using a computer or an API key](https://github.com/wurp/vibe-dev-template/wiki/Using-a-computer-or-an-API-key).)
- A free **GitHub** account.

## Set up (once, about 15 minutes)

Steps 1–3 happen in a web browser, on your phone or a computer.

1. **Create a GitHub account** at [github.com/signup](https://github.com/signup), if you don't have one.
2. **Copy this template.** At the top of this page, tap **Use this template → Create a new repository**. Give it a short name (for example `plant-diary`), then choose:
   - **Private** (recommended): only you can see the code. To download your app, stay signed in to GitHub in Chrome on your phone.
   - **Public**: anyone can see the code, and you can send the download link to friends. You can switch later in the repository's settings.

   Then tap **Create repository**.
3. **Let Claude use it.**
   - If you've never used Claude Code on the web: go to [claude.ai/code](https://claude.ai/code), sign in, and connect GitHub when asked.
   - Then give Claude access to the new repository: go to [github.com/apps/claude/installations/new](https://github.com/apps/claude/installations/new) (or, if Claude is already installed, [github.com/settings/installations](https://github.com/settings/installations) → **Configure** next to Claude), choose **Only select repositories**, and add your new one.
   - GitHub may ask you to approve permissions. That's expected.
4. **Start your app.** In the Claude app, open **Code**, tap **New session**, tap the repository name shown above the message box, and pick your new repository. Then say what you want, for example "a diary for my houseplants that reminds me to water them."
5. **Install it.** When Claude says it's ready, it gives you a link.
   - Long-press the link, choose **Copy link**, and paste it into **Chrome**. (Downloads can stall inside the Claude app.) For a private repository, Chrome must be signed in to GitHub.
   - If Chrome warns about the file, tap **Download anyway**, then tap the download.
   - The first time, Android asks you to allow installs from Chrome, and Google Play Protect asks you to confirm an app from an unknown developer. Both are normal for apps not from the Play Store.
   - Play Protect scans each new version before it installs. Just wait for it.

After that, tell Claude what to change. The link stays the same, and the new version installs over the old one.

## If something goes wrong

- **The app crashed:** open it again. It shows a **Copy for Claude** button. Tap it and paste the result to Claude.
- **Anything else:** see [Troubleshooting](https://github.com/wurp/vibe-dev-template/wiki/Troubleshooting).

## More

- [Setup in detail](https://github.com/wurp/vibe-dev-template/wiki/Setup-in-detail), with what each screen looks like.
- [Faster checks with one network setting](https://github.com/wurp/vibe-dev-template/wiki/Setup-in-detail#optional-faster-checks).
- [How it works](https://github.com/wurp/vibe-dev-template/wiki/How-it-works), for developers.
- [Costs and limits](https://github.com/wurp/vibe-dev-template/wiki/Costs-and-limits).
- Questions and ideas: [Discussions](https://github.com/wurp/vibe-dev-template/discussions).

MIT licensed. Not affiliated with Anthropic.
