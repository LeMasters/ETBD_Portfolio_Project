> **Caveat lector:** Mostly written by Claude AI.

# Your Portfolio, Search Engines and AI

A guide for students using the Alexander portfolio template · 19 Nov 2026 · Garrison LeMasters

## The short version

Your portfolio site is built to be found by search engines and to ask AI companies not to train on your work. You can leave both as they are. Two things are up to you:

1. **Whether to allow AI training.** Off by default. One switch in the Analytics form turns it on.
2. **Your site's address.** It works either way, but the address affects how much the AI opt-out can do (section 5).

What no setting can do for you: make people find your site, or force any company to respect your wishes. The first depends on what you write and where you link to your site; the second depends on the law and on each company's choices.

## Who owns your work

You do. In the U.S., copyright belongs to you the moment your work exists, with no form to file. Miami's [intellectual property policy](https://codes.ohio.gov/ohio-administrative-code/rule-3339-15-06) recognises students' ownership of their own writing, art, programs and other works.

- **The © line.** Your site's footer shows "© year Your Name". It isn't required by law, but it tells visitors you claim your work, and it can make it harder for someone who copies it to argue they didn't know ([U.S. Copyright Office, Circular 3](https://copyright.gov/circs/circ03.pdf)).
- **Registration** with the Copyright Office is optional. It's needed before you could sue someone in the U.S. over your work. Most students never need it.

Be careful with work that isn't only yours:

- **Team projects.** Teammates may own the work jointly with you. Name your role and credit the team on the project page.
- **Client or sponsored projects.** You may have signed an agreement that gives the work to the client or limits what you can show. Check before you post.
- **Assets you didn't make.** Asset-store art, music, sound effects, fonts and code libraries belong to their makers. Credit them in the project description, and follow their licences.

This guide is general information, not legal advice. For questions about a specific project, ask your instructor or Miami's Office of General Counsel.

## Being found in search

The site already does the technical part of search-engine optimisation (SEO); what decides whether people find you is what you write and where you link to it.

| The site does this for you | Only you can do this |
| --- | --- |
| Page titles built from your name, area of expertise and project titles | Write an area of expertise people would actually search for ("3D environment artist", "systems designer") |
| A short description of every page, from your expertise line and captions | Give every project a clear title and a one-line caption |
| A sitemap listing your pages, so search engines don't miss any | Fill in **Alt text** for every image: search engines read it, and so do people using screen readers |
| Structured data telling search engines this is a person's portfolio and each project is a creative work by you | Link to your portfolio from LinkedIn, itch.io, ArtStation, GitHub, your résumé and email signature |
| Fast pages, sized images and proper headings, which search engines favour | Use the same name everywhere, so search engines connect your profiles |

**Optional: Google Search Console.** This free Google tool shows whether Google has found your site and which searches lead to it.

