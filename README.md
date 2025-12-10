# VulnDaily

> Daily vulnerability briefings for those who work smart, not hard. 

Showcasing a summary of:
- Newly disclosed CVEs  
- Known exploited vulnerabilities  
- CISA alerts and vendor advisories  
- Notable security news and patches  

Each morning, a script aggregates data from public feeds and drops a new
Markdown post into the blog under [`_posts/`](./_posts). GitHub
Pages builds the site automatically.

---

## Live site
Hot off the press: `https://experiencinghumanit.github.io/vulndaily/`

You should see:
- A **Home** page listing the most recent daily summaries  
- A **detail page** for each day with the full Markdown report  

---

## Repository structure
- `README.md` – Entry page for Pages
- `_config.yml` – Jekyll configuration
- `_layouts/` – HTML layouts
- `_posts/` – Auto-generated daily vulnerability roundups (`YYYY-MM-DD-vulndaily.md`)
- `index.md` – Home page listing recent posts

---

## Publishing a new daily report
Python script writes a new file into `_posts/` with front matter:

   ```yaml
   ---
   layout: post
   title: "Daily Vulnerability Summary — 2025-12-10"
   date: 2025-12-10 06:00:00 +0000
   source_count: "12+ feeds"
   vuln_count: "Vulns"
   ---
