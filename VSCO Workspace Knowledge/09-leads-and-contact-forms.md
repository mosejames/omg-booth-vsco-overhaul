# VSCO Workspace - Leads and Contact Forms

## Creating Leads

### Manual Creation:
1. Go to the dashboard > New Lead
2. Enter job date (if established for the main shoot/event)
3. Enter name and email for at least one contact
4. Enter any other collected information

### Automatic Creation:
- Through a VSCO Workspace contact form embedded on your website
- Through a public questionnaire set to auto-create a lead
- Via Zapier integrations (e.g., Acuity Scheduling, Calendly)

---

## Lead Sources

**Location:** Settings > Lead Sources

- Pre-populated with common sources when starting your account
- Track where leads are coming from (Google, referral, Instagram, etc.)
- Must be customized to exactly match what appears on your contact forms
- If using WordPress plugins (Contact Form 7 or Gravity Forms), the source field is required and must exactly match Settings > Lead Sources
- Detailed analysis available in Booking Trends by Lead Source report

---

## Lead Status

Tracks where the lead is during the sales process.

### Customizable Statuses with Rules:
- Set rules on each status (e.g., auto-change after X days)
- Example: "Initial Contact" auto-changes to "Needs Follow Up" after 3 days if lead is still open
- Status changes trigger notifications via daily email and dashboard tile
- Status changes can trigger automations

---

## Contact Forms

**Location:** Settings > Contact Forms

### Creating a Form:
1. Go to Settings > Contact Forms > New Contact Form
2. Name your form
3. Set the direct URL
4. Give the page a title
5. Add an intro message
6. Configure the fields

### Field Configuration:
- Choose which fields are **Required, Optional, or Hidden**
- **Drag & drop** fields to reorder appearance
- Change **Labels** to control wording of questions
- Common fields: FirstName, LastName, Email, HomePhone, MobilePhone, WorkPhone, Source, EventDate, JobType, Message

### Adding Custom Fields:
- Create custom fields in Settings > Custom Fields
- Multiple field types available
- Custom field data appears in new lead email notifications and on the lead's worksheet
- Custom fields can be selected as fields on the Contact Form

---

## Embedding Forms on Your Website

### General iFrame Method:
1. After creating your form, select "Embed Form" next to it
2. Copy the iFrame code from the dialog box
3. Access the HTML source code of your website page
4. Paste the iframe code where you want the form

**Redirect Configuration:** If redirecting after submission, add a script to Settings > Branding > Advanced Design > Page Footer HTML so the redirect doesn't happen inside the iFrame.

### Squarespace:
- Insert a **Code Block** on your contact page
- Paste the iFrame embed code

### WordPress (Three Methods):

1. **iFrame Method**: Simplest. Embed via iFrame code. If theme doesn't support iFrame, use the Advanced iFrame plugin.

2. **Contact Form 7 Integration**:
   - Install Contact Form 7 plugin
   - Install VSCO Workspace Contact Form 7 Integration plugin
   - Enter Studio ID and Secret Key from workspace.vsco.co/settings/api/new-lead
   - Map form fields to Workspace fields
   - Source field is required

3. **Gravity Forms Integration**:
   - Install Gravity Forms + VSCO Workspace Gravity Forms Integration plugin
   - Add Secret Key and Alias from Settings > API Integrations > Legacy New Lead API
   - Map form fields to Workspace fields

### Embeddable Items:
- Contact forms
- Public questionnaires (via Embed Questionnaire option)
- Bookable events (via Scheduling > Bookable Events > Actions > Embeddable Link)

---

## Auto-Responding to New Leads

### Setup:
- Create automation observing Lead > Created, executing immediately
- Add condition: "if web lead" (not manually created)
- Optionally filter by job type
- Add action: Send email using template

### Templates Available:
- Standard auto-response
- Out-of-office auto response
- Auto-send quote upon new lead creation
- Available in the Template Gallery
