# Academic Website & Portfolio — Nguyen Bao Trung, MD, MSc

This repository powers the personal academic website of **Nguyen Bao Trung, MD, MSc** ([trungnb.github.io](https://trungnb.github.io)), built with [AcademicPages](https://academicpages.github.io) and hosted on **GitHub Pages**.

---

## 📂 Repository Structure

* **`_config.yml`**: Global site configuration (Name, bio, ORCID, affiliations, social links).
* **`_pages/`**:
  * `about.md`: Homepage bio, research interests, and recent news.
  * `cv.md`: Online Curriculum Vitae.
  * `publications.html`, `portfolio.html`, `teaching.html`: Section index pages.
* **`_publications/`**: Markdown files for each peer-reviewed publication or manuscript.
* **`_portfolio/`**: Markdown files for applied AI projects, platforms (e.g., *PeriApicaI*), and software.
* **`_teaching/`**: Markdown files for mentorship and academic supervision activities.
* **`files/`**: Place downloadable PDFs here (e.g., full CV PDF, paper preprints).
* **`images/`**: Site icons, favicons, and profile pictures (`profile.jpg`).

## 🌐 Bilingual Content Convention

English and Vietnamese pages are maintained as explicit pairs:

* English content uses `lang: en`; Vietnamese content uses `lang: vi`.
* Each pair shares the same `translation_key` and has matching URL structure under `/` and `/vi/`.
* Collection entries should keep the same date in both languages so the index pages remain newest-first.
* New pages and collection entries should be added in both languages, with `lang`, `translation_key`, `permalink`, and localized UI labels set in the front matter where needed.

The language switcher uses `translation_key` to open the equivalent page. If a translation is not available yet, it falls back to the corresponding language homepage.

---

## 📸 How to Update Your Profile Photo (Avatar)

1. Save your portrait photo as **`profile.jpg`** (or `.png`).
2. Put it into the **`images/`** folder (replacing `images/profile.jpg`).
3. *(Alternative)*: If you put your image inside **`files/bio.jpg`**, update line 14 of `_config.yml`:
   ```yaml
   author:
     avatar: "../files/bio.jpg"
   ```
4. Commit and push to GitHub.

---

## 📝 How to Add a New Publication

Create a new file in `_publications/` (e.g., `2026-06-01-new-paper-title.md`):
```yaml
---
title: "Your Paper Title Here"
collection: publications
lang: en
translation_key: new-paper-title
permalink: /publication/2026-06-01-new-paper-title
excerpt: "Short 1-2 sentence summary of findings."
date: 2026-06-01
venue: 'Journal Name'
paperurl: 'https://doi.org/your-doi-link'
citation: '<strong>Nguyen BT</strong>, et al. (2026). &quot;Your Paper Title.&quot; <i>Journal Name</i>.'
---

### Abstract
Abstract text goes here...
```

---

## 🚀 Deployment

Any commit pushed to the `main` branch will automatically trigger GitHub Pages to build and deploy the live site in ~1 minute.
