# AI for Boomers website: handoff

**Goal:** publish this static one-page site at **https://aiforboomersbook.com** (with www redirecting to it).

## What's here
- `index.html`, `styles.css`, `assets/`: the full site. It's pure static HTML and CSS, with no build step and no server code.
- `screenshots/`: previews for desktop and mobile.
- Asset paths are relative, so the site works from any host root.

## Book facts (already in the site)
- Title: AI for Boomers: A Funny, Plain-English Guide for People Who Remember Rotary Phones
- Author: Tyler Redshaw. Imprint: Levered Press (© 2026)
- Amazon paperback: https://www.amazon.com/dp/B0HQPKZ68L ($14.99)
- Kindle: https://www.amazon.com/dp/B0HR2BW228 ($4.99)
- Bookstore ISBN, via Ingram/IngramSpark (55% discount, returnable): 979-8-234-29646-7
- Contact: redshawtj@gmail.com (mailto link, no contact form)
- Instagram: https://www.instagram.com/aiforboomersbook/

## Steps
1. **Register the domain** `aiforboomersbook.com`. It was available as of Nov 9, 2026 (RDAP check), and the expected cost is about $10–20 a year. Use any registrar, for example Cloudflare, Porkbun, Namecheap or Vercel. Turn on WHOIS privacy and auto-renew.
2. **Host it for free** on Vercel, Netlify, Cloudflare Pages or GitHub Pages. Deploy this folder as the site root. There is no build command, and the output directory is the root.
3. **Connect the domain.** Add `aiforboomersbook.com` and `www.aiforboomersbook.com` to the host, set the DNS records the host gives you, make the apex the primary, and redirect www to it. HTTPS should turn on automatically.
4. **Replace the canonical URL** in `index.html`, along with `og:url`, `og:image` and the JSON-LD `url`, with absolute `https://aiforboomersbook.com/...` URLs if they aren't already.
5. **Check after launch:**
   - The page loads over HTTPS on a phone and a desktop.
   - All the buy links open the right Amazon pages.
   - The sell-sheet PDF downloads.
   - The mailto link works.
   - Social preview: paste the URL into a Facebook or LinkedIn post preview, or opengraph.xyz.
6. **Link it everywhere:** the Instagram bio, the Amazon Author Central profile, the IngramSpark title (if it has a website field), the bookstore sell sheet, and bookstore submission forms.

## Ground rules
- Don't add tracking or analytics unless Tyler asks.
- Don't add reviews, testimonials or sales claims that aren't real.
- The author bio uses only these facts: lives in Vienna, VA; grew up in Richmond; went to UVA; software engineer.

## Nice-to-haves later
- An email signup for future books (Buttondown, MailerLite or ConvertKit).
- A "Find it locally" list as bookstores start stocking it.
- A contact form through Formspree or Netlify Forms, if spam becomes a problem.
