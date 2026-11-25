> **Caveat lector:** Mostly written by Claude AI.

# How to Set Up Your Own Domain Name

19 Nov 2026 · Garrison LeMasters

## Before you start

Your own domain moves your portfolio from `your-username.github.io/portfolio/` to an address like `janedoe.com`. It takes about 30 minutes of work, plus some waiting, and costs about $11 a year for a .com ([Cloudflare's price as of October 2026](https://costgoat.com/compare/domains)).

What it gets you:

- **An address that is yours.** If you ever move your site away from GitHub, the address, your links and your search ranking come with you.
- **Full search and AI-crawler settings.** Your site's `robots.txt` file only works at the top of an address, so your AI-training opt-out and sitemap start working fully.
- **A cleaner line on your résumé and business card.**

You need:

- Your Alexander portfolio already published on GitHub Pages.
- A debit or credit card (or PayPal) for the domain.
- Your GitHub username and the name of your portfolio repository.

In the steps below, replace `janedoe.com` with your domain, `your-username` with your GitHub username, and `portfolio` with your repository's name.

## Step 1: Buy your domain on Cloudflare

Cloudflare sells domains at cost, with no markup, and the renewal price is the same as the first year.

1. Go to [dash.cloudflare.com/sign-up](https://dash.cloudflare.com/sign-up) and create a free account.
2. Open the email Cloudflare sends you and verify your address. You can't buy a domain until you do.
3. In the Cloudflare dashboard, open **Domain Registration → Register domains** (in the left sidebar).
4. Type the name you want, such as `janedoe`, and select **Search**. Pick an available name and select **Purchase**.
5. Fill in your contact details. The law requires real details; Cloudflare hides them from public lookups.
6. Add your card or PayPal and complete the purchase.
7. Open **Domain Registration → Manage domains**, select your domain, and check that **Auto-renew** is on.

Choosing a name: your own name is best (`janedoe.com`, `jane-doe.com`). Short, no numbers, easy to say aloud. A .com is the most familiar ending.

Cloudflare now manages your domain's settings (its "DNS"). That is where you'll do Steps 2 and 3.

## Step 2: Prove to GitHub that the domain is yours

This stops anyone else attaching your domain to their own GitHub site. You'll need two browser tabs: GitHub and Cloudflare.

**In GitHub**

1. Click your profile picture (top right) → **Settings**. This is your account's settings, not the repository's.
2. In the left sidebar, under "Code, planning, and automation", select **Pages**.
3. Select **Add a domain**, type `janedoe.com`, and select **Add domain**.
4. GitHub shows a TXT record with two parts: a **name** starting `_github-pages-challenge-your-username`, and a **value** (a string of letters and numbers). Leave this tab open.

**In Cloudflare**

5. In the dashboard, select your domain, then **DNS → Records**.
6. Select **Add record** and fill it in:

| Field | Enter |
| --- | --- |
| Type | TXT |
| Name | `_github-pages-challenge-your-username` (only this part; Cloudflare adds `.janedoe.com` itself) |
| Content | The value GitHub showed you |
| TTL | Auto |

7. Select **Save**.

**Back in GitHub**

8. Select **Verify**. If it fails, wait 10 minutes and try again; new records can take a while to show up.

Keep this TXT record for as long as you own the domain.

## Step 3: Point your domain at GitHub Pages

Five records tell the internet that `janedoe.com` and `www.janedoe.com` live on GitHub Pages. You add them all in Cloudflare.

1. In Cloudflare, select your domain, then **DNS → Records**.
2. If the list already has any **A**, **AAAA** or **CNAME** records named `janedoe.com` (or `@`) or `www`, delete them. Leave the TXT record from Step 2.
3. Select **Add record** and add each row below, one at a time, selecting **Save** after each.

| Type | Name | IPv4 address / Target | Proxy status |
| --- | --- | --- | --- |
| A | `@` | `185.199.108.153` | DNS only |
| A | `@` | `185.199.109.153` | DNS only |
| A | `@` | `185.199.110.153` | DNS only |
| A | `@` | `185.199.111.153` | DNS only |
| CNAME | `www` | `your-username.github.io` | DNS only |

**Proxy status must be DNS only (a grey cloud), not Proxied (an orange cloud).** Cloudflare turns the proxy on by default, so click the orange cloud on each record to turn it grey before you save. With the proxy on, GitHub can't set up the secure `https://` connection for your site.

The four numbers are GitHub Pages' addresses, from [GitHub's instructions](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site). Leave TTL on **Auto**.

## Step 4: Connect the domain to your portfolio

1. On GitHub, open your **portfolio** repository (not your account settings this time).
2. Select **Settings** (the tab along the top), then **Pages** in the left sidebar.
3. Under **Custom domain**, type `janedoe.com` and select **Save**.
4. GitHub runs a DNS check. Wait until it shows a green tick and **DNS check successful**. This usually takes a few minutes, occasionally a few hours.
5. Republish your site so its links use the new address: open the **Actions** tab, select **Publish site** on the left, then **Run workflow → Run workflow**. (Your next save in Pages CMS would also do it.)

You don't need to add any file to your repository. Older guides mention a `CNAME` file; your site publishes through GitHub Actions, which doesn't use one.

## Step 5: Turn on HTTPS and check

1. Stay in the repository's **Settings → Pages**. After the DNS check passes, GitHub sets up a security certificate for your domain. This takes from 15 minutes to about an hour.
2. When the **Enforce HTTPS** box can be ticked, tick it. Until then it is greyed out; come back later.
3. Check that each of these opens your portfolio, with a padlock in the address bar:
   - `https://janedoe.com`
   - `https://www.janedoe.com`
   - `https://your-username.github.io/portfolio/` (this old address now forwards to the new one)
4. Update your links: LinkedIn, itch.io, your résumé, email signature, and anywhere else you listed the old address.

## Afterwards

**Keep it running**

- **Renewal.** Cloudflare charges your card once a year. Keep the card on your account current. If the domain lapses, someone else can buy it.
- **Before deleting or renaming your portfolio repository**, remove the domain from its **Settings → Pages** first, then delete the records from Step 3.
- **Optional: Google Search Console.** Add your site as a **Domain** property. Google gives you a TXT record; add it in Cloudflare exactly as in Step 2, then select **Verify** in Google.

**If something goes wrong**

| What you see | What to do |
| --- | --- |
| GitHub's DNS check keeps failing | Wait an hour. Then compare your Cloudflare records with the table in Step 3, character by character. |
| **Enforce HTTPS** stays greyed out | Check every record in Step 3 shows a grey cloud (DNS only). Then, in the repository's **Settings → Pages**, select **Remove** next to the domain, type it again, and **Save**. Wait an hour. |
| "Not secure" warning or certificate error | Same as above: grey clouds, then remove and re-add the domain. |
| The domain shows a 404 page | In the **Actions** tab, check the latest **Publish site** run has a green tick. If not, run it again (Step 4, item 5). |
| `www.janedoe.com` doesn't work but `janedoe.com` does | Check the CNAME record: name `www`, target `your-username.github.io`, no `https://` and no `/portfolio`. |
| Images or styles missing on the new address | Republish (Step 4, item 5) so Alexander rebuilds the site for its new address. |

## Sources

- [Cloudflare: Register a new domain](https://developers.cloudflare.com/registrar/get-started/register-domain)
- [GitHub: Managing a custom domain for your GitHub Pages site](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site)
- [GitHub: Verifying your custom domain for GitHub Pages](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/verifying-your-custom-domain-for-github-pages)
- [CostGoat: Domain registrar price comparison (October 2026)](https://costgoat.com/compare/domains)
