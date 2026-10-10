# Winners Paradise Hub Railway Deployment
Original GitHub backup: `backup/pre-crm-unification-20261011`.

1. Railway ka PostgreSQL database backup/snapshot banao; GitHub backup DB backup nahi hai.
2. Variables unchanged rakho: BOT_TOKEN, SUPPORT_GROUP_ID, DATABASE_URL, AUTHORIZED_STAFF_IDS.
3. NEW: OWNER_IDS=YOUR_NUMERIC_TELEGRAM_ID.
4. GitHub main update Railway auto-deploy (agar enabled hai) trigger karega.
5. Logs check karo; customer DM, staff reply, old topic, /profile, /accounts, /label VIP aur automatic account capture test karo.
6. Passwords intentionally plaintext database mein store honge. Database access limited rakho.
Rollback via backup source branch possible hai, lekin PostgreSQL schema automatically downgrade nahi hota.
