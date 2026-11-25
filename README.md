### Hi, I'm Nahom 👋

**Mobile Engineer (Flutter) · Addis Ababa, Ethiopia · open to remote work**

I build production mobile and operational systems for commerce, logistics, POS and hospitality, the kind that have to keep working when the network doesn't. At Red Cloud ICT Solutions I was responsible for five interconnected Flutter apps used daily by 700+ businesses across Ethiopia, processing 20M+ ETB a day in cash and mobile-money payments.

---

#### What I've shipped

- **CNDroid POS** (Android, on certified fiscal devices)
  - Re-architected offline selling on encrypted SQLite, so 200+ restaurants and 350+ distributors keep trading through internet and server outages.
  - Built LAN mode from scratch: one Android till runs a local server for the whole branch, serving the other tills and kitchen screens.
  - Built e-invoicing for the Ministry of Revenues system: A4 invoice rendering in native Android, thermal printing, email and SMS sharing, signed QR codes.
  - Introduced the app's first automated test suite (about 200 tests).
- **HuluBeje Delivery** (driver app)
  - Dual-provider routing with automatic fallback, retry and route caching.
  - Live trips that react when a customer cancels or changes the address mid-delivery.
- **HuluBeje** (consumer super-app, 60K+ downloads)
  - Runs as a mini-app inside telebirr and Bank of Abyssinia's super-app; I led the client-side integration with Bank of Abyssinia, working with their team.
  - Post-payment order changes between dine-in, pickup and delivery.
  - [Google Play](https://play.google.com/store/apps/details?id=com.cnetsoftwares.cnetpay_client) · [App Store](https://apps.apple.com/us/app/hulubeje-hulu-beje/id1661524972)

> The production code belongs to my employer and is private, so I document the architecture instead.

#### Architecture case studies

How I designed these systems: problem, constraints, architecture diagrams, decisions and trade-offs.

- **[Selling through outages: offline and LAN mode for a production POS](https://github.com/Nahmeg28/engineering-case-studies/blob/main/01-offline-lan-pos.md)**: encrypted SQLite, an on-device branch server, sync and concurrency.
- **[Routing that doesn't strand drivers: dual-provider fallback](https://github.com/Nahmeg28/engineering-case-studies/blob/main/02-dual-provider-routing.md)**: retry with backoff, caching, provider abstraction.
- **["Saved" should mean saved: offline mode that survives power cuts](https://github.com/Nahmeg28/engineering-case-studies/blob/main/03-offline-durability.md)**: root-causing data loss, encrypted SQLite, sync races.
- **[From a Unilever order to a fiscal receipt, unattended](https://github.com/Nahmeg28/engineering-case-studies/blob/main/04-unilever-order-pipeline.md)**: third-party integration with fiscal hardware.
- **[Making the fiscal printer and the ERP agree](https://github.com/Nahmeg28/engineering-case-studies/blob/main/05-fiscal-reconciliation.md)**: automatic reconciliation driven by a tested decision table.
- **[Debugging notebook: five production bugs](https://github.com/Nahmeg28/engineering-case-studies/blob/main/06-debugging-notebook.md)**: symptom, root cause, fix, lesson.
- **[E-invoicing with the tax authority's signed QR](https://github.com/Nahmeg28/engineering-case-studies/blob/main/07-e-invoicing-signed-qr.md)**: Ministry of Revenues integration, printer selection, failing early.

Everything I shipped on the POS, release by release: **[contributions](https://github.com/Nahmeg28/engineering-case-studies/blob/main/CONTRIBUTIONS.md)**. Shorter design decisions: **[engineering notes](https://github.com/Nahmeg28/engineering-case-studies/blob/main/engineering-notes/README.md)**.

Screenshots and more on my **[portfolio](https://nahomulugeta-port.vercel.app/)**.

---

#### Stack

**Mobile:** Flutter · Dart · Java (Android platform channels) · SQLite / sqflite · Hive
**Architecture:** BLoC · Stacked (MVVM) · Provider · get_it · repository and service layers
**Integrations:** REST APIs (.NET, NestJS) · Firebase Cloud Messaging · Supabase · maps and routing · fiscal printers · QR and mobile-money payments
**Web:** JavaScript · TypeScript · React
**Also:** C# / .NET · Figma (UI/UX design)

---

#### Get in touch

[Email](mailto:nahmulu28@gmail.com) · [LinkedIn](https://www.linkedin.com/in/nahom-mulugeta-nimb28) · [Portfolio](https://nahomulugeta-port.vercel.app/)
