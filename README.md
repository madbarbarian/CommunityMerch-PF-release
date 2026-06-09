# Community Merch Fundraising Platform

> **White-label print-on-demand fundraising platform for schools, PTAs, sports teams, and community organizations.**

[![Next.js](https://img.shields.io/badge/Next.js-16-black)](https://nextjs.org)
[![Turso](https://img.shields.io/badge/Turso-SQLite-green)](https://turso.tech)
[![Stripe](https://img.shields.io/badge/Stripe-Connect-blueviolet)](https://stripe.com)
[![Vercel](https://img.shields.io/badge/Vercel-Deploy-black)](https://vercel.com)

A licensable SaaS platform that enables organizations to design and sell custom merchandise for fundraising — with zero inventory risk. Built on Printful POD, Stripe Connect, and optional AI design generation.

---

## ▲ Deploy to Vercel

> ⚠️ **デプロイ前に必ずお読みください**
> → **[セットアップガイドを別タブで開いてから](docs/00-START-HERE.md)** ボタンをクリックしてください。
> 各入力欄の「📖」リンクからもガイドを確認できます。

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/madbarbarian/CommunityMerch-PF-release&env=TURSO_DATABASE_URL,TURSO_AUTH_TOKEN,BETTER_AUTH_SECRET,BETTER_AUTH_URL,NEXT_PUBLIC_APP_URL,GOOGLE_CLIENT_ID,GOOGLE_CLIENT_SECRET,RESEND_API_KEY,EMAIL_FROM,STRIPE_SECRET_KEY,STRIPE_PUBLISHABLE_KEY,STRIPE_WEBHOOK_SECRET,PRINTFUL_API_KEY,PRINTFUL_WEBHOOK_SECRET,CLOUDFLARE_R2_ACCOUNT_ID,CLOUDFLARE_R2_ACCESS_KEY_ID,CLOUDFLARE_R2_SECRET_ACCESS_KEY,CLOUDFLARE_R2_BUCKET_NAME,CLOUDFLARE_R2_PUBLIC_URL,OPENAI_API_KEY,CRON_SECRET,PLATFORM_ADMIN_EMAIL&envDescription%5BTURSO_DATABASE_URL%5D=Turso管理画面→DB名クリック→Connectタブ→Connection%20URL&envLink%5BTURSO_DATABASE_URL%5D=https://github.com/madbarbarian/CommunityMerch-PF-release/blob/main/docs/00-START-HERE.md&envDescription%5BTURSO_AUTH_TOKEN%5D=同じConnect画面→Create%20Token→Auth%20Token（一度だけ表示。必ずコピー）&envLink%5BTURSO_AUTH_TOKEN%5D=https://github.com/madbarbarian/CommunityMerch-PF-release/blob/main/docs/00-START-HERE.md&envDescription%5BBETTER_AUTH_SECRET%5D=ランダム文字列①。Macターミナルで%20openssl%20rand%20-base64%2032%20を実行してコピー&envLink%5BBETTER_AUTH_SECRET%5D=https://github.com/madbarbarian/CommunityMerch-PF-release/blob/main/docs/00-START-HERE.md&envDescription%5BBETTER_AUTH_URL%5D=デプロイ後のVercel%20URL。今は空欄でOK（デプロイ完了後に設定）&envLink%5BBETTER_AUTH_URL%5D=https://github.com/madbarbarian/CommunityMerch-PF-release/blob/main/docs/00-START-HERE.md&envDescription%5BNEXT_PUBLIC_APP_URL%5D=BETTER_AUTH_URLと同じURLを入力。今は空欄でOK&envLink%5BNEXT_PUBLIC_APP_URL%5D=https://github.com/madbarbarian/CommunityMerch-PF-release/blob/main/docs/00-START-HERE.md&envDescription%5BGOOGLE_CLIENT_ID%5D=Google%20Cloud%20Console→認証情報→OAuth%202.0→クライアントID&envLink%5BGOOGLE_CLIENT_ID%5D=https://github.com/madbarbarian/CommunityMerch-PF-release/blob/main/docs/00-START-HERE.md&envDescription%5BGOOGLE_CLIENT_SECRET%5D=Google%20Cloud%20Console→認証情報→OAuth%202.0→クライアントシークレット&envLink%5BGOOGLE_CLIENT_SECRET%5D=https://github.com/madbarbarian/CommunityMerch-PF-release/blob/main/docs/00-START-HERE.md&envDescription%5BRESEND_API_KEY%5D=Resend管理画面→API%20Keys→Create%20API%20Key&envLink%5BRESEND_API_KEY%5D=https://github.com/madbarbarian/CommunityMerch-PF-release/blob/main/docs/00-START-HERE.md&envDescription%5BEMAIL_FROM%5D=送信元メールアドレス。例:noreply@yourapp.com。ドメインなしはonboarding@resend.dev&envLink%5BEMAIL_FROM%5D=https://github.com/madbarbarian/CommunityMerch-PF-release/blob/main/docs/00-START-HERE.md&envDescription%5BSTRIPE_SECRET_KEY%5D=Stripe→Developers→API%20keys→Secret%20key（sk_live_...）&envLink%5BSTRIPE_SECRET_KEY%5D=https://github.com/madbarbarian/CommunityMerch-PF-release/blob/main/docs/00-START-HERE.md&envDescription%5BSTRIPE_PUBLISHABLE_KEY%5D=Stripe→Developers→API%20keys→Publishable%20key（pk_live_...）&envLink%5BSTRIPE_PUBLISHABLE_KEY%5D=https://github.com/madbarbarian/CommunityMerch-PF-release/blob/main/docs/00-START-HERE.md&envDescription%5BSTRIPE_WEBHOOK_SECRET%5D=今は空欄でOK。デプロイ後にStripe%20Webhookを設定してから追加します&envLink%5BSTRIPE_WEBHOOK_SECRET%5D=https://github.com/madbarbarian/CommunityMerch-PF-release/blob/main/docs/00-START-HERE.md&envDescription%5BPRINTFUL_API_KEY%5D=Printful→Settings→API→Generate%20API%20Key&envLink%5BPRINTFUL_API_KEY%5D=https://github.com/madbarbarian/CommunityMerch-PF-release/blob/main/docs/00-START-HERE.md&envDescription%5BPRINTFUL_WEBHOOK_SECRET%5D=今は空欄でOK。デプロイ後にPrintful%20Webhookを設定してから追加します&envLink%5BPRINTFUL_WEBHOOK_SECRET%5D=https://github.com/madbarbarian/CommunityMerch-PF-release/blob/main/docs/00-START-HERE.md&envDescription%5BCLOUDFLARE_R2_ACCOUNT_ID%5D=Cloudflareダッシュボード右サイドバーのAccount%20ID&envLink%5BCLOUDFLARE_R2_ACCOUNT_ID%5D=https://github.com/madbarbarian/CommunityMerch-PF-release/blob/main/docs/00-START-HERE.md&envDescription%5BCLOUDFLARE_R2_ACCESS_KEY_ID%5D=R2→Manage%20R2%20API%20Tokens→Create%20Token→Access%20Key%20ID&envLink%5BCLOUDFLARE_R2_ACCESS_KEY_ID%5D=https://github.com/madbarbarian/CommunityMerch-PF-release/blob/main/docs/00-START-HERE.md&envDescription%5BCLOUDFLARE_R2_SECRET_ACCESS_KEY%5D=Create%20Token→Secret%20Access%20Key（一度だけ表示。必ずコピーして保存）&envLink%5BCLOUDFLARE_R2_SECRET_ACCESS_KEY%5D=https://github.com/madbarbarian/CommunityMerch-PF-release/blob/main/docs/00-START-HERE.md&envDescription%5BCLOUDFLARE_R2_BUCKET_NAME%5D=R2で作成したバケット名。例:myapp-uploads&envLink%5BCLOUDFLARE_R2_BUCKET_NAME%5D=https://github.com/madbarbarian/CommunityMerch-PF-release/blob/main/docs/00-START-HERE.md&envDescription%5BCLOUDFLARE_R2_PUBLIC_URL%5D=R2バケット→Settings→Public%20Access→Public%20Bucket%20URL（https://pub-xxx.r2.dev）&envLink%5BCLOUDFLARE_R2_PUBLIC_URL%5D=https://github.com/madbarbarian/CommunityMerch-PF-release/blob/main/docs/00-START-HERE.md&envDescription%5BOPENAI_API_KEY%5D=【任意】OpenAI→API%20keys→Create%20new%20key。空欄でもOK（AI生成機能が使えなくなるだけ）&envLink%5BOPENAI_API_KEY%5D=https://github.com/madbarbarian/CommunityMerch-PF-release/blob/main/docs/00-START-HERE.md&envDescription%5BCRON_SECRET%5D=ランダム文字列②（BETTER_AUTH_SECRETとは別の値）。openssl%20rand%20-base64%2032%20で生成&envLink%5BCRON_SECRET%5D=https://github.com/madbarbarian/CommunityMerch-PF-release/blob/main/docs/00-START-HERE.md&envDescription%5BPLATFORM_ADMIN_EMAIL%5D=あなた自身のメールアドレス。このアドレスでGoogleログインするとプラットフォーム管理者になります&envLink%5BPLATFORM_ADMIN_EMAIL%5D=https://github.com/madbarbarian/CommunityMerch-PF-release/blob/main/docs/00-START-HERE.md)

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
