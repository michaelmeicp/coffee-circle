# Coffee Circle

Independent, bilingual group drink requests for Hong Kong and Macau. This is not an official Starbucks ordering or payment service; no Starbucks logo or product imagery is used.

The organizer creates a group, enters their own password (at least 8 characters), and shares the participant link or QR. Save the private organizer link and password separately. Participants enter a nickname and drink preferences, then keep their private edit link for changes before cutoff. Organizer costs and store information remain private. Unknown prices remain unknown.

This repository contains the static GitHub Pages frontend only. Its public API configuration points to the existing Coffee Circle Worker. It contains no database, orders, credentials or private links. Organizer sessions are kept in memory; refreshing requires the password again.

Daily request clearing is configured for 23:59 Macau; group settings and catalog remain. The organizer must update the next day's cutoff. Actual cron execution and free-tier limits still require production monitoring; provider backups and copied lists are outside live-record clearing.

Menu choices are preferences to confirm with the chosen store, not a verified live regional menu or price list. Source references: [Hong Kong drinks](https://www.starbucks.com.hk/en/catalog/category/view/s/drinks/id/70/), [coffees](https://www.starbucks.com.hk/en/catalog/category/view/s/coffees/id/74/), and [customization FAQ](https://www.starbucks.com.hk/questions-about-mobile-order-to-table). Names were researched on 2026-10-03; Macau availability and detailed option matrices remain unverified.

QR generation uses qrcode-generator; see QR-LICENSE.txt. Real iOS/Safari and multiple physical devices require a final user check.
