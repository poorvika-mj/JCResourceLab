# JC Resource Lab — Combined Full Stack

Everything runs from ONE file: `server.js`

## Files in this folder

```
server.js          ← Run this — serves both frontend & backend
frontend_b64.txt   ← Your React frontend (auto-loaded by server.js)
schema.sql         ← Paste in Supabase SQL Editor once
package.json       ← Dependencies
.env               ← Fill in your Supabase keys
```

---

## Setup (3 steps)

### Step 1 — Supabase
1. Go to **https://supabase.com** → New Project → Name it `jc-resource-lab` → Region: Singapore
2. Go to **SQL Editor** → paste the entire `schema.sql` file → click **Run**
3. Go to **Settings → API** → copy:
   - Project URL (looks like `https://xyz.supabase.co`)
   - service_role secret key (starts with `eyJ...`)

### Step 2 — Fill in .env
Open `.env` and replace the two placeholders:
```
SUPABASE_URL=https://your-actual-id.supabase.co
SUPABASE_SERVICE_ROLE_KEY=eyJ...your-actual-key...
```

### Step 3 — Run in VS Code
Open terminal in VS Code (`Ctrl + backtick`) and type:
```bash
npm install
node server.js
```

Then open your browser at **http://localhost:5000** ✅

---

## Admin Login
- Email: `admin@jcrl.com`
- Password: `admin123`

## For auto-restart on file changes (optional)
```bash
npm run dev
```
