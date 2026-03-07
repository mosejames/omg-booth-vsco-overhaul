# VSCO Workspace - Job Types, Job Roles, and Event Types

## Job Types

**Location:** Settings > Job Types

Job Types define the categories of services you offer (e.g., weddings, headshots, commercial, photo booth, family sessions).

### Three Main Components of a Job Type:
1. **Workflow** -- The tasks auto-assigned to jobs of this type
2. **Job Roles** -- The default contacts for jobs of this type
3. **Event Types** -- The default events for jobs of this type

### Configuration:
- Give the job type a name
- Select the workflow and profit center
- Set an initial lead status (which status new leads of this type receive by default)
- Check which custom fields should be available for jobs of that type
- Reorder custom fields to control their appearance on the job worksheet
- Once set up, defaults apply any time a new lead or job of that type is created

### Prerequisites:
Set up these first:
- Workflows (Settings > Workflow)
- Job Roles (Settings > Job Roles)
- Event Types (Settings > Event Types)

---

## Job Roles

**Location:** Settings > Job Roles

Job Roles represent the people involved in a job -- you, your team, and your clients.

### Setting Up Job Roles on Job Types:
- Select from existing roles or create a new one (saved to Settings > Job Roles)
- Setting default contacts creates placeholders when adding a new lead/booking
- You must mark which job roles are the "clients" on the job type

### Example Wedding Job Roles:
- Primary Contact (client)
- Secondary Contact (client)
- Venue Contact
- Florist
- DJ
- Catering
- Other vendor contacts

### Referral Tracking via Job Roles:
- Create a "Referral" job role
- Tie a person to a job as a referral
- Track all booked jobs they've referred from their contact card's Leads & Jobs tab

---

## Event Types

**Location:** Settings > Event Types

Three base categories (observable in automations):
1. **Call** -- Phone calls, discovery calls
2. **Meeting** -- In-person or virtual meetings
3. **Session** -- Photo/video sessions, shoots

Custom event types extend these (e.g., Wedding, Engagement Session, Ordering Session).

### Setting Default Event Types on Job Types:
- Select which events should be auto-created on new jobs of that type
- Example: A Wedding job type might have Wedding Session, Engagement Session, and Pre-Wedding Meeting as defaults

---

## Event Channels

Each event can have a channel:

- **In Person** -- Set location via Google Maps lookup or custom address
- **Over the Phone** -- Set call-in number (defaults when selecting Call type)
- **Virtually** -- Set custom URL, or auto-generate Google Meet link (if Google Calendar integrated)

### Event Channel Tokens:
- `{{channel}}` -- The channel type
- `{{channel_details}}` -- Full channel details
- `{{virtual_url}}` -- Virtual meeting URL
- `{{phone_number}}` -- Call-in phone number

Use these in email templates and automations (e.g., meeting reminder emails).
