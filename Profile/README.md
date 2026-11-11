# KyoRox — Stateless SAML 2.0 to HS256 JWT Middleware Proxy

**Official Platform:** [https://kyorox.com](https://kyorox.com) • **Developer Docs:** [https://kyorox.com/docs](https://kyorox.com/docs) • **Trust & Security:** [https://kyorox.com/trust](https://kyorox.com/trust) • **Live Status:** [https://kyorox.com/status](https://kyorox.com/status)

KyoRox is an engineering-first B2B authentication middleware engine that converts complex enterprise **OASIS SAML 2.0 XML assertions** (Okta, Microsoft Entra ID, Google Workspace, JumpCloud, PingIdentity, and Custom SAML 2.0) into deterministic, cryptographically signed **`HS256` JSON Web Tokens (JWT)** in under 12 milliseconds.

---

### Core Architectural Guarantees

* **100% Stateless Volatile RAM Execution (`0 Bytes` End-User PII on Disk):** Incoming SAML XML responses are verified, normalized, and signed strictly in volatile memory. Immediately after the HTTP redirect handoff, the buffer is garbage-collected.
* **Defense-in-Depth Cryptography:**
  * Pinned **X.509 `RSA-SHA256`** XML signature validation with built-in XXE and XML Signature Wrapping (XSW) shields.
  * **300-Second Atomic Nonce Replay Lock** preventing Man-in-the-Middle assertion replay attacks.
  * **FIPS-197 `AES-256-GCM`** authenticated vault encryption at rest for tenant signing secrets (unique 96-bit IV + 128-bit Auth Tag).
  * Constant-time **`SHA-256`** API key authentication (`kx_live_...`).
* **Transparent Flat-Rate Tiers (`$0 MAU Tax`):**
  * **Starter (`$39/mo`):** 1 Active SAML IdP Connection, Unlimited Monthly Active Users & Logins.
  * **Growth (`$139/mo`):** Up to 5 Active SAML IdP Connections, Unlimited Monthly Active Users & Logins.
  * **Enterprise (`$349/mo`):** Unlimited (999) Active SAML IdP Connections, Unlimited Monthly Active Users & Logins.
  * *(Prices exclude applicable local VAT/GST/Sales Tax calculated automatically at checkout via our Merchant of Record, Lemon Squeezy).*

---

### Official Open-Source Integration Examples

| Repository | Stack | Purpose |
| :--- | :--- | :--- |
| **[`kyorox-node-jwt-example`](https://github.com/kyorox-official/kyorox-node-jwt-example)** | Node.js / Express / Fastify (Zero External Deps) | Production reference showing how to initiate SSO and verify incoming `HS256` JWT handoffs from `sso.kyorox.com`. |
| **[`kyorox-python-jwt-example`](https://github.com/kyorox-official/kyorox-python-jwt-example)** | Python 3 / FastAPI / Flask | Production reference for verifying KyoRox `HS256` SAML-to-JWT callback tokens in Python backends. |

---

### Documentation & Enterprise Support

* **6-IdP Step-by-Step Integration Guides:** [https://kyorox.com/docs](https://kyorox.com/docs)
* **Customer Control Plane:** [https://kyorox.com/dashboard](https://kyorox.com/dashboard)
* **Security & Vulnerability Disclosure:** [https://kyorox.com/security](https://kyorox.com/security)
* **Support & Engineering Desk:** `support@kyorox.com` (24–36 Hour Response SLA)
