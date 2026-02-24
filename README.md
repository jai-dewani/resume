# Resume
A repository containing my latex file with github-actions set to create a PDF and push it to `gh-pages` branch which is then hosted so I can easily update my information in latex, push the changes and expect my updates to be reflected in the hosted version of this repo with no hassle.  
You can check it out here [jai-dewani.github.io/resume](https://jai-dewani.github.io/resume/)

## 📊 Analytics & Tracking

This resume now includes comprehensive tracking capabilities to help you understand who's viewing your resume and from where.

### Features
- **View Tracking**: Monitor every resume view with Google Analytics
- **Source Attribution**: See where traffic comes from (LinkedIn, email, networking, etc.)
- **Custom Link Generation**: Create trackable links for specific companies/recruiters
- **Engagement Metrics**: Track how long people spend viewing your resume
- **Geographic Insights**: See where your resume is being viewed globally

### Quick Start
1. **Set up Google Analytics**: Follow the guide in `TRACKING_SETUP.md`
2. **Generate Custom Links**: Use `.\link-generator.html` to create trackable URLs
3. **Monitor Analytics**: Check your Google Analytics dashboard for insights

### Example Trackable Links
```
# For job applications
https://jai-dewani.github.io/resume/?source=linkedin&medium=application&campaign=senior_sde&id=google_application

# For networking
https://jai-dewani.github.io/resume/?source=networking&medium=business_card&campaign=tech_conference_2026&id=contact_john_doe

# For recruiter outreach
https://jai-dewani.github.io/resume/?source=email&medium=recruiter&campaign=q1_2026&id=recruiter_jane_smith
```

### Special mention 
- Thanks to [@ronaksakhuja](https://github.com/ronaksakhuja) and [@rajivnayanc](https://github.com/rajivnayanc) for sharing their [@ronaksakhuja/resume](https://github.com/ronaksakhuja/resume)  and &lt;private&gt; repositories for giving me an idea, how I can create an action for compiling the latex file to generate the PDF on the fly on every update (makes my life so easy) 

- [@imabp](https://github.com/imabp/) gave me the idea to make this a template repository, check out his [version](https://github.com/imabp/resume)

- Thanks to [@harshkapadia2](https://github.com/harshkapadia2/) for sharing his [@harshkapadia2/resume](https://github.com/harshkapadia2/resume) repository and giving me some ideas on how I can improve my action file and also pointing out that [@himanshusharma89](https://github.com/himanshusharma89/) is using some sort of method to embed his PDF in the HTML view so the mobile users don't need to download the file just for viewing. CHeckout this repo here [@himanshusharma89/resume](https://github.com/himanshusharma89/resume/)
