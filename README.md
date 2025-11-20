# Audient Health Email Signatures

A collection of professional HTML email signatures for Audient Health team members.

## Overview

This repository contains HTML email signature templates designed for use across various email clients. Each signature includes:

- **Personal Information**: Name, job title, and company name
- **Contact Details**: Phone number, email address, website, and physical address
- **Branding**: Audient Health logo
- **Social Media**: LinkedIn and Twitter/X profile links
- **Legal Disclaimers**: Company registration details and confidentiality notices

## File Structure

```
Audient-Health-Email-Signatures/
├── README.md
├── signatures.html              # Template signature file
├── StefaniaRucci.html          # Individual signature example
├── audient_health_logo.png     # Company logo (full version)
└── email_audient_logo.png      # Company logo (email-optimised version)
```

## Features

- **Email Client Compatible**: Built using table-based HTML for maximum compatibility across email clients (Outlook, Gmail, Apple Mail, etc.)
- **Responsive Design**: Optimised for both desktop and mobile email clients
- **Brand Consistency**: Uses Audient Health brand colours (RGB: 248, 98, 149 / #F86295)
- **Accessibility**: Includes proper ARIA labels and semantic HTML
- **Legal Compliance**: Includes required legal disclaimers and opt-out information

## Usage

### For Individual Signatures

1. Open the desired signature HTML file in a text editor
2. Copy the entire HTML content
3. In your email client:
   - **Gmail**: Settings → General → Signature → Create new → Paste HTML
   - **Outlook**: File → Options → Mail → Signatures → New → Paste HTML
   - **Apple Mail**: Mail → Preferences → Signatures → + → Paste HTML
   - **Other clients**: Refer to your email client's documentation for adding HTML signatures

### Creating New Signatures

To create a new signature for a team member:

1. Copy an existing signature file (e.g., `StefaniaRucci.html`)
2. Rename it to match the person's name (e.g., `JohnSmith.html`)
3. Update the following fields:
   - Name (line 37)
   - Job title (line 47)
   - Phone number (line 179 and 185)
   - Email address (line 226 and 232)
   - Website URL (if different, line 273 and 279)
   - Social media links (lines 347 and 369)
   - Any other personal information

### Image Requirements

- Ensure `email_audient_logo.png` is accessible (either hosted online or embedded as base64)
- For best compatibility, host images on a reliable server or use base64 encoding
- Current logo references a local file: `email_audient_logo.png`

## Technical Details

### HTML Structure

The signatures use nested table layouts for maximum email client compatibility:

- Outer table: Main container
- Middle table: Content layout (name/title on left, logo on right)
- Inner tables: Contact information rows with icons

### Styling

- **Font**: Arial (fallback to system default)
- **Primary Colour**: RGB(248, 98, 149) / #F86295
- **Text Colour**: Black (RGB(0, 0, 0))
- **Font Sizes**:
  - Name: 18px
  - Title/Company: 14px
  - Contact info: 14px
  - Legal text: 10px

### External Dependencies

- Icons are loaded from HubSpot CDN (phone, email, website, address, social media icons)
- Logo should be hosted or embedded locally

## Customisation

### Changing Brand Colours

To update the brand colour throughout a signature, search and replace:

- `rgb(248, 98, 149)` or `#f60098` (appears in divider lines and icon backgrounds)

### Adding/Removing Contact Fields

Each contact field is a table row (`<tr>`) within the contact information section (starting around line 142). To add or remove fields:

1. Copy an existing contact row structure
2. Update the icon source, alt text, and link/content
3. Adjust spacing as needed

## Notes

- **Image Hosting**: For production use, consider hosting the logo on a CDN or company server rather than using local file paths
- **Testing**: Always test signatures in multiple email clients before deployment
- **Legal Text**: The legal disclaimers are specific to Audient Health Ltd. and should not be modified without legal review
- **Opt-Out**: The signature includes GDPR-compliant opt-out instructions

## Support

For questions or issues with email signatures, please contact the IT team or project maintainer.

## License

Internal use only - Audient Health Ltd.
