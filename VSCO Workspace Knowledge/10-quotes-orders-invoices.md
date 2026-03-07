# VSCO Workspace - Quotes, Orders, and Invoices

## Quotes

Quotes bundle products/services, questionnaires, contracts, and payment options into one easy-to-follow link for clients.

### Four Components of a Quote:
1. **Products & Services** -- Predetermined line items
2. **Payment Schedule** -- Determines invoice count and due dates
3. **Contracts** -- Legal agreements for client signature
4. **Questionnaires** -- Intake forms for client information

### Building a Basic Quote:
1. Go to the lead's job overview > Quotes & Orders > New Quote
2. Add recipient, quote name, message, expiration, sales tax group
3. Add products by selecting "Add Product" (search existing or Manual Entry)
4. Select a Payment Schedule (edit existing or Add New)
5. Optionally add a Questionnaire
6. Add a Contract
7. Save & Continue
8. Preview via direct link
9. Send via Email Quote button or automation
10. Save as template: Click "Copy to Quote Templates" for future use

### Advanced Quotes:
- Give clients multiple options to choose from during booking
- Allow selection from multiple payment schedule options
- Support filling out and signing multiple questionnaires and/or contracts
- Multiple quote options presented as "one or another" (clients can't remove or add items)
- Set default expiration dates
- Can be sent manually or by automation

### Upgradable Quotes:
- Offer tiered packages and optional add-ons
- Boost bookings by letting every client get exactly what they need

---

## Products & Services

**Location:** Settings > Products & Services

### Creating Products:
- Give it a type, name, and description
- Set pricing with multiple options and configurations
- Attach deliverable workflows if set up
- Mark as taxable or non-taxable
- Save with "Save As Product" for reuse

### Packages:
- Created in Settings as pre-configured bundles
- Added from the "Add Product" dropdown in quotes, quote templates, or orders
- Save time when building quotes for common service bundles

**Important:** Changes to products don't dynamically update existing product or quote templates. If products change, swap out old versions manually in templates.

---

## Orders

Two ways to create an order:
1. **From a quote**: When a client approves/books a quote, it becomes an order automatically
2. **Manually**: Create an order directly on the job

When a quote is approved:
- It becomes an open order
- The lead automatically moves to "Booked" stage
- Invoices are generated based on the payment schedule

---

## Invoices

Invoices are documents requesting specific payment from the client.

### How Invoices Work:
- Created automatically based on the payment schedule when an order is booked
- **100% due immediately** = ONE invoice with today's due date
- **50% retainer + balance on job date** = TWO invoices (one due today, one due on job date)
- Access invoices on the Quotes & Orders tab of the job
- Send invoice links via Invoicing email templates

### Automated Invoice Reminders:
- Set up automations to send payment reminders before/after due dates
- Track payment status in the job ledger

---

## Payment Schedules

Determines how an order is broken into invoices.

### Examples:
- 100% now = 1 invoice
- 50% retainer + 50% on job date = 2 invoices
- 33% retainer + 33% mid-point + 34% on delivery = 3 invoices

### In Advanced Quotes:
- Offer clients multiple payment schedule options to choose from

### Payment Schedule Tokens:
- `{{payment_schedule.retainer}}` -- Retainer amount
- `{{payment_schedule.final_amount}}` -- Final balance amount
- `{{payment_schedule.summary_list}}` -- Summary of the full payment schedule

---

## Discounts

- Discounts can be added to quotes or orders
- Can be set as **Pre-Tax** (standard pre-tax discount taken off before sales tax)
