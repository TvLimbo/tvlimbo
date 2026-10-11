# 📺 TVLIMBO

![TVLIMBO](https://img.shields.io/badge/TVLIMBO-EST.2010-E30613?style=for-the-badge)
![Next.js](https://img.shields.io/badge/Next.js-14-black?style=flat-square&logo=next.js)
![Three.js](https://img.shields.io/badge/Three.js-Premium-white?style=flat-square&logo=three.js)
![Limburg](https://img.shields.io/badge/Made%20in-Limburg-FF4A57?style=flat-square)

**Limburgs Talent. Wereldse Sterren.**
> Het online internet televisie platform waar talent geen like nodig heeft, maar een podium.

---

### 📖 Het Verhaal

**TVLimbo** werd opgericht in **2010 aan de Maaskade in Venlo** door **Bjorn Louer**.

De officiële opening werd verricht door artiest **Lange Frans** - het startschot voor een nieuw tijdperk voor Limburgs talent.

Wat begon als een lokale zender aan de Maas, groeide uit tot het platform waar zangers, dansers, muzikanten, comedians en presentatoren uit Limburg zich kunnen ontwikkelen tot ware sterren.

In 2026 bouwen we verder: van Maaskade naar mainstage.

---

### 🚀 TVLIMBO 2.0 - Tech Stack

We bouwen geen YouTube kloon. We bouwen een **premium online TV-zender**.

| Layer | Tech |
| :--- | :--- |
| **Framework** | Next.js 14 (App Router) + TypeScript |
| **Styling** | Tailwind CSS + shadcn/ui |
| **3D / Motion** | Three.js (@react-three/fiber) + Framer Motion |
| **Auth** | NextAuth.js - Google Login + Handmatig Login |
| **Database** | Prisma + PostgreSQL |
| **Upload** | UploadThing / Cloudinary |
| **Video** | Video.js + HLS voor Live TV |
| **Design** | Vrolijk, Fris, Premium - Wit `#FFFFFF` + Limburgs Rood `#E30613` |

---

### ✨ Features

#### 🔴 Live TV Experience
- Echte TV player met LIVE badge, pulserende dot
- Programma gids: "Nu op TV" & "Straks"
- Kanalen: Talent van de Week, Maaskade Sessions, etc.

#### 👤 Talent Systeem
- Eigen profiel pagina `/talent/[id]`
- Artiestennaam, bio, categorie (Zang, Dans, Muziek, Comedy)
- Boek-knop voor optredens
- Social links

#### 📹 Upload Systeem
- **Video (16:9)** - Max 2GB, thumbnail, titel, beschrijving, categorie
- **Reels (9:16)** - Max 60 sec, hashtags, TikTok-style feed
- Drag & drop upload met rode progress bar
- Status: In Review -> Live

#### 🔐 Auth
- Google Login (One-click)
- Handmatig: Email / Wachtwoord + Wachtwoord vergeten
- Role based: Viewer / Talent / Admin

#### 🎨 Premium UI
- Glassmorphism header
- Three.js vloeiende blobs in hero
- 24-32px border-radius overal
- Skeleton loaders & micro-interacties

---

### 📦 Installatie

```bash
# Clone
git clone https://github.com/jouwnaam/tvlimbo.git
cd tvlimbo

# Install
npm install

# Env vars aanmaken
cp.env.example.env
# Vul in: DATABASE_URL, NEXTAUTH_SECRET, GOOGLE_CLIENT_ID, GOOGLE_CLIENT_SECRET, UPLOADTHING_TOKEN

# Database
npx prisma db push
npx prisma studio

# Run
npm run dev
