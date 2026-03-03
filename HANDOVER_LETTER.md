# AFPAConnect Platform — Project Handover Agreement Letter

**Date:** March 1, 2026
**From:** [Your Name / Your Company]
**To:** AFPA (American Franchise Professionals Association)
**Re:** Transfer of AFPAConnect Web Platform — 10-Month Installment Transfer Plan

---

## Overview

This letter outlines the terms under which the AFPAConnect web platform will be handed over to AFPA. The transfer is structured across **10 monthly installment payments**. Access to the platform, its source code, and its underlying infrastructure will be granted in stages, with full and unconditional ownership transferring only upon receipt of the final payment.

---

## What Is Being Transferred

The AFPAConnect platform is a full-stack web application. Upon completion of all payments, AFPA will receive full ownership and control of the following:

### 1. Source Code
- The complete Next.js 14 application codebase (App Router architecture)
- All components, pages, API routes, and utility libraries
- Database schema files and migration scripts (11 SQL migrations)
- Configuration files (Next.js, Tailwind CSS, TypeScript, PostCSS)
- The private GitHub (or equivalent) repository with full commit history

### 2. Hosting & Deployment
- The **Vercel** project account (or transfer of the deployment to AFPA's own Vercel account)
- All production environment variables and build settings
- Domain DNS configuration records (A records + CNAME)

### 3. Database & Authentication (Supabase)
- Full ownership of the **Supabase** project (`buusmlcevpmczmnwcryc.supabase.co`)
- Transfer of the Supabase organization to an AFPA-owned account
- All production data: franchise listings (600+), user profiles, quiz results, leads, applications, assessments, blog posts, and analytics
- All Supabase storage buckets (images, documents, logos)
- The **Service Role Key** (admin-level database access that bypasses row-level security)
- The Anon/Public key

### 4. Third-Party Service Credentials
- **OpenAI API key** — powers the AI franchise matching engine (quiz results, embeddings)
- **Resend API key** — powers all transactional email (quiz confirmations, lead notifications)
- **Google OAuth credentials** — powers the analytics dashboard (Google My Business, Google Ads, Google Analytics)
- **Meta / Facebook App credentials** — powers the Meta Ads analytics integration
- **LinkedIn OAuth credentials** — powers the LinkedIn Ads analytics integration

### 5. Documentation
- A handover guide explaining the role-based access system (5 roles: admin, advisor, franchisor, franchise_rep, user)
- Environment variable reference sheet
- Instructions for managing franchise listings, user accounts, advisor profiles, and quiz data
- Notes on the AI matching system (OpenAI GPT-4o-mini + text-embedding-3-small)

---

## Staged Access During the Payment Period

To protect both parties, access will be granted in stages as payments are received. **Full production control will not transfer until the final payment is made.**

### Immediately Upon Signing (Month 0)
- Read access to the source code repository (view/clone, no push access to the main branch)
- Access to a **staging/preview environment** (a separate Vercel preview deployment) for testing and review
- Written documentation of the platform architecture and all service dependencies

### Upon Each Monthly Payment (Months 1–9)
- AFPA may request specific content changes, configuration updates, or new features, which will be implemented by [Your Name] within the terms of this agreement
- AFPA receives a monthly status report confirming the platform's operational health
- After **Payment 5 (Month 5):** AFPA receives read-only access to the Supabase dashboard (can view data, reports, and schema — cannot modify service role keys or project settings)
- After **Payment 7 (Month 7):** AFPA receives the ability to push approved content changes to a staging branch (reviewed and merged by [Your Name])

### Upon Final Payment (Month 10) — Full Transfer
- Full repository ownership transferred (AFPA becomes admin on the GitHub org/repo)
- Supabase project transferred to AFPA's Supabase organization
- All third-party API keys and credentials transferred or regenerated under AFPA's accounts
- Vercel project transferred to AFPA's Vercel account
- Domain DNS control transferred
- All environment variables delivered in writing
- [Your Name] removed as an owner/admin from all services

---

## What Remains Retained Until Final Payment

The following items remain under [Your Name]'s control until all 10 payments are received in full. This is a standard protection for installment-based asset transfers:

| Item | Retained Until |
|------|----------------|
| Supabase Service Role Key (admin DB access) | Final payment |
| Vercel account ownership / deployment control | Final payment |
| Domain registrar control | Final payment |
| Main branch push access (production deploys) | Final payment |
| OpenAI, Resend, Google OAuth credentials | Final payment |
| Full GitHub repository admin rights | Final payment |

**Note:** AFPA will not have the ability to independently deploy to production, modify the database schema, transfer services to new accounts, or regenerate API keys until the final payment is received. This ensures continuity of the business relationship and protects the value of the asset being sold.

---

## Continuity & Support During the Transfer Period

During the 10-month payment period, [Your Name] agrees to:

- Maintain the platform in operational condition (hosting, database, email, AI features)
- Apply critical security patches and dependency updates as needed
- Remain available for questions, minor content changes, and bug fixes (reasonable scope to be agreed in a separate support agreement if applicable)
- Not make material changes to the platform's structure or functionality without AFPA's approval

AFPA agrees to:

- Make payments on schedule as agreed
- Not attempt to circumvent access controls, extract credentials, or independently transfer services during the payment period
- Not engage a third party to replicate or redeploy the platform during the payment period
- Notify [Your Name] of any issues or required changes through agreed communication channels

---

## Default Clause

If AFPA fails to make a scheduled payment within **[X] days** of the due date, [Your Name] reserves the right to:

1. Suspend AFPA's staging/preview environment access
2. Place the platform into maintenance mode until payment is received
3. Treat the agreement as void if **two or more payments** are missed, in which case all previously transferred materials (partial code access, documentation) must be returned or deleted, and no further transfer will occur

---

## Technical Contact & Transition Notes

The platform was built and is currently maintained by:

**[Your Name]**
**Email:** [your@email.com]
**Phone:** [your phone]

Key technical notes for AFPA's incoming technical team:

- The platform runs on **Next.js 14 (App Router)**. A developer familiar with React and Next.js will be required for any ongoing development.
- The database is **Supabase (PostgreSQL)**. Row-level security (RLS) is enabled and the admin Service Role Key must be kept private — it grants unrestricted database access.
- The AI features require an active **OpenAI account with billing enabled**. Costs scale with quiz volume.
- Email notifications require an active **Resend account**. Current sender domain must be re-verified if the sending domain changes.
- The analytics dashboard (Google, Meta, LinkedIn) requires OAuth re-authorization if credentials change.
- **No mobile app** exists — this is a web-only platform accessible on all screen sizes.

---

## Signatures

By signing below, both parties agree to the terms of this staged handover agreement.

---

**[Your Name / Company]**

Signature: ___________________________

Date: ___________________________

---

**AFPA Authorized Representative**

Name: ___________________________

Title: ___________________________

Signature: ___________________________

Date: ___________________________

---

*This letter constitutes an agreement of intent. Both parties are advised to have this document reviewed by legal counsel before signing. A formal contract with binding payment terms, default remedies, and IP assignment language should be drafted by an attorney.*
