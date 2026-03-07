# VSCO Workspace - Contracts and Questionnaires

## Contracts

### Creating Contracts:
Contracts are typically created as part of the quote/booking process.

1. Choose from existing contract templates OR click New to create one
2. Fill in Contract Settings details
3. Write Contract Text
4. Tick "Save as Template" to reuse later

### Contract Features:
- **Tokens**: Personalize contracts using tokens (e.g., client name, job date, package details)
- **Payment schedule integration**: Include `{{payment_schedule.summary_list}}` to auto-insert payment terms
- **Initials boxes**: Add next to any place where the client should initial
- **Digital signatures**: Clients sign electronically
- **Custom fields**: Can be used in contracts

### Sending Contracts:
- As part of a quote (most common) -- included in the booking flow
- Independently using Contract Invitation email templates
- In advanced quotes, clients can sign one or more contracts during booking

---

## Questionnaires

**Location:** Settings > Questionnaires

### Menu Sections:
- **Responses** -- View submitted responses
- **Open Invitations** -- Track pending questionnaire invitations
- **Templates** -- Manage questionnaire templates
- **Public** -- Public questionnaires accessible without invitation

### Building a Questionnaire:
1. Create and name a form
2. Add fields (the questions)
3. Configure field types and visibility

### Field Types:
- **Layout Fields**: Don't collect data; provide instructions or info to clients
- **Basic Form Fields**: Standard data collection
- **Advanced Form Fields**: More complex data collection

### Field Visibility Settings:
- **Hidden**: Not shown to clients
- **Private**: Only you see in the Workspace account
- **Viewable**: Clients can see the field
- **Editable**: Clients can see AND edit responses (most common)

### Sending Questionnaires:
- Use Questionnaire Invitation email templates
- Template uses `{{item.name_link}}` token for the questionnaire link
- Can be included in quotes/booking process

### Public Questionnaires:
- Make any questionnaire public by checking "Public Form"
- Select which branding the form appears under
- Anyone with the link can fill it out without an invite
- Can be set to auto-create a lead in Workspace
- Can be embedded on websites using iframe code

### Embedding Public Questionnaires:
1. Select "Embed Questionnaire" next to the public questionnaire
2. Copy the iframe code from the dialog box
3. Paste into your website's HTML

### Integration with Quotes:
- Add questionnaires to quotes to collect information before contract signing
- In advanced quotes, clients fill out one or more questionnaires during booking
- Questionnaire responses can pre-fill contract fields

### Option: Show in Client Portal
- Configure whether the questionnaire appears in the client portal after initial submission
