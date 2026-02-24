# Resume Tracking Setup Guide

## Setup Instructions

### 1. Get Google Analytics 4 Measurement ID
1. Go to [Google Analytics](https://analytics.google.com/)
2. Create a new GA4 property for your resume website
3. Copy your Measurement ID (format: `G-XXXXXXXXXX`)
4. Replace `GA_MEASUREMENT_ID` in `index.html` with your actual ID

### 2. Enable Enhanced Tracking
The implementation automatically tracks:
- **Page Views**: Every time someone visits your resume
- **Traffic Sources**: Where visitors came from (Google, LinkedIn, direct, etc.)
- **Time on Page**: How long people spend viewing your resume
- **Geographic Data**: Where your visitors are located
- **Device Information**: Mobile vs desktop usage

## Custom Link Tracking

### Creating Trackable Links for Specific Users

You can create custom links with tracking parameters:

**Basic Format:**
```
https://jai-dewani.github.io/resume/?source=SOURCE&medium=MEDIUM&campaign=CAMPAIGN&id=USER_ID
```

**Examples:**

1. **For LinkedIn applications:**
   ```
   https://jai-dewani.github.io/resume/?source=linkedin&medium=application&campaign=job_search&id=company_abc
   ```

2. **For specific recruiters:**
   ```
   https://jai-dewani.github.io/resume/?source=email&medium=recruiter&campaign=direct_outreach&id=recruiter_jane_doe
   ```

3. **For networking events:**
   ```
   https://jai-dewani.github.io/resume/?source=networking&medium=business_card&campaign=tech_conference_2026&id=contact_001
   ```

4. **For job applications:**
   ```
   https://jai-dewani.github.io/resume/?source=job_portal&medium=application&campaign=senior_sde_roles&id=zeiss_application
   ```

### URL Parameters Explained

- **source**: Where the traffic comes from (linkedin, email, networking, etc.)
- **medium**: The marketing medium (application, recruiter, business_card, etc.)
- **campaign**: The campaign name (job_search, direct_outreach, etc.)
- **id**: Unique identifier for tracking specific users/companies

## What You Can Track

### 1. **Basic Metrics**
- Total page views
- Unique visitors
- Traffic sources and referrers
- Geographic location of visitors
- Device/browser information

### 2. **Engagement Metrics**
- Time spent on resume page
- Bounce rate
- Return visitors

### 3. **Custom Events**
- `resume_view`: When someone views your resume
- `pdf_load`: When the PDF loads successfully
- `engagement_10s`: Users who spend 10+ seconds
- `engagement_30s`: Users who spend 30+ seconds
- `session_duration`: Total time spent on page

### 4. **Custom User Tracking**
- Track clicks from specific companies/recruiters
- Monitor which campaigns are most effective
- See if specific people you sent links to have viewed your resume

## Viewing Your Analytics

### Google Analytics 4 Dashboard
1. Go to [Google Analytics](https://analytics.google.com/)
2. Select your property
3. Key reports to check:
   - **Reports > Engagement > Pages and screens**: See page views
   - **Reports > Acquisition > Traffic acquisition**: See traffic sources
   - **Reports > Engagement > Events**: See custom events
   - **Explore**: Create custom reports

### Custom Reports You Can Create

1. **Recruiter Tracking Report**
   - Filter by `custom_user_id` parameter
   - See which specific recruiters have viewed your resume

2. **Campaign Performance**
   - Group by `campaign` parameter
   - Compare effectiveness of different outreach methods

3. **Geographic Analysis**
   - See which cities/countries your resume is being viewed from
   - Useful for relocation planning

## Privacy Considerations

- Google Analytics is GDPR compliant
- No personal data is collected beyond standard web analytics
- Users can opt-out via browser settings
- Consider adding a privacy notice if required in your jurisdiction

## Advanced Features You Can Add

### 1. **Real-time Notifications**
Set up Google Analytics alerts to get notified when:
- Someone views your resume
- Traffic spikes occur
- Specific custom IDs are tracked

### 2. **Integration with Google Sheets**
- Export data automatically to Google Sheets
- Create custom dashboards
- Track application success rates

### 3. **A/B Testing**
- Test different resume versions
- Track which performs better
- Optimize for better engagement

## Cost Breakdown

**Current Setup: FREE**
- Google Analytics 4: Free up to 10M events/month
- GitHub Pages hosting: Free
- No additional infrastructure costs

**Optional Paid Upgrades:**
- Google Analytics 360: $150k+/year (enterprise only)
- Custom domain: $10-15/year
- Additional analytics tools: $9-50/month

## Troubleshooting

### If tracking isn't working:
1. Check that you've replaced `GA_MEASUREMENT_ID` with your actual ID
2. Verify the property is set up correctly in Google Analytics
3. Check browser console for JavaScript errors
4. Ensure ad blockers aren't blocking Google Analytics

### Testing Your Setup:
1. Visit your resume with custom parameters
2. Check Google Analytics Real-time reports
3. Verify events are being recorded

## Next Steps

1. Set up Google Analytics property
2. Replace the measurement ID in `index.html`
3. Deploy to GitHub Pages
4. Test with custom tracking URLs
5. Monitor your analytics dashboard
6. Create custom links for different applications/outreach