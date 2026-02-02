# Tether Legal Documents

This folder contains the legal documents for the Tether app.

## Documents

- [Privacy Policy](privacy-policy.md)
- [Terms of Service](terms-of-service.md)
- [Health Disclaimer](health-disclaimer.md)

## Hosting on GitHub Pages

These documents are designed to be hosted on GitHub Pages. To set up:

1. Create a new GitHub repository (e.g., `threshold-legal` or use the main app repo)
2. Push this `legal/` folder to the repository
3. Go to Settings → Pages → Enable GitHub Pages from `main` branch
4. Your documents will be available at:
   - `https://[username].github.io/[repo]/privacy-policy`
   - `https://[username].github.io/[repo]/terms-of-service`
   - `https://[username].github.io/[repo]/health-disclaimer`

## Before Publishing

Replace all instances of:
- `PLACEHOLDER` → Your business/developer name
- `PLACEHOLDER@EMAIL.COM` → Your contact email

## Files to Update After Hosting

Update the URLs in `app/mission-control.tsx`:
```typescript
const PLACEHOLDER_URLS = {
    privacy: 'https://[username].github.io/[repo]/privacy-policy',
    terms: 'https://[username].github.io/[repo]/terms-of-service',
    contact: 'mailto:your-real-email@example.com',
    rateApp: 'https://apps.apple.com/app/threshold',
};
```
