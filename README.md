<div align="center">

<img src="docs/screenshots/icon.png" alt="HatamiDev" width="96" height="96" />

# HatamiDev Portfolio & License Platform

**پرتفولیو حرفه‌ای + پلتفرم فروش و مدیریت لایسنس**

[![Live Demo](https://img.shields.io/badge/Live-hatamidev.com-6366f1?style=for-the-badge&logo=vercel&logoColor=white)](https://hatamidev.com)
[![Author](https://img.shields.io/badge/Mehran_Hatami-Developer-0ea5e9?style=for-the-badge)](https://github.com/HatamiDev)
[![License](https://img.shields.io/badge/License-Proprietary-red?style=for-the-badge)](#license)

[English](#english) · [فارسی](#فارسی)

</div>

---

## فارسی

> **توجه:** این ریپازیتوری یک **نمایشگاه عمومی (Showcase)** است. سورس کامل پروژه به‌صورت تجاری فروخته می‌شود و در اینجا منتشر **نشده** است.

### درباره پروژه

سایت [hatamidev.com](https://hatamidev.com) دو نقش هم‌زمان دارد:

1. **پرتفولیو شخصی** — معرفی مهارت‌ها، پروژه‌ها و تجربه‌های Mehran Hatami
2. **پلتفرم فروش لایسنس** — فروش، فعال‌سازی و مدیریت محصول Vendrix (پنل فروشگاهی)

### ویژگی‌های کلیدی

| ماژول | توضیح |
|---|---|
| 🌐 **چندزبانه** | فارسی، انگلیسی و آلمانی با `next-intl` |
| 🎬 **رابط سینمایی** | انیمیشن‌های Framer Motion و Anime.js |
| 🔐 **پورتال مشتری** | مدیریت لایسنس، دانلود محصول، پشتیبانی |
| 💳 **سیستم پرداخت** | PayPal، انتقال بانکی، کد تخفیف |
| 📜 **قرارداد دیجیتال** | امضای الکترونیکی نسخه‌بندی‌شده |
| 🔑 **مدیریت لایسنس** | امضای Ed25519، اعتبارسنجی آفلاین |
| 💬 **پشتیبانی تلگرام** | چت زنده با اتصال به تلگرام شخصی |
| 📊 **داشبورد ادمین** | آنالیتیکس، SEO، بلاگ، خبرنامه |
| 📱 **PWA** | قابل نصب روی موبایل |

### Tech Stack

```
Next.js 16  ·  React 19  ·  TypeScript  ·  Tailwind CSS 4
PostgreSQL  ·  Prisma 7  ·  NextAuth  ·  BullMQ  ·  Redis
Framer Motion  ·  Anime.js  ·  next-intl  ·  Zod
```

### معماری (خلاصه)

```mermaid
graph TB
    subgraph Client
        A[Browser / PWA]
    end
    subgraph Next.js App
        B[App Router + i18n]
        C[Admin Panel]
        D[Client Portal]
        E[API Routes]
    end
    subgraph Services
        F[PostgreSQL]
        G[Redis Queue]
        H[Telegram Webhook]
    end
    A --> B
    B --> C & D
    C & D --> E
    E --> F & G & H
```

### اسکرین‌شات‌ها

> UI/UX طراحی و پیاده‌سازی شده — سورس کامل در ریپازیتوری عمومی موجود نیست.

| صفحه | لینk |
|---|---|
| صفحه اصلی | [hatamidev.com](https://hatamidev.com) |
| محصول Vendrix | [hatamidev.com/fa/products/panelfull](https://hatamidev.com/fa/products/panelfull) |
| قیمت‌گذاری | [hatamidev.com/fa/pricing](https://hatamidev.com/fa/pricing) |
| بلاگ | [hatamidev.com/fa/blog](https://hatamidev.com/fa/blog) |

### Build Status

✅ Production build verified — Next.js 16.2.10 (Webpack) — 195 routes compiled successfully.

---

## English

> **Note:** This repository is a **public showcase only**. The full source code is proprietary commercial software and is **not published** here.

### About

[hatamidev.com](https://hatamidev.com) serves dual purposes:

1. **Personal portfolio** — showcasing skills, projects, and experience
2. **License commerce platform** — selling, activating, and managing Vendrix (e-commerce panel) licenses

### Key Features

- **Trilingual** (FA / EN / DE) with SEO-optimized routing
- **Cinematic UI** with Framer Motion and Anime.js
- **Client portal** for license management, downloads, and support
- **Payment system** — PayPal, bank transfer, discount codes
- **Digital contracts** with versioned e-signatures
- **License management** — Ed25519 signed certificates, offline validation
- **Telegram-integrated support chat**
- **Admin dashboard** — analytics, SEO, blog, newsletter
- **PWA** — installable on mobile devices

### Tech Stack

Next.js 16 · React 19 · TypeScript · Tailwind CSS 4 · PostgreSQL · Prisma 7 · NextAuth · BullMQ · Redis

### Live Demo

🌐 **[hatamidev.com](https://hatamidev.com)**

---

## License

© 2024–2026 Mehran Hatami. All rights reserved.

This is proprietary software. No part of this project may be copied, modified, or distributed without explicit written permission from the author.

For licensing inquiries: [mehran873@gmail.com](mailto:mehran873@gmail.com) · [Telegram @hatamidev](https://t.me/hatamidev)

---

<div align="center">

**Built with ❤️ by [Mehran Hatami](https://hatamidev.com)**

[GitHub](https://github.com/HatamiDev) · [LinkedIn](https://www.linkedin.com/in/mehranhatami1) · [Instagram](https://www.instagram.com/mehranhatami_)

</div>
