# KyoRox — Stateless Enterprise SAML 2.0 to HS256 JWT Authentication Middleware Proxy

[![Website](https://img.shields.io/badge/Website-kyorox.com-0d9488?style=for-the-badge)](https://kyorox.com)
[![SSO Gateway](https://img.shields.io/badge/Edge_Gateway-sso.kyorox.com-10b981?style=for-the-badge)](https://sso.kyorox.com)
[![Pricing](https://img.shields.io/badge/Flat_Pricing-$39%2Fmo_(%240_MAU_Tax)-065f46?style=for-the-badge)](https://kyorox.com/pricing)
[![Docs](https://img.shields.io/badge/Developer_Docs-5_Min_Quickstart-0f172a?style=for-the-badge)](https://kyorox.com/docs)

**KyoRox** ([https://kyorox.com](https://kyorox.com)) is an enterprise B2B stateless **OASIS SAML 2.0 to RFC 7519 HS256 JWT authentication middleware proxy**. Connect **Okta Workforce**, **Microsoft Entra ID (Azure AD)**, **Google Workspace**, **JumpCloud**, **PingIdentity (PingOne / PingFederate)**, **OneLogin**, and any Custom SAML 2.0 Identity Provider to your Node.js, TypeScript, Python, FastAPI, Django, Go, or Next.js application in **5 minutes** with **0 bytes of end-user PII stored on disk**.

---

## Why Engineering & InfoSec Teams Choose KyoRox Over Legacy SSO Brokers

- **100% Stateless Volatile RAM Execution (`< 12ms` P99 Latency)**: SAML 2.0 XML assertions are verified in volatile RAM and converted into a 300-second `HS256` JWT (`?access_token=<JWT>&token_type=Bearer&expires_in=300`). Memory buffers are garbage-collected immediately upon `HTTP 302` handoff—eliminating GDPR/HIPAA third-party employee directory storage liability.
- **Stateless Just-In-Time (JIT) Role Sync vs. Stateful SCIM**: Normalizes verified `sub`, `email`, `given_name`, `family_name`, and `roles` / `groups` (up to **256KB XML payloads / 650+ Active Directory groups**) directly inside the signed JWT.
- **Zero-Friction Customer IT Onboarding**:
  - **Hosted OASIS SP Metadata XML**: `https://sso.kyorox.com/metadata/{tenant_id}`
  - **1-Click IdP Metadata `.XML` & `.CER/.PEM` Auto-Extractor** inside [kyorox.com/dashboard](https://kyorox.com/dashboard)
  - **Zero-Downtime Multi-Certificate Rollover**: Pin up to 3 X.509 PEM certificates simultaneously
  - **Automated 30 / 14 / 7-Day X.509 Certificate Expiry Radar**
- **Flat-Rate Pricing ($0 Monthly Active User Tax Forever)**:
  - **Starter Plan ($39/mo)**: 1 Active SAML 2.0 IdP Connection, Unlimited Users & Logins
  - **Growth Multi-Tenant Plan ($139/mo)**: Up to 5 Active SAML 2.0 IdP Connections (78% savings vs. $125/connection brokers)
  - **Enterprise Scale Plan ($349/mo)**: Up to 999 Active SAML 2.0 IdP Connections, 99.9% Uptime SLA

---

## Official Open-Source Zero-Dependency JWT Verification Repositories

1. **Node.js / TypeScript Zero-Dependency HS256 Verifier**: [Kyorox-official/kyorox-node-jwt-example](https://github.com/Kyorox-official/kyorox-node-jwt-example)
2. **Python 3 Stdlib (`hmac.compare_digest`) Zero-Dependency HS256 Verifier**: [Kyorox-official/kyorox-python-jwt-example](https://github.com/Kyorox-official/kyorox-python-jwt-example)

---

## Platform & Documentation Links

- **Homepage & Live SAML-to-JWT Terminal**: [https://kyorox.com](https://kyorox.com)
- **Pricing & Competitor Cost-Savings Calculator**: [https://kyorox.com/pricing](https://kyorox.com/pricing)
- **6-IdP Integration Guides & API Reference**: [https://kyorox.com/docs](https://kyorox.com/docs)
- **Supported Enterprise Identity Providers**: [https://kyorox.com/integrations](https://kyorox.com/integrations)
- **Stateless RAM Architecture & Features**: [https://kyorox.com/features](https://kyorox.com/features)
- **B2B SaaS Deployment Blueprints**: [https://kyorox.com/customers](https://kyorox.com/customers)
- **Trust & Compliance Center**: [https://kyorox.com/trust](https://kyorox.com/trust)
- **Cryptographic Security Posture**: [https://kyorox.com/security](https://kyorox.com/security)
- **Live Gateway Uptime Telemetry**: [https://kyorox.com/status](https://kyorox.com/status)
