# Privacy Policy — FamAerie

**Last updated:** 17 July 2026  
**App:** FamAerie (package: `com.famaerie.app`)  
**Operator:** FamAerie / developer contact below

---

## 1. Introduction

This Privacy Policy explains how **FamAerie** processes personal data. FamAerie is a local-first family organiser. Sensitive financial and health content is encrypted on your device before it is stored or synced. Certain family-coordination data may sync in readable form so multiple devices in your family group stay consistent.

By creating or using a FamAerie account, you acknowledge the practices described here.

---

## 2. Who we are

For the purposes of India’s **Digital Personal Data Protection Act, 2023 (DPDP Act)**, the Data Fiduciary is **FamAerie** (“we”, “us”, “our”).

**Privacy contact:** afzalalikhan9@gmail.com  
**Subject line for grievances:** Privacy Grievance — FamAerie

If you are a child or a person with disability using FamAerie through a parent, guardian, or Head of Family account, that adult acts as the account controller for managed profiles.

---

## 3. Our privacy design

- **Local-first storage** — Most records live in an encrypted-capable local database on your phone.
- **Field-level encryption** — Designated sensitive fields (ledger amounts, bank SMS bodies, many health notes, remittance amounts, profile avatars, etc.) are encrypted on your device with **AES-256-GCM** under a Family Master Key our servers cannot decrypt.
- **Encrypted backups** — Backups uploaded to our servers are ciphertext. Recovery key material is wrapped with your PIN. We cannot decrypt those blobs without your PIN or device keys.
- **On-device AI** — Supported AI features run inference on your device after you download model weights. Prompt content for that local model is not sent to us for inference.

**Important:** FamAerie is not zero-knowledge for every field. Some identity, family-structure, and household-list data syncs in readable form so multi-device family features work.

---

## 4. Data we process

Depending on how you use FamAerie, we may process:

### A. Account & identity
- Display name and family name  
- Role within the family (Head of Family, spouse, child, grandparent, etc.)  
- Phone number (OTP sign-in via Firebase Authentication)  
- One-way hash of phone number and PIN (never plaintext PIN)  
- Device/session tokens  
- Optional profile photo (encrypted before sync)

### B. Sensitive vault content (encrypted on device before sync/backup)
- Financial ledger amounts, merchants, bank SMS bodies  
- Health notes, medication details, doctor notes (where marked sensitive)  
- Notes and remittance amounts (where marked sensitive)  
- Encrypted backup blobs and PIN-wrapped key bundles

### C. Family coordination data (may sync in readable form)
- Grocery/pantry item names, quantities, brands  
- Chore titles and reward metadata  
- Managed profile demographics (name, DOB, school, blood group)  
- Domestic help salary and attendance notes  
- Closet item names and household inventory labels  
- Ledger category labels, currencies, dates (not encrypted amounts)

### D. Device permissions & signals
- **SMS** (Android, if granted) — on-device bank SMS parsing  
- **Notifications** — reminders and family alerts  
- **Camera / gallery** — avatars or documents you capture  
- **Location** — only when you use features that require it (e.g. SOS)

### E. Technical & security logs
- App version, device type, crash/diagnostic events, API error codes

---

## 5. How we collect data

We collect data you enter; data from features you enable (e.g. SMS parsing); data synced between family devices you invite; and limited technical data when the app communicates with **nestii-backend.fly.dev**.

Phone OTP verification is performed by **Google Firebase Authentication**.

---

## 6. Purposes

We process data to:

- Create and secure your account and family group  
- Provide family CRM features (finance, kitchen, health, kids, chores, inventory, notes, calendar)  
- Sync authorised family devices and deliver encrypted backups  
- Send notifications you enable  
- Detect abuse, fraud, and security incidents  
- Comply with law and improve reliability

**We do not sell personal data. We do not use encrypted vault contents for advertising.**

---

## 7. Children & managed profiles

FamAerie is intended for family use. Profiles for children and managed members are created and controlled by an adult Head of Family or authorised managing member.

---

## 8. Sharing & processors

We share data only as needed to operate FamAerie:

| Processor | Purpose |
|-----------|---------|
| **Fly.io** (nestii-backend.fly.dev) | API hosting and databases |
| **Google Firebase** | OTP authentication and push notifications |
| **Open Food Facts** (via our API, optional) | Barcode/product lookup when you use it |
| **Hugging Face** (optional) | On-device AI model download when you install it |

Family members you invite may see family-shared data according to role. We do not sell data to brokers.

Emergency sharing you initiate (SOS / dialer / WhatsApp) leaves FamAerie under your control.

---

## 9. International transfers

Servers and processors may be located outside India. Encrypted vault blobs remain ciphertext in transit and at rest on our systems.

---

## 10. Retention

We retain account and sync data while your family group is active. Encrypted backups remain until you delete them or delete your family group. Local data remains on your device until you clear app data or uninstall.

---

## 11. Security

We use TLS in transit, AES-256-GCM for sensitive fields, X25519 key exchange, hashed PIN storage on servers, and device secure storage for master keys. You are responsible for protecting your device, PIN, and OTP access.

---

## 12. Your rights (DPDP Act)

You may request access, correction, erasure, or withdrawal of consent for optional processing. Contact **afzalalikhan9@gmail.com**.

Because many vault fields are encrypted with keys only you control, we may be unable to produce plaintext copies from our servers. You can view them on an unlocked device you control.

---

## 13. Changes

We may update this Policy. The “Last updated” date will change. Material changes will be highlighted in-app where practicable.

---

## 14. Governing law

This Policy is governed by the laws of **India**. Courts at **Bengaluru, Karnataka** have exclusive jurisdiction, subject to mandatory consumer or data-protection venues.

---

**Contact:** afzalalikhan9@gmail.com
