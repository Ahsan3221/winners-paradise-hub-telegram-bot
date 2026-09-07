# Winners Paradise Hub — Telegram / BotFather Details

## Identity

- **Bot name:** Winners Paradise Hub
- **Bot username:** `@Winnersparadisehubbot`
- **Topics support group ID for Railway:** `-1005493103200`

## Edit About

Paste this into BotFather → **Edit About**:

```text
🏆 Choose your game and connect with the Winners Paradise Hub support team.
```

## Edit Description

Paste this into BotFather → **Edit Description**:

```text
Welcome to Winners Paradise Hub! 🏆

Choose your game, select an available bonus option, and connect with our support team for quick assistance.

Send /start to begin your support chat.
```

## Edit Commands

Paste only these four lines into BotFather → **Edit Commands**:

```text
start - Start or restart your support chat
help - Show help and available commands
games - Choose or change your game
support - Reach the support team
```

## Edit Privacy Policy

Create a public GitHub repository with this suggested name:

```text
winners-paradise-hub-telegram-bot
```

Upload the completed `PRIVACY_POLICY.md` file, then place its public HTTPS URL in BotFather → **Edit Privacy Policy**.

Example URL format:

```text
https://github.com/YOUR_GITHUB_USERNAME/winners-paradise-hub-telegram-bot/blob/main/PRIVACY_POLICY.md
```

If BotFather does not accept the normal GitHub page URL, use the Raw format:

```text
https://raw.githubusercontent.com/YOUR_GITHUB_USERNAME/winners-paradise-hub-telegram-bot/main/PRIVACY_POLICY.md
```

## Required group settings

1. Add `@Winnersparadisehubbot` as an administrator to the correct private Topics-enabled support group.
2. Give the bot **Manage Topics** and **Send Messages** permissions.
3. BotFather → Bot Settings → Group Privacy → **Turn Off**.
4. After changing Group Privacy, remove the bot from the group and add it again.
5. In Railway, set the support group exactly as:

```env
SUPPORT_GROUP_ID=-1005493103200
```

6. Set the first staff/owner ID as:

```env
AUTHORIZED_STAFF_IDS=5991692961
```

## Test

- Send `/start` to @Winnersparadisehubbot in a private chat.
- Select a bonus and game.
- Send a text message.
- A customer topic should appear in the support group.
- Reply from the authorized staff account inside that topic; the customer should receive it.
