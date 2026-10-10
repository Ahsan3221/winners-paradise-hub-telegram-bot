# Winners Paradise Hub — Telegram Customer CRM

This bot preserves existing `winners_paradise_hub_users`, `winners_paradise_hub_topics`, and `winners_paradise_hub_staff` PostgreSQL tables and existing forum topic IDs. Additional CRM tables are created additively.

**Features:** customer labels (case-insensitive, any custom value), game account lookup, saved plaintext game passwords, account auto-capture from staff chat templates, pinned customer profiles, notes, assignment, audit history, durable message queue, owner-only staff management, opt-in broadcasts, privacy/deletion commands and **CashMaster** game selection.

**Automatic account capture:** send in a customer's staff forum topic:
```text
👤 Username: Sarah333fk
🔑 Password: 009988
Log in and let me know if you need help ❤️✨
```
The bot detects Firekirin and stores credentials while forwarding the message. Suffixes: 3s Orionstars, 3fk Firekirin, 3v Vblink, 3u UltraPanda, 3r Riversweeps, 3j Juwa, 3gv GameVault, 3mw Milkyway, 3cm CashMaster (repeated 3 digits supported). `Game: Other Name` handles custom names.

**Staff commands:** `/profile`, `/accounts`, `/setaccount Game Username`, `/label My Custom Label`, `/unlabel VIP`, `/findaccount Username`, `/note Text`, `/history`, `/assign ID`, `/status pending`, `/close`, `/groupid`.

**Railway:** preserve `BOT_TOKEN`, `SUPPORT_GROUP_ID`, `DATABASE_URL`, `AUTHORIZED_STAFF_IDS`. Add `OWNER_IDS` containing owner numeric Telegram ID for owner commands. No encryption key. Take a PostgreSQL snapshot before deploying. If auto-deploy is connected to GitHub main it may deploy automatically. GitHub source backup: `backup/pre-crm-unification-20261011`.

**Tests:** `python -m pytest -q`; live Telegram and PostgreSQL integration tests not executed.
