---
name: share-app
description: Help the author share the app with other people, either by sending the download link to friends or by publishing on Google Play. Use when the author wants others to have the app.
---

# Share the app

Explain the two options in plain words and ask which they want. Don't start the bigger one without saying what it involves.

## Option 1: send friends the link (easiest)

The same download link works for anyone, because this repository is public.

- Friends install it the way the author did: open the link in Chrome, allow installs from Chrome the first time, and confirm Google Play Protect's prompt.
- For a new version, they open the link again and install over the old one. Their data stays.
- Mention plainly:
  - Anyone with the link can install the app.
  - The app's code is public.
  - Each phone keeps its own data. Nothing is shared between phones unless you build that.
- Google is tightening the rules for apps installed from outside the Play Store from 2027. Sharing by link may need extra steps after that.

## Option 2: publish on Google Play (a bigger job)

Tell the author up front what it takes, then ask whether to go ahead:

- **Their own Google Play developer account.** It costs $25 once and needs ID verification. It's set up at play.google.com/console, easiest on a computer.
- **A closed test first.** New personal accounts must have at least 12 testers opted in for 14 days before the app can be public.
- **A privacy policy and a data-safety form,** even if the app collects nothing.
- **A private release signing key.** It must never go in this public repository. The debug key in `keystore/` can't be used for Play.

What you can do for them:

1. **Write the listing.** Draft it from what you know about the app, show it in plain text, and ask for changes. Save it as:
   - `fastlane/metadata/android/en-US/title.txt`: the name (max 30 characters for Play).
   - `fastlane/metadata/android/en-US/short_description.txt`: one sentence (max 80 characters).
   - `fastlane/metadata/android/en-US/full_description.txt`: what it does, who it's for, and what it doesn't do. Be honest.
2. **Draft a short privacy policy** in plain language, based on what the app actually does. Check `app/src/main/AndroidManifest.xml` for permissions and internet use, not your memory.
3. **Walk them through the Play Console steps** one at a time, in plain words, when they're ready.

Before saying it's ready, confirm nothing secret is in the repository (see "Secrets" in `CLAUDE.md`), and ask the author to confirm the app works on their phone. Then push, so the listing is saved.
