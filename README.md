# Community Merch Fundraising Platform

> **White-label print-on-demand fundraising platform for schools, PTAs, sports teams, and community organizations.**

[![Next.js](https://img.shields.io/badge/Next.js-16-black)](https://nextjs.org)
[![Turso](https://img.shields.io/badge/Turso-SQLite-green)](https://turso.tech)
[![Stripe](https://img.shields.io/badge/Stripe-Connect-blueviolet)](https://stripe.com)
[![Vercel](https://img.shields.io/badge/Vercel-Deploy-black)](https://vercel.com)

A licensable SaaS platform that enables organizations to design and sell custom merchandise for fundraising — with zero inventory risk. Built on Printful POD, Stripe Connect, and optional AI design generation.

---

## ▲ Deploy to Vercel

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/madbarbarian/CommunityMerch-PF-release&env=TURSO_DATABASE_URL,TURSO_AUTH_TOKEN,BETTER_AUTH_SECRET,BETTER_AUTH_URL,NEXT_PUBLIC_APP_URL,GOOGLE_CLIENT_ID,GOOGLE_CLIENT_SECRET,RESEND_API_KEY,EMAIL_FROM,STRIPE_SECRET_KEY,STRIPE_PUBLISHABLE_KEY,STRIPE_WEBHOOK_SECRET,PRINTFUL_API_KEY,PRINTFUL_WEBHOOK_SECRET,CLOUDFLARE_R2_ACCOUNT_ID,CLOUDFLARE_R2_ACCESS_KEY_ID,CLOUDFLARE_R2_SECRET_ACCESS_KEY,CLOUDFLARE_R2_BUCKET_NAME,CLOUDFLARE_R2_PUBLIC_URL,OPENAI_API_KEY,CRON_SECRET,PLATFORM_ADMIN_EMAIL)

Clicking the button opens Vercel's guided setup — you'll be prompted to enter each service credential with a description of where to find it.

> **Before deploying:** Prepare your service accounts and credentials first.
> → **[Licensee Preparation Checklist](docs/licensee-preparation-checklist.md)**

**【日本語補足】** デプロイボタンを押すと、Vercel の画面で必要な認証情報を1つずつ入力するフローが始まります。事前に各サービスのアカウントを作成し、APIキーを取得しておく必要があります。準備手順は上記チェックリストを参照してください。

---

## 📦 What You Get

- **Organization management** — Multi-tenant with 4 roles: Admin / Member / Student / Buyer
- **Campaign creation wizard** — Design upload + AI design generation (OpenAI gpt-image-1)
- **Print-on-demand fulfillment** — Automatic order submission to Printful, ships to buyer's home
- **Stripe Connect payments** — Org bank account payouts with configurable platform fee
- **T-shirt mockup preview** — Printful Mockup Generator API integration
- **Platform admin panel** — Business operator control center (`/admin`) with discount codes, org management, staff roles
- **Setup Wizard** — 9-step onboarding for first-time licensee configuration
- **White-label** — All branding (name, colors, domain) configured via Setup Wizard — zero hardcoded brand data

**【日本語補足】** このプラットフォームはホワイトラベル設計です。サービス名・ロゴ・カラーなどの識別情報は一切コードにハードコードされておらず、セットアップウィザードで設定します。ライセンシーは自分のブランドでインスタンスを展開できます。

---

## 🚀 Setup Flow

1. **Prepare** — Create accounts and gather credentials for all required services
   → [Licensee Preparation Checklist](docs/licensee-preparation-checklist.md)

2. **Deploy** — Click the **Deploy to Vercel** button above and enter your credentials when prompted

3. **Configure** — After deployment, visit `/setup` to complete the Setup Wizard:
   - Step 1: Accept the license agreement
   - Step 2: Set your brand identity (name, tagline, colors, domain, support email)
   - Steps 3–8: Verify each service is connected (Turso, Stripe, Printful, Resend, OpenAI, R2)
   - Step 9: Launch — your platform goes live and you're redirected to `/admin`

4. **Manage** — Use `/admin` as your platform control panel

→ **[Full Setup Guide](docs/00-START-HERE.md)**

---

## 🔧 Required Services

| Service | Purpose | Free Tier |
|---------|---------|-----------|
| [Turso](https://turso.tech) | Database | 9GB, never pauses |
| [Stripe](https://stripe.com) | Payments + Connect | Pay-as-you-go |
| [Printful](https://printful.com) | Print-on-demand fulfillment | Free (per order) |
| [Resend](https://resend.com) | Transactional email | 100/day free |
| [Cloudflare R2](https://cloudflare.com/r2) | File storage | 10GB/mo free |
| [Google Cloud](https://console.cloud.google.com) | OAuth login | Free |
| [OpenAI](https://platform.openai.com) | AI design generation | Optional, ~$0.04/image |

**【日本語補足】** 必須サービスはすべて無料枠が充実しており、小〜中規模の運用では費用がほとんどかかりません。OpenAIはオプションです（AI生成デザイン機能が必要な場合のみ）。

---

## License

Proprietary. All rights reserved.

This platform is licensed, not sold. Each deployment requires a separate license agreement. Contact the IP owner for licensing terms.

**【日本語補足】** このプラットフォームはオープンソースではありません。ライセンス契約に基づいてのみ使用できます。ライセンス取得については IP オーナーにお問い合わせください。
