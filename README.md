#  Fahemeni — فاهمني

> **AI-Powered All-in-One Arabic Learning Platform** — Built for Algerian students, designed to make learning click.

[![Next.js](https://img.shields.io/badge/Next.js-15-000000?style=flat-square&logo=nextdotjs&logoColor=white)](https://nextjs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5-3178C6?style=flat-square&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![Prisma](https://img.shields.io/badge/Prisma-ORM-2D3748?style=flat-square&logo=prisma&logoColor=white)](https://www.prisma.io/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind-CSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)](https://tailwindcss.com/)
[![License](https://img.shields.io/badge/License-MIT-0d9488?style=flat-square)](LICENSE)

---

## 📌 Overview

**Fahemeni** (Arabic: فهمني — *"Make Me Understand"*) is a next-generation AI learning platform tailored for Algerian students. It combines AI tutoring, interactive lessons, and a smart admin dashboard into one cohesive experience — available in **Arabic**, **French**, and **English**.

With **3,000+ users** and ~90 daily active learners, Fahemeni is already proving that localized AI education works.

---

## ✨ Features

### 🤖 AI-Powered Learning
- Conversational AI tutor with context-aware responses
- Personalized learning paths based on student progress
- Instant explanations in Arabic, French, or English

### 🌍 Full Internationalization (i18n)
- Native **RTL** support for Arabic
- Three-language UI: `ar` / `fr` / `en`
- Custom `useLang()` hook with flat JSON locale files

### 📊 Admin Dashboard
- Real-time analytics and student tracking
- Parallel Prisma queries for performance
- Content management across subjects and levels

### 🎨 Premium UI/UX
- RTL-first Arabic interface with Tajawal / Cairo fonts
- Teal accent design system (inspired by Notion, Linear, Stripe)
- Fully responsive — mobile, tablet, desktop
- PWA-ready with install prompt

### 🔐 Authentication & Access
- Secure access code system with sticky banner UI
- Subscription tiers with in-app popup flow
- Role-based access: Student / Admin

---

## 🗂️ Project Structure

```
fahemeni/
├── app/
│   ├── [locale]/            # i18n routing (ar, fr, en)
│   ├── admin/               # Admin dashboard pages
│   ├── api/                 # API routes
│   └── (auth)/              # Auth pages
├── components/
│   ├── ui/                  # Reusable UI components
│   ├── chat/                # AI chat interface
│   └── dashboard/           # Admin widgets
├── lib/
│   ├── prisma.ts            # Prisma client
│   └── useLang.ts           # i18n hook
├── locales/
│   ├── ar.json              # Arabic translations
│   ├── fr.json              # French translations
│   └── en.json              # English translations
├── prisma/
│   └── schema.prisma        # Database schema
└── public/                  # Static assets
```

---

## 🚀 Getting Started

### Prerequisites

- Node.js `>= 18`
- PostgreSQL (or any Prisma-supported DB)
- An Anthropic / OpenAI API key for AI features

### Installation

```bash
# Clone the repository
git clone https://github.com/your-username/fahemeni.git
cd fahemeni

# Install dependencies
npm install

# Set up environment variables
cp .env.example .env
```

### Environment Variables

```env
DATABASE_URL="postgresql://user:password@localhost:5432/fahemeni"
NEXTAUTH_SECRET="your-secret"
NEXTAUTH_URL="http://localhost:3000"
AI_API_KEY="your-api-key"
```

### Run Locally

```bash
# Push database schema
npx prisma db push

# Start development server
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| **Framework** | Next.js 15 (App Router) |
| **Language** | TypeScript |
| **Styling** | Tailwind CSS |
| **Database ORM** | Prisma |
| **Auth** | NextAuth.js |
| **AI** | Anthropic Claude / OpenAI |
| **Fonts** | Tajawal, Cairo (Arabic) |
| **Deployment** | Vercel |

---

## 🌐 Internationalization

Fahemeni supports three locales out of the box:

```json
// locales/ar.json (Arabic — RTL)
{
  "hero.title": "منصة التعلم الذكية",
  "hero.subtitle": "تعلم بالطريقة التي تفهمها"
}

// locales/fr.json (French)
{
  "hero.title": "Plateforme d'apprentissage IA",
  "hero.subtitle": "Apprenez à votre façon"
}
```

Switch language using the `useLang()` hook:

```ts
const { t, locale } = useLang()

return <h1>{t('hero.title')}</h1>
```

---

## 📈 Stats

| Metric | Value |
|---|---|
| 👥 Total Users | 3,000+ |
| 📅 Daily Active Users | ~90 |
| 🌍 Languages Supported | 3 (AR, FR, EN) |
| 📚 Subjects Covered | Multiple (BAC-aligned) |

---

## 🗺️ Roadmap

- [x] AI chat tutor
- [x] Admin dashboard
- [x] Full i18n (AR / FR / EN)
- [x] RTL Arabic UI
- [x] PWA support
- [x] Subscription system
- [ ] Mobile app (React Native)
- [ ] Offline mode
- [ ] Parent tracking portal
- [ ] Gamification & badges
- [ ] Video lessons integration

---

## 🤝 Contributing

Contributions are welcome! Please open an issue first to discuss what you'd like to change.

```bash
# Create a feature branch
git checkout -b feature/your-feature-name

# Commit your changes
git commit -m "feat: add your feature"

# Push and open a PR
git push origin feature/your-feature-name
```

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

## 👤 Author

**Ouzal Med Achraf** — Solo Founder & Builder

[![GitHub](https://img.shields.io/badge/GitHub-@OuzalMedAchraf-181717?style=flat-square&logo=github)](https://github.com/ouzali30)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-OuzalMedAchraf-0A66C2?style=flat-square&logo=linkedin)](https://linkedin.com)
[![Email](https://img.shields.io/badge/Email-ouzala30@gmail.com-0d9488?style=flat-square&logo=gmail)](mailto:ouzala30@gmail.com)

---

<div align="center">

Built with ❤️ in **Algeria 🇩🇿** — making education accessible for every student.

**[🌐 Visit Fahemeni](https://fahemeni.com)**

</div>
