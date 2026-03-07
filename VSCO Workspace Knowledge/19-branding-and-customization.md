# VSCO Workspace - Branding and Customization

## Brand Settings

**Location:** Settings > Branding

### Brand Details:
- Brand Name, Email, Brand Website
- Secure Alias (unique Workspace URL identifier)
- Custom Domain (use your own domain for client-facing pages)
- Fallback URL (must contact VSCO to change; old links redirect properly)
- Location, Office Hours, Phone Numbers

### Logos and Images:
- **Printout Logo** -- Smaller logo in top right corner of orders and invoices
- **Email Logo** -- Optional; inserted at bottom of all outgoing emails
- **Page Background** -- Background behind your content
- All images are optional

### Colors:
- **Page Background** -- Background color of entire page
- **Box Background** -- Background color of content box
- **Error Text Color** -- Color for error messages
- **Printout Accent** -- Accent color for PDF printouts

### Footer:
- Appears at bottom of all Client Access pages
- Add contact details, terms of service, privacy policy links
- Customizable via Settings > Branding > Advanced Design > Page Footer HTML

---

## Multiple Brands

One of the biggest differentiators of Workspace.

- All accounts have one brand by default
- Additional brands added in minutes
- Run multiple brands from one account
- Each brand has different branding, reporting, and client-facing configuration
- Break down profit/loss, lead sources, and product sales by brand
- Example: Commercially branded booking link for corporate clients, softer wedding-branded quote for brides -- all from one account

---

## Custom Domain

- Set up a CNAME DNS record pointing to Workspace
- Client URLs won't change during platform updates
- VSCO notifies you when CNAME record changes are needed

---

## Custom Fonts

**Location:** Settings > Branding > Advanced Design Editor > Page CSS

### Using Google Fonts:
```css
@import url('https://fonts.googleapis.com/css2?family=family+name');
body {
  --headline-font: 'family name', sans-serif;
  --default-font: 'family name', sans-serif;
  --monospace-font: 'family name', monospace;
}
```

### Three Font Variables:
- `--headline-font` -- Headlines
- `--default-font` -- Body text
- `--monospace-font` -- Currencies, token output

### Notes:
- Does NOT affect emails and PDFs
- Custom fonts apply to all client access pages, including embedded contact forms
- Different fonts can be set for headlines, regular text, and monospace

---

## Advanced CSS Customization

- Available in the Page CSS section of the Advanced Design Editor
- At the bottom of branding settings
- Workspace's CSS is subject to change at any time
- Support team does not provide official CSS support -- changes at your own risk

---

## Admin-Only Access

Branding settings can only be modified by Administrator users. Standard users cannot access branding configuration.
