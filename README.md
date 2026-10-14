# Md. Sabbir Ahmed | Academic Research Portfolio

**Source repository:** `mdsabbirahmedbracu/mdsabbirahmedbracu.github.io`  
**Public URL:** https://mdsabbirahmedbracu.github.io/

This is an **actual Jekyll/al-folio v1** site using the `al_folio_core` Ruby gem and the al-folio bibliography, navigation, and search plugin ecosystem. It is not the earlier one-page HTML portfolio.

## Design revision (October 2026)

This version emphasizes **academic community leadership** with a dedicated `/community/` page and separate official/context links for the Asia SIGCHI Committee, HCCS Research Group, ACM SIGCHI Dhaka Chapter, and HCI Winter School 2027. The homepage includes a leadership ribbon immediately below the introduction and three expanded community cards. University administration and reviewing have been moved into the separate `/service/` page. Colors and fonts have been updated to a reserved navy, ivory, and bronze palette with Source Serif 4 and Source Sans 3.

## Deploy to your existing repository

1. Back up the current `main` branch (for example, download its ZIP or create an `old-portfolio` branch).
2. Extract this ZIP and copy **everything inside** `mdsabbirahmedbracu-alfolio-site/` to the **root** of your existing GitHub repository. Include `.github/workflows/deploy.yml`, dotfiles, `_config.yml`, `Gemfile`, the `_pages` directory, and assets. Do not nest the folder inside the repository.
3. Remove obsolete old-site items such as the previous root-level `index.html`, `css/`, `js/`, `libs/`, and `gulpfile.js`. **This is essential:** the old root `index.html` would override the new Jekyll `/` homepage.
4. Commit and push to `main`.
5. Under **GitHub → Settings → Pages → Build and deployment**, choose **GitHub Actions** rather than "Deploy from a branch".
6. Open the **Actions** tab and inspect the `Build and deploy academic website` workflow. Once successful, open https://mdsabbirahmedbracu.github.io/.

## Local run

Requires Ruby 3.3 and Bundler, plus access to RubyGems to install dependencies.

```bash
bundle install
bundle exec jekyll serve --livereload
```

Open http://localhost:4000/. RubyGems is required for the *first* installation. This ZIP does not vendor theme gems, in line with al-folio v1 architecture.

## How to update content

| Edit | File |
| --- | --- |
| Short bio and homepage features | `_pages/about.md` |
| Research agenda | `_pages/research.md` |
| Peer-reviewed publications | `_bibliography/papers.bib` |
| Research projects | `_projects/*.md` |
| Teaching and mentoring | `_pages/teaching.md` |
| Regional and local HCI community leadership | `_pages/community.md` |
| Institutional and scholarly service | `_pages/service.md` |
| News | `_pages/news.md`; optionally use `_news/*.md` for dated announcements |
| Academic/social links | `_data/profile.yml`, `_data/socials.yml` |
| Primary photo | `assets/img/prof_pic.jpg` |
| Downloadable CV | `assets/pdf/Md_Sabbir_Ahmed_Academic_CV.pdf` |
| Design: navy/ivory/bronze, Source Sans 3 + Source Serif 4 | `assets/css/portfolio.css` |
| Al-folio config | `_config.yml` |

## Academic community roles and source verification

- The official [Asia SIGCHI Committee directory](https://sigchi.org/people/committees/asia-committee/) identifies Md. Sabbir Ahmed as **Vice Chair**.
- HCCS pages provided by the user are linked at `https://hccs.cse.bracu.ac.bd/` and `/people`. These pages were not retrievable in the development environment. The publicly indexed BRAC University faculty profile lists **Assistant Director & Communications Lead**, and the user explicitly confirms the current website title as **Co-Founder and Assistant Director**. Both the Community and homepage display this exact title. The HCCS website and people directory are linked but could not be loaded for independent verification in the authoring environment.
- The ACM SIGCHI Dhaka Chapter role is **Treasurer**; Winter School 2027 is presented as an organizing initiative, not a separate elected office.
- Each academic-community role now has separate content, organizational context, practical contributions, and official links when available.

## Research integrity and content decisions

- The newer four-page CV supplies the primary factual basis. The older five-page CV and LinkedIn export fill in teaching and earlier publication history. The exact HCCS role was additionally confirmed directly by the user in October 2026.
- Only **published** works appear in BibTeX; manuscripts under review were not silently presented as accepted work.
- Project pages distinguish PI, co-PI, collaboration, and local coordination roles, and avoid asserting as-yet-unpublished results.
- The brown-suit portrait is the chosen homepage picture. The navy portrait is retained as an optional source image.
- All seven user-provided academic links are included on the contact page; both email addresses are public.
- Previously omitted older papers have been restored where the user’s academic CV and public publication metadata provide author and DOI details. Bibliography records should still be compared with the publisher record before final release.

## Before publishing: publication and status verification

Please verify final author spellings, titles, and DOIs against publishers, and check that descriptions of ongoing studies remain appropriate for public release. The **USENIX 2026 entry links to the verified official USENIX presentation page**. That publication does not have a conventional DOI in its USENIX record. The public News page uses years rather than claiming announcement dates.

## Build limits for this delivery

The authoring environment could validate file structure and data but could not fetch Ruby gems from RubyGems or execute a real Jekyll build. Please treat the first GitHub Actions run as the integration test. Resolve any plugin compatibility error with its log and avoid replacing this site with the old HTML page.

The configuration pins al-folio plugin versions drawn from the upstream v1 series and uses an HTML/CSS content layer that preserves compatibility with the plugin-backed default layout. This is not a full copy of upstream al-folio source. If you prefer full upstream code, start from the official template then transfer `_pages`, `_projects`, `_bibliography`, `_data`, `assets`, and `_config` values from this package.

Official theme: https://github.com/alshedivat/al-folio  
Documentation: https://github.com/alshedivat/al-folio/tree/main/docs
