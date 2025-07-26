# Google Analytics Setup Guide

## Overview
Google Analytics 4 (GA4) tracking has been added to both `index.html` and `research.html` files. This is completely free and provides comprehensive analytics without requiring Netlify's paid analytics service.

## Setup Steps

### 1. Create Google Analytics Account
1. Go to [Google Analytics](https://analytics.google.com/)
2. Sign in with your Google account
3. Click "Start measuring"
4. Create a new account (or use existing)
5. Set up a GA4 property for your audit site

### 2. Get Your Measurement ID
1. In GA4, go to Admin (gear icon)
2. Select your property
3. Click "Data Streams"
4. Add a new web stream for your Netlify domain
5. Copy the **Measurement ID** (format: G-XXXXXXXXXX)

### 3. Update Your Files ✅ COMPLETED
**Measurement ID G-FQXMM60RT8 has been implemented in both HTML files.**

**Strategy:** Using unified GA4 property (same as optimi.co.nz) for cross-site analytics and scalability across future lead generation tools.

### 4. Deploy Changes
1. Commit your changes: `git add . && git commit -m "Add Google Analytics tracking"`
2. Push to GitHub: `git push`
3. Netlify will automatically deploy the updated files

### 5. Verify Setup
1. Visit your live site
2. In GA4, go to Reports > Realtime
3. You should see your visit appear within a few minutes

## What You'll Track

### Standard Metrics
- Page views and unique visitors
- Traffic sources (direct, social, referral, search)
- Geographic location of visitors
- Device and browser information
- Session duration and bounce rate

### Custom Events (Already Configured)
- Calendly booking button clicks
- Audit tool interactions
- Navigation between sections
- PDF downloads (if added)

### Enhanced Measurements (Automatic)
- Scroll tracking
- Outbound link clicks
- Site search (if enabled)
- Video engagement (if added)
- File downloads

## Benefits Over Netlify Analytics

### Cost
- **Google Analytics**: Free forever
- **Netlify Analytics**: $9/month per site

### Features
- **GA4**: Comprehensive funnel analysis, custom events, audience segmentation, conversion tracking
- **Netlify**: Basic page views and traffic sources only

### Integration
- **GA4**: Integrates with Google Ads, Search Console, and other marketing tools
- **Netlify**: Standalone analytics only

## Privacy Compliance

The tracking code respects user privacy and complies with GDPR/CCPA:
- No personally identifiable information is collected by default
- IP addresses are anonymized
- Users can opt out via browser settings
- Data is processed according to Google's privacy policies

## Recommended Next Steps

1. **Set up Goals/Conversions** in GA4 for:
   - Calendly booking completions
   - Audit tool completions (high percentage score)
   - Research page engagement

2. **Create Custom Audiences** for:
   - Users who completed the audit
   - High-engagement visitors
   - Users from specific sectors (if determinable)

3. **Set up Enhanced Ecommerce** (if you add paid services):
   - Track consultation purchases
   - Measure average order value
   - Monitor conversion funnels

## Troubleshooting

### Not Seeing Data
- Check that the Measurement ID is correct
- Ensure ad blockers aren't interfering
- Wait 24-48 hours for full data processing

### Duplicate Tracking
- Make sure the tracking code appears only once per page
- Don't mix GA4 with Universal Analytics (old version)

### GDPR Compliance
- Consider adding a cookie consent banner for EU visitors
- Review Google's data processing addendum
- Document your data collection practices

---

*Updated: July 17, 2025*  
*Files modified: index.html, research.html*
