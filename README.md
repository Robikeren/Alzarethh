# StudyMate AI

AI Tutor pelajaran berbasis Claude API.

## Struktur File

```
studymate/
├── api/
│   └── chat.js        ← Backend (serverless function)
├── public/
│   └── index.html     ← Frontend
├── vercel.json        ← Konfigurasi Vercel
└── package.json
```

## Cara Deploy ke Vercel

### 1. Daftar/Login Vercel
- Buka https://vercel.com
- Login dengan GitHub

### 2. Upload ke GitHub
- Buat repo baru di https://github.com/new
- Upload semua file ini ke repo tersebut

### 3. Deploy di Vercel
- Di dashboard Vercel, klik "Add New Project"
- Pilih repo GitHub yang tadi dibuat
- Klik "Deploy"

### 4. Tambahkan API Key
- Setelah deploy, buka Settings → Environment Variables
- Tambahkan:
  - Name:  ANTHROPIC_API_KEY
  - Value: sk-ant-xxxxxxx (API key kamu)
- Klik Save, lalu Redeploy

### 5. Selesai!
Website kamu sudah live dan bisa diakses siapa saja.

## Cara dapat API Key Anthropic
- Buka https://console.anthropic.com
- Daftar/login
- Klik "API Keys" → "Create Key"
- Copy key-nya (dimulai dengan sk-ant-)
