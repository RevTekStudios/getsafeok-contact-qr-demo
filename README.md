# Get Safe OK Contact QR — Sample Demo

This repository contains a **sample demonstration page** for [Get Safe OK](https://getsafeok.org). It shows what a **Contact QR Code Creator** could look like if Get Safe OK offered a tool like this to partners, advocates, and community organizations.

This is a **concept demo**, not a production service. It is meant to illustrate the user experience, workflow, and output — so stakeholders can evaluate whether this approach fits Get Safe OK’s mission and distribution model.

## What problem does this demo address?

Get Safe OK helps people find local victim and survivor services in Oklahoma. In some situations, someone may need a **discreet way to save a helpful phone number** on their device — one that does not obviously label itself as a crisis or victim-services contact.

This demo shows a tool that:

1. Lets a user pick a **local Oklahoma victim service** from a predefined list.
2. Builds a **neutral-sounding contact name** (for example, “Community Resources” or “Local Information”).
3. Embeds **search-friendly keywords** in the contact notes field.
4. Generates a **QR code** that, when scanned, prompts the phone to **add a saveable contact** (vCard) — no website visit or app install required.

The QR code encodes contact data directly. It does **not** link to a hosted page.

## What the demo includes

- A two-step layout: **setup form** on the left, **QR preview** on the right
- A dropdown of Oklahoma victim service phone numbers
- A “Random Name” option for neutral contact titles
- Editable keywords stored in the contact notes field
- QR code generation, PNG download, and clipboard copy
- A “Download Test Contact” option to verify the vCard before printing or sharing the QR code
- **Runs entirely in the browser** — no server, database, or hosting needed for the demo itself

## How to open the demo

1. Open `index.html` in a modern web browser (Chrome, Edge, Firefox, or Safari).
2. Enter the access password when prompted.
3. Select a local service, adjust the contact name and keywords if needed, then click **Generate Contact QR**.
4. Scan the QR code with a phone camera, or use **Download Test Contact** to inspect the contact file first.

Because everything runs locally, selections (such as the last chosen service) may be remembered on that device via browser storage.

## Intended audience for this sample

This page is primarily for **Get Safe OK stakeholders** — program staff, partners, and technical reviewers — to:

- See how a contact-based QR workflow might feel in practice
- Understand the privacy-oriented design choices (neutral naming, embedded vCard vs. public URL)
- Discuss whether a similar tool should be built, integrated, or distributed differently

It is **not** intended as a public-facing production app without further review, hardening, and organizational approval.

## Design notes

| Choice | Rationale |
|--------|-----------|
| vCard QR instead of URL | Scanning adds a contact immediately; no internet required after generation |
| Neutral contact names | Reduces obvious labeling of survivor/victim services on the device |
| Keywords in notes | Helps the contact surface in phone search without revealing service identity in the display name |
| Local-only execution | Keeps the demo simple and avoids storing sensitive configuration on a server |
| Password gate | Limits casual access while the sample is shared internally |

## Limitations of this demo

- Service list and contact defaults are **hard-coded** in the page
- Password protection is **basic** and suitable only for informal demos
- QR output should be **test-scanned** on target devices before any real-world use
- No analytics, user accounts, audit logging, or content management

## Credits

Built by [RevTek Studios](https://revtekstudios.com) as a sample for Get Safe OK.

QR code generation uses [Project Nayuki’s QR Code generator](https://www.nayuki.io/page/qr-code-generator-library) (MIT License).
