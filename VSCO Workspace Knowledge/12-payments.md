# VSCO Workspace - Payments

## Payment Gateways

**Location:** Settings > Client Payment Methods

### Online Payment Processors:
1. **Stripe**
2. **Square**
3. **PayPal Standard**

### Offline Payment Methods:
- "Mail a Check" (recommended minimum)
- Cash, wire transfer, etc.

---

## Stripe Payment Methods

Through Stripe's configuration, you can enable:
- **Credit Cards** (default)
- **ACH / Bank Transfer**
- **Apple Pay** (requires configuring your Workspace domain or custom domain)
- **Google Pay**
- **Cash App**
- **PayPal** (available in certain countries)

Access via "Configure Payment Methods" button within your Stripe integration.

---

## Square Payment Methods

- **Credit Cards** -- Enabled by default; can be disabled
- **ACH** -- Can be enabled; option to disable credit cards and only allow ACH

---

## ACH Payments

### Via Stripe:
1. Go to Settings > Client Payment Methods
2. Configure Stripe account
3. Enable ACH in payment methods
4. Clients see bank account option when paying an invoice
5. Client searches for their bank to connect and pay via ACH

### Via Square:
1. Go to Settings > Client Payment Methods
2. Connect Square account
3. Enable ACH Payment
4. Optional: Disable credit cards to only allow ACH

### Processing Timeline:
- ACH payments take **2-5 business days** to fully post
- Invoice is marked as **paid** upon successful initial transaction
- Payment shows as **Pending** on job ledger until fully posted
- Status updates from Pending to Posted

### Settlement Options (Square ACH):
- **Standard Settlement** -- Lower percentage processing fee, capped at $5
- **Two-Day Settlement** -- Higher percentage fee, no cap

---

## Credit Card Surcharges

**Location:** Settings > Client Payment Methods > Stripe/Square Configuration

### Setup:
- Check "Apply a surcharge fee to all credit card transactions"
- **Default rate:** 3%
- **Maximum rate:** 4%
- Customizable surcharge label on ledgers and payment screens (default: "credit card surcharge")

### Important Details:
- Surcharges apply ONLY to credit card payments
- NOT applied to ACH, Direct Debit, or other non-card methods
- Processing fees are taken from the total amount (including tax, tips, and surcharges)
- You can disable specific payment methods in Stripe to avoid certain fees

---

## Accepting Tips

Two options:
1. **Tips on Invoices** -- Accept tips directly through invoices alongside credit cards and ACH
2. **Standalone Tipping Page** -- Dedicated page for collecting tips outside normal invoice flow

Tips are included in the payment processing total (processing fees calculated on full amount including tips).

---

## Tax Settings

**Location:** Settings > Taxes & Currency (Admin-only access)

### Tax Rates:
- Enter various tax rates for your area
- Each rate can be set as **inclusive** or **exclusive**

### Tax Groups:
- Assigned to orders subject to sales tax
- Each group can contain **up to 3 separate tax rates**
- Select the applicable Tax Group when creating quotes/orders

### Product-Level Tax Control:
- Individual products can be marked as **non-taxable** by unchecking "Taxable"
