# VSCO Workspace - Email System

## Email Setup

**Location:** Settings > Mail Settings

### Mail Server Options:
1. **Gmail Integration (Google 2-way sync)** -- Works with @gmail.com and Google Workspace (G Suite). Outgoing emails appear in your Gmail sent folder; no BCC needed.
2. **Outlook Integration** -- Microsoft Outlook email support
3. **Custom SMTP Servers** -- For other email providers

### How Email Sending Works:
- Emails sent from Workspace go to the recipient's inbox
- When recipients reply, responses go to your normal email client (unless using Gmail Integration)
- To log replies without Gmail integration, forward them to the brand's **BCC address**

### BCC Address:
- Each brand has a unique BCC address for importing communications
- Forward client replies to this address to keep all communication tracked
- Not needed if using Gmail Integration (2-way sync handles automatically)

### Brand Sender:
- The email used to send automated messages (payment receipts, automation emails)
- Select from any Gmail, Custom SMTP, or Outlook email you've integrated

---

## Gmail Integration

**Location:** Settings > Mail Settings > New Integration > Google (2-way sync)

### Features:
- Works with @gmail.com and Google Workspace (G Suite)
- Creates an "Import to VSCO Workspace" label in Gmail for quick message import
- Email tracking: Sent, Delivered, Opened, Read, Link Clicked status
- Access to templates, tokens, branding, and automations
- Full two-way sync -- no BCC needed

---

## Email Templates

**Location:** Settings > Email Templates

### Creating Templates:
- Build new templates at Settings > Email Templates
- Quick-create by clicking "Save as Template" from any email you're composing

### Template Types (determines available tokens and where it can be used):
- **General Use** -- Inquiry responses, follow-ups; available in Compose dropdown on the job's Mail tab
- **Quote Invitation** -- For sending quotes/proposals
- **Questionnaire Invitation** -- Uses `{{item.name_link}}` token for the questionnaire link
- **Contract Invitation** -- For sending contracts outside of a quote
- **Invoicing** -- Shown when emailing an invoice link
- **Order Receipts** -- Accessible when emailing an order's direct link

---

## Tokens

Tokens are placeholders in double curly brackets `{{ }}` used in emails, contracts, and questionnaires.

### Key Token Categories:

**Brand Tokens:**
- `{{brand.name}}`, `{{brand.email}}`, `{{brand.website}}`
- `{{brand.email_signature}}`, `{{brand.location}}`, `{{brand.office_hours}}`
- `{{brand.client_portal_linked}}`, `{{brand.client_portal_url}}`

**Job Tokens:**
- `{{job.name}}` -- Full name of the job
- `{{job.everyone.first_names}}` -- List of every contact's first name

**Recipient Tokens:**
- Auto-populate with each recipient's info when sending to multiple people

**Invoice Tokens:**
- `{{invoice.balance}}`, `{{invoice.due_date}}`, `{{invoice.due_period}}`

**Payment Schedule Tokens:**
- `{{payment_schedule.retainer}}`, `{{payment_schedule.final_amount}}`
- `{{payment_schedule.summary_list}}`

**Item Tokens:**
- `{{item.name_link}}` -- Links to questionnaires, invoices, etc.

**Client Portal Token:**
- `{{recipient.portal_linked}}` -- Link to the client portal

**Custom Field Tokens:**
- `{{job.custom.custom-field-token}}` or role-based prefix variations
- Auto-generated when you create a custom field

Creating a new Job Role, Event Type, or Custom Field automatically generates a full set of tokens.

---

## Email Signatures

**Location:** Settings > Branding (Look & Feel section)

- One email signature per Brand
- Add images using the "Insert File" option in the editor bar
- Resize images by clicking and using the adjustment handle
- Use `{{brand.email_signature}}` token in templates and manually drafted emails
- For multi-brand accounts, the token auto-populates the correct signature based on the job's brand

---

## Email Deliverability

### Mail Log:
**Location:** Email Activity Log (left sidebar) or Mail tab on a job's profile page

### Email Status Categories:
- **Sent** -- Message transferred to your email server, queued for delivery
- **Delivered** -- Message reached the client's email server (doesn't guarantee they saw it)
- **Opened** -- Tracking image was loaded (note: opening in your Gmail sent folder also triggers this)
- **Bounced** -- Rejected by client's mail server (misconfigured server, incorrect domain, flagged as spam)
- **Clicked** -- Link in email was clicked (most reliable confirmation)

---

## SPF Records

**Purpose:** DNS TXT record that helps email providers determine message authenticity.

**Who needs it:** Only if using the legacy mailer system. NOT needed for Gmail integration, Outlook, or Custom SMTP.

### Setup:
1. Add a TXT record to your domain's DNS settings
2. VSCO Workspace IP: `50.31.39.46`
3. Set TTL low initially (3600 seconds / 1 hour)
4. Verify using the SPF verification form

**Troubleshooting:** If mail isn't delivered at all (not even to spam), you likely already have an SPF record that doesn't include Workspace.

---

## DKIM Records

**Purpose:** Prevent outgoing emails from being marked as spam.

### Setup:
1. Log into your domain host
2. Add the DKIM TXT record
3. Copy DNS Host name to Host field
4. Copy TXT record value to TXT Value field
5. In Google, select "Start Authentication"
6. Status should change from "Not Authenticating Email" to "Authenticating Email"

Recommended alongside SPF records for best deliverability.

---

## Mass Emails

Workspace does NOT have direct integration with MailChimp, Flodesk, or similar services.

### Workaround:
1. Download contacts from Address Book or filtered Leads/Jobs sidebar lists as CSV
2. Upload to external email service
3. Download via the download icon (top right of your list)
4. Options: download only visible columns or all columns
5. Create tailored lists using custom reports and tagging in Address Book
