# Resume website

A plain HTML/CSS/JS portfolio. There's no build step, so open `index.html` in a browser to preview it.

```
index.html     the page
styles.css     colours, fonts, layout (tokens at the top)
script.js      theme toggle, mobile menu, scroll reveal, contact form
thanks.html    fallback "message sent" page
assets/        favicon, logos, your photo and résumé PDF
```

## Before you publish, replace these

1. **Résumé PDF**: save it as `assets/Paul_Muniu_Resume.pdf`.
2. **Photo** (optional): save it as `assets/portrait.jpg`. Then, in `index.html`, uncomment the `<img>` line in the portrait card and delete the `PM` monogram line.
3. **Third project card**: it's marked `PLACEHOLDER`. Put a real Power BI or Streamlit project there.
4. **Experience**: the two entries marked `PLACEHOLDER` need your real roles and education.
5. **LinkedIn**: put your profile URL in the Contact section.

## Publishing on Netlify

**Without GitHub (fastest):** go to https://app.netlify.com/drop and drag this whole folder onto the page.
The site is live in seconds. To update it later, drag the folder again.

**With GitHub (recommended):** push this folder to a new GitHub repo. In Netlify, choose
*Add new site → Import an existing project → GitHub*, then pick the repo. Leave the build command empty and set the publish directory to `/`.
From then on, every `git push` updates the site.

Rename the site under *Site configuration → Change site name* (e.g. `paul-muniu.netlify.app`).

## Contact form

The form uses Netlify Forms. Netlify detects it on deploy, and messages appear under
*Forms* in your Netlify dashboard. To get them by email, open *Forms → Form notifications* and add your address.
The form only works on the live Netlify site, not when you open the file locally.
