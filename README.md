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
├── logo/
│   └── email_audient_logo.png  # Company logo (email-optimised version)
└── icons/
    ├── phone-icon-dark-2x.webp
    ├── email-icon-dark-2x.webp
    ├── link-icon-dark-2x.webp
    ├── address-icon-dark-2x.webp
    ├── linkedin-icon-dark-2x.webp
    └── x-icon-dark-2x.webp
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

- All images (logo and icons) are hosted on GitHub using raw.githubusercontent.com
- Images are referenced using commit-specific URLs for version control:
  - Logo: `https://raw.githubusercontent.com/Direct-Design-Studio/Audient-Health-Email-Signatures/bb6b43ed5de045e458e6400acf3605c80ebf86d9/logo/email_audient_logo.png`
  - Icons: `https://raw.githubusercontent.com/Direct-Design-Studio/Audient-Health-Email-Signatures/bb6b43ed5de045e458e6400acf3605c80ebf86d9/icons/[icon-name].webp`
- Using commit-specific URLs ensures images remain stable even if the repository structure changes

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

- **Icons**: All icons (phone, email, website, address, LinkedIn, X/Twitter) are loaded from GitHub raw URLs:
  - Base URL: `https://raw.githubusercontent.com/Direct-Design-Studio/Audient-Health-Email-Signatures/bb6b43ed5de045e458e6400acf3605c80ebf86d9/icons/`
- **Logo**: Company logo is hosted on GitHub raw URLs:
  - URL: `https://raw.githubusercontent.com/Direct-Design-Studio/Audient-Health-Email-Signatures/bb6b43ed5de045e458e6400acf3605c80ebf86d9/logo/email_audient_logo.png`
- All images use commit-specific URLs to ensure stability and version control

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

- **Image Hosting**: All images (logo and icons) are hosted on GitHub using raw.githubusercontent.com with commit-specific URLs. This ensures images remain accessible and version-controlled. If you need to update images, commit the changes and update the commit hash in the signature HTML files.
- **Testing**: Always test signatures in multiple email clients before deployment
- **Legal Text**: The legal disclaimers are specific to Audient Health Ltd. and should not be modified without legal review
- **Opt-Out**: The signature includes GDPR-compliant opt-out instructions
- **Icon Updates**: When updating icons, ensure the new commit hash is updated in all signature files to maintain consistency

## Support

For questions or issues with email signatures, please contact the IT team or project maintainer.

## License

Internal use only - Audient Health Ltd.
