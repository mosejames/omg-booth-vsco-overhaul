# VSCO Workspace - Integrations

## Zapier

**Location:** Settings > API Integrations

### Setup:
1. Go to Settings > API Integrations
2. Click "New Zapier Integration"
3. Click "Add the VSCO Workspace Zapier App" (opens Zapier)
4. Grab your unique API key
5. In Zapier, click "Add Connection" and paste the API key

### Available Triggers (data FROM Workspace):
- **Contact Created** -- When a new contact is created; sends contact details to another app
- **Order Booked** -- When a new order is booked (manual or electronic); sends order info
- **Payment Created** -- When a new payment is created; sends payment info

### Available Actions (data INTO Workspace):
- **Create a Job** -- Create jobs from external scheduling tools (Calendly, Acuity)
- **Create a Contact** -- Generate contacts from external sources; supports Additional Contact Fields and Contact Custom Fields mapping

### Specific Zapier Integrations:

**MailChimp:**
- Trigger: Contact Created in Workspace
- Action: Add/update subscriber in MailChimp
- Select Contact Kind (required) and Brand

**Acuity Scheduling:**
- Trigger: Acuity appointment scheduled
- Action: Create a Job in Workspace
- Must select Job Role from dropdown (cannot be mapped to Acuity field)

**Calendly:**
- Trigger: Calendly appointment scheduled
- Action: Create a Job in Workspace
- Map Calendly fields to Workspace job fields

### Zapier Webhooks:
- Use with Workspace's Web Request Automation action
- Enables advanced no-code integrations via incoming/outgoing HTTP requests

---

## ShootProof Integration

**Location:** Settings > Gallery Integrations

### Setup:
1. Click CONNECT on the ShootProof tile
2. Log into ShootProof and grant permissions
3. Set default order import settings (expense category, default payee)

### Features:
- Link ShootProof galleries to Workspace jobs
- Create new ShootProof galleries directly from jobs
- Import ShootProof orders to centralize financials
- If linked contact doesn't exist in ShootProof, Workspace creates it automatically

### Linking a Gallery:
1. Navigate to job overview > Galleries widget
2. Click Link Gallery > browse/search galleries
3. Select gallery and set which Workspace event it links to
4. Name the gallery, select preset, event, and linked contact

---

## Pic-Time Integration

**Location:** Settings > Gallery Integrations

### Setup:
1. Click CONNECT on the Pic-Time tile
2. Sign up or connect existing Pic-Time account
3. Must be logged into Pic-Time in the same browser
4. Click Approve in Pic-Time to grant access
5. Set default order import settings

### Features:
- Link Pic-Time galleries to Workspace jobs
- Create new Pic-Time galleries directly from jobs
- Import Pic-Time orders
- Display gallery cover photo in client emails
- Link multiple galleries to different events in the same job

---

## Fundy Order Imports

### Process:
1. Navigate to job's Quotes & Orders section
2. Click Import Order
3. Upload Fundy order XML file
4. Match up sales tax rates from the import to your Workspace tax settings

---

## WordPress Integrations

### Contact Form 7:
1. Install Contact Form 7 WordPress plugin
2. Install VSCO Workspace Contact Form 7 Integration plugin
3. Enter Studio ID and Secret Key from workspace.vsco.co/settings/api/new-lead
4. Configure form field mapping
5. Source field is required -- must match Workspace lead sources
6. Custom fields supported (format: CF-xxxxx)

### Gravity Forms:
1. Install Gravity Forms + VSCO Workspace Gravity Forms Integration plugin
2. Add Secret Key and Alias from Settings > API Integrations > Legacy New Lead API
3. Map form fields to Workspace fields
4. Mappable: FirstName, LastName, Email, phones, Source, EventDate, JobType, Message, custom fields

---

## Quo/OpenPhone (Text Messaging)

See `16-texting-sms.md` for full details.

---

## Gmail Integration

See `15-email-system.md` for full details.

---

## Google Calendar Integration

See `14-calendar.md` for full details.