1. Sign in at [search.google.com/search-console](https://search.google.com/search-console) and add a **URL prefix** property with your site's full address.
2. Choose the **HTML tag** method and copy the code inside `content="…"`.
3. Paste it into **Google Search Console code** in the Analytics form and save.
4. Wait for the site to rebuild (a minute or two), then click **Verify**.

Search engines take days or weeks to list a new site. Nothing here can make a site rank first; links from places people already visit matter most.

## AI: training versus search

By default your site asks AI companies not to train their models on it, while still letting search tools, including AI search, find and link to you. These are two different uses:

- **AI training.** A company copies pages and images in bulk to teach a model. Your work becomes part of what the model learned. You get no credit, link or visit.
- **AI search and answers.** A tool such as ChatGPT search, Claude or Perplexity looks up pages to answer a question and usually links to its sources. This can send people to your site.

Your site uses several signals, because no single one is read by every company:

| Signal | Where it is | What it says | Works if your site is in a subfolder? |
| --- | --- | --- | --- |
| `tdm-reservation` tag | Every page | You reserve text-and-data-mining rights. Under EU copyright law this is the recognised opt-out ([W3C TDMRep](https://www.w3.org/community/reports/tdmrep/CG-FINAL-tdmrep-20240510/)). | Yes |
| `noai, noimageai` tags | Every page | Please don't use this page or its images for AI. Informal; some dataset builders honour it. | Yes |
| `robots.txt` crawler list | One file | Named AI-training crawlers (OpenAI's GPTBot, Anthropic's ClaudeBot, Google-Extended, Apple, Meta, Common Crawl and others) may not collect the site. Search crawlers may. | No (see section 5) |
| `Content-Usage` and `Content-Signal` lines | Same file | The same wish in two newer formats: an IETF draft standard and Cloudflare's policy. | No |

**What these signals can't do:**

- **They are requests.** Reputable companies say they follow them. A company that ignores them isn't stopped by anything on your site.
- **They aren't retroactive.** Work collected before you published it, or before a company adopted a signal, isn't removed.
- **Page tags cover pages, not files.** An image opened directly by its address carries no tag.
- **Opting out of Google's AI training doesn't affect Google Search.** Blocking the Google-Extended token leaves your site in Google's search results.

## Your two choices

Neither choice has a right answer; each trades one thing for another.

### 1. Allow AI training, or not

Set in **Analytics → Allow AI companies to train on this site**. Off unless you turn it on; you can change it at any time.

|  | Off (the default) | On |
| --- | --- | --- |
| What your site asks | Don't train AI models on my work | No objection to AI training |
| Search and AI search | Unaffected: you can still be found and linked | Unaffected |
| Who it suits | Most people, especially if your images, writing or style are what you are showing | People who want their work as widely absorbed as possible, or who don't mind |

### 2. Your site's address

Your address depends on what you name your GitHub repository. Decide early: changing it later changes the address, and links you have shared stop working.

|  | `username.github.io/portfolio` | `username.github.io` | Your own domain (e.g. `jordanlee.com`) |
| --- | --- | --- | --- |
| How | Any repository name (here, "portfolio") | Name the repository exactly `username.github.io` | Buy a domain and connect it in the repository's settings |
| Cost | Free | Free | About $12–20 a year, every year |
| `robots.txt` (the crawler list) | Not read: crawlers only look at the top of an address | Read | Read |
| Page tags | Work | Work | Work |
| Look on a résumé | Fine | Cleaner | Cleanest; yours even if you leave GitHub |
| Catch | — | Only one such site per GitHub account | If you stop paying, the address lapses and someone else can buy it |

Your GitHub username is part of the first two addresses, so pick one you'd be comfortable showing an employer.

## What no setting can do

Anything on a public website can be copied by a person or a program that ignores the rules. A few habits limit what can be taken and help if it is.

- **Your repository is public, originals included.** The site shows resized copies of your images, but the files you upload sit in your GitHub repository, which anyone can browse. If an image is valuable at full size, upload a smaller version (for example 1800 px on the long side) and keep the original yourself.
- **Show work, not source.** Link to playable builds on itch.io or Steam rather than uploading them, and keep project files, source art and code you don't want reused out of the repository.
- **Watermarks are a trade-off.** A small name or address on an image discourages casual reuse but can distract reviewers. Many portfolios skip them.
- **Keep proof of authorship.** Dated working files, version history and process images show the work is yours if it's ever disputed.
- **If someone copies your work:** contact them first. If that fails, the site hosting the copy usually has a copyright takedown form (in the U.S., a DMCA notice). Your instructor or Miami's Office of General Counsel can advise.
- **If you used AI tools in a project,** say how in its description. Many employers and courses expect it, and it avoids questions later.

## Checklist before you share your site

- [ ] My area of expertise says what I do, in words people would search for
- [ ] Every project has a clear title and a one-line caption
- [ ] Every image has alt text
- [ ] Team projects name my role and credit my teammates
- [ ] Client or sponsored work is cleared for posting
- [ ] Assets I didn't make are credited, and their licences allow this use
- [ ] Images I want to protect are uploaded at web size, not full resolution
- [ ] I've decided on AI training (Analytics form) and my site's address
- [ ] My portfolio is linked from LinkedIn, itch.io and my résumé
- [ ] (Optional) I've added the site to Google Search Console

## Glossary and help

| Term | Meaning |
| --- | --- |
| Crawler | A program that visits websites automatically, for a search engine or an AI company |
| `robots.txt` | A file at the top of a web address telling crawlers what they may visit |
| SEO | Search-engine optimisation: making a site easy for search engines to understand and list |
| Sitemap | A file listing a site's pages for search engines |
| Structured data | Hidden labels in a page that tell search engines what it is about (a person, a creative work) |
| TDM | Text and data mining: analysing large amounts of content by computer, including to train AI |
| AI training | Copying content in bulk to teach an AI model |
| AI search | An AI tool looking up pages to answer a question, usually with links to its sources |

**Help.** Questions about your site: your instructor. Questions about who owns a particular project: your instructor or Miami's Office of General Counsel.

**Sources:** [U.S. Copyright Office, Circular 3: Copyright Notice](https://copyright.gov/circs/circ03.pdf) · [Miami University intellectual property policy (Ohio Admin. Code 3339-15-06)](https://codes.ohio.gov/ohio-administrative-code/rule-3339-15-06) · [W3C TDM Reservation Protocol](https://www.w3.org/community/reports/tdmrep/CG-FINAL-tdmrep-20240510/) · [Google: how to write a robots.txt file](https://developers.google.com/crawling/docs/robots-txt/create-robots-txt) · [IETF AI Preferences draft (Content-Usage)](https://datatracker.ietf.org/doc/draft-ietf-aipref-attach/)
