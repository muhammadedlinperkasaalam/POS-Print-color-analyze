# AddintaPOS: in-house point-of-sale for a print shop

A web POS I built and run at Addinta Printing, Surabaya. It takes customer
files from WhatsApp, analyzes color coverage per page, prices each job
automatically, and handles checkout, receipts, and WhatsApp delivery.

**Stack:** PHP · MySQL · JavaScript (jQuery, AJAX) · Node.js

**Result:** a 30-page color check went from 5-10 minutes to about 1 minute.

> Customer data in these screenshots is blurred. Source code is private.

## Screenshots

### 1. Print Analyzer
![Print Analyzer](<img src="screenshots/01-print-analyzer.png" alt="Print Analyzer" width="700">)
Uploads or WhatsApp files are previewed page by page, classified by color
coverage, and priced from a configurable price profile, with per-sheet
correction before checkout.

### 2. WhatsApp file intake
![WhatsApp file intake](screenshots/02-whatsapp-intake.png)
A Node.js WhatsApp gateway downloads customer files automatically; files are
grouped by sender and can be analyzed one by one or in a batch.

### 3. Cashier screen
![Cashier screen](screenshots/03-cashier.png)
Analyzed jobs flow into the cart grouped by customer file, with quantity,
discount, delivery fee, cash-denomination buttons, and keyboard shortcuts.

### 4. Receipt and WhatsApp delivery
![Receipt](screenshots/04-receipt.png)
After payment: printable receipt, change, order-queue handoff, and the
receipt sent to the customer over the same WhatsApp gateway.

### 5. Color detection settings
![Color settings](screenshots/05-color-settings.png)
Adjustable grayscale tolerance, near-white cutoff, tier thresholds, and
sampling size across five color tiers.

## Contact
Muhammad Edlin Perkasa Alam · muhammad.edlin@gmail.com