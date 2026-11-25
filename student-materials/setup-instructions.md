# Your Portfolio Site: Setup Instructions

21 Nov 2026 · Garrison LeMasters

## Overview

You will end up with a portfolio site built on Alexander, the department's template, at `https://<your-username>.github.io/<repository-name>/`, edited entirely through web forms: no code, nothing to install. Setup takes about 30 minutes; your content takes as long as your content takes.

| Tool | What it does for you |
| --- | --- |
| GitHub | Stores your site's files and publishes the site. Free. |
| Pages CMS | The forms you use to change text and upload images. Free. |
| Alexander (the class template) | The design. You make your own copy of it in Part 1. |

Each time you save a form, GitHub rebuilds your site. Changes appear one to two minutes later.

Before you start, read the companion page, **Portfolio Site: Best Practices**, for photo sizes and writing advice.

## Part 1: Get your copy of Alexander

1. **Make a GitHub account** at github.com, if you don't have one, and verify your email. Choose the username with care: it appears in your site's address. A plain form of your name works best.
2. **Open the Alexander template:** [template link from your instructor]. Click **Use this template → Create a new repository**.
3. **Name the repository**, for example `portfolio`. Leave it **Public**. Click **Create repository**.
4. **Turn on publishing.** In your new repository: **Settings → Pages**. Under **Build and deployment → Source**, choose **GitHub Actions**.
   - GitHub then suggests starter workflows (Jekyll, Static HTML). Ignore them: your copy already has its own.
5. **Run the first build.** Open the **Actions** tab. The first run, "Publish site", has probably failed, because publishing wasn't on yet. That is expected. Open the run and click **Re-run all jobs**.
   - No run listed? Click **Publish site** on the left, then **Run workflow**.
   - Wait until both stages, **build** and **deploy**, show green check marks (about a minute).
6. **Visit your site** at `https://<your-username>.github.io/portfolio/`. The address also appears under **Settings → Pages**. You will see Alexander's sample content; Part 3 replaces it.

## Part 2: Connect Pages CMS

1. Go to **app.pagescms.org** and click **Sign in with GitHub**. Approve the request.
2. **Give Pages CMS access to your repository.** When asked to install the Pages CMS app, choose your account, select **Only select repositories**, pick your portfolio repository, and click **Install**.
3. Back in Pages CMS, **open your repository**. Use the existing repository; do not use "Create from template" (that makes a different, unrelated site).
4. The forms appear on the left: **Profile, Selected Work, Gallery, Experience, Education, Tools, Appearance, Analytics**.

### If your repository isn't listed in Pages CMS

Pages CMS hasn't been given access to it yet. Fix it on GitHub:

1. **Open the installed-apps page:** go to **github.com/settings/installations** while signed in. (The long way: your profile picture, top right → **Settings** → **Applications** in the left sidebar, under "Integrations" → the **Installed GitHub Apps** tab.)
2. **Find Pages CMS** in the list and click **Configure** beside it.
3. **Scroll down to "Repository access."** It should be set to **Only select repositories**.
4. **Add your repository:** click **Select repositories**, type its name, and click it in the dropdown.
5. **Click Save.** GitHub may ask for your password or a security code first.

Then reload app.pagescms.org: your repository should now be in the list.

## Part 3: Fill in the forms

Work through the forms in this order, and **delete every sample entry you don't replace**: anything left over appears on your site under your name. A form left empty makes its section disappear from the page.

| Form | What goes in | Watch for |
| --- | --- | --- |
| Profile | Name, area of expertise, your About paragraph, email, LinkedIn and GitHub addresses, other links, résumé PDF | Your name and area of expertise sit at the top of every page. Leave About, LinkedIn or GitHub empty to hide them. |
| Selected Work | One entry per piece of work: title, kind (case study, project or brief, shown as a label before the title), caption, description, image, alt text, year, role, links, tags, sections, order | Order 1 comes first. Case study = a long page, told as a story; brief = one line on the home page. Sections add pictures beside text, swapping sides on each row. |
| Gallery | One entry per image: title, image, Show on home page, alt text, order, caption | Tick Show on home page for the images you want there; with none ticked, the first five appear. |
| Experience | One entry per job, internship or assistantship: role, organization, website, location, dates, order, what you did, related work | Order 1 comes first, usually the most recent. Lead with a verb: "Designed", "Ran", "Built". |
| Education | Degree, school, year, order, optional detail | Order 1 comes first. |
| Tools | The software, languages and media you use: choose each from the Tool list (shown with its logo, or a plain icon), or type it under Other tool if it isn't listed; each with an optional note that stays general ("C#; three years"), never about one project | Say where you used it, e.g. "C#; three years". |
| Appearance | Colour scheme, typeface for text, typeface for titles | Try each choice and look at the result. |
| Analytics | Visitor statistics (optional), whether AI companies may train on your site, a Google Search Console code (optional) | AI training stays refused unless you switch it on. See the README for setting up statistics. |

To add an image, click the image field and upload from your computer. Alexander makes smaller copies for phones itself; for sizes, see **Best Practices**.

Click **Save** after each form. Each save starts a rebuild.

Two habits that save work:

- **Check every Order number before you save.** If you scroll while the cursor is still in an Order box, the scroll wheel changes the number (1 can become 0). Click somewhere else on the page before scrolling.
- **Upload one image at a time.** Wait for its thumbnail to appear before uploading the next. Several uploads in quick succession can lose some of them; if a thumbnail is missing, upload that image again.

## Part 4: Publish, check, update

- **After each save**, the site updates in one to two minutes. You can watch progress in your repository's **Actions** tab. Several quick saves leave some runs marked "cancelled": that is normal, and only the latest run matters.
- **Page looks unchanged?** Your browser may be showing a saved copy for up to 10 minutes. Reload while holding Shift (Mac: Cmd-Shift-R; Windows: Ctrl-Shift-R).
- **Check it as a reviewer would:**
  - [ ] On your phone, scrolled all the way down
  - [ ] Every link clicked: email, LinkedIn, GitHub, project links, résumé
  - [ ] No sample content left anywhere
  - [ ] Your name and the browser-tab title are right
  - [ ] The preview looks right when you paste your address into a message to yourself
- **Updating later** works the same way: open Pages CMS, edit, save. The site lives in your own GitHub account and stays yours after the class.

## Troubleshooting

| What you see | Likely cause | What to do |
| --- | --- | --- |
| Red X in Actions at the "configure-pages" step | Publishing not turned on | Part 1, step 4; then re-run |
| Run stuck at "Queued" for many minutes | GitHub is having an outage | Check githubstatus.com and wait; saving again won't help |
| Your repository isn't listed in Pages CMS | Pages CMS lacks access | Follow steps 1–5 in Part 2, "If your repository isn't listed" |
| A form or field described here is missing in Pages CMS | Pages CMS is showing the forms it loaded earlier | Reload app.pagescms.org |
| Your site's address shows a "404" page, though the run is green | Wrong capital letters in the repository part of the address (it is case-sensitive) | Copy the address from Settings → Pages |
| Saved, run is green, page unchanged | Browser showing a saved copy | Shift-reload, or wait 10 minutes |
| A yellow "Analytics:" warning on a run in Actions | The statistics code in the Analytics form wasn't recognised | Paste the code again; your site publishes without statistics meanwhile |
| A photo looks soft | The original is smaller than the recommended size | See **Best Practices**, Photos |
| Someone else's name or projects still showing | Sample entries left in a form | Delete them in each form and save |
| Page shows plain text with no design | A setup problem in your copy | Ask your instructor; send your site's address |
