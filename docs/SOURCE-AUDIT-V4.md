# Source audit and content assurance (14 October 2026)

## Source priority
1. **User correction (14 October 2026):** HCCS title is exactly **Co-Founder and Assistant Director**. Do not replace it with Associate Director, Research Leader, or another title.
2. **Current academic CV:** `CV_Md Sabbir Ahmed(1).pdf`, 4 pages, used for degrees, appointments, current paper and grant information, research projects, and university/community service.
3. **User-supplied LinkedIn About text and LinkedIn export:** `Profile.pdf`, used to check the positioning of the research biography and community appointments.
4. **Older detailed academic CV:** `CV_Sabbir_Detailed_Academic_2025.pdf`, used primarily for earlier papers and teaching/service records. Some older dates conflict with the latest CV and are not used where there is a discrepancy.
5. **Public institutional and society directories:** [BRAC University profile](https://cse.bracu.ac.bd/faculty_profile/54/md_sabbir_ahmed) and [SIGCHI Asia Committee](https://sigchi.org/people/committees/asia-committee/). BRACU lists `Assistant Director & Communications Lead` for HCCS; SIGCHI currently lists `Vice Chair` for Md. Sabbir Ahmed. HCCS site was supplied by user but not directly retrievable during development.

## Specific assertions and grounding

| Website assertion | Source | Treatment |
| --- | --- | --- |
| Md. Sabbir Ahmed, Senior Lecturer, BRAC University | Current CV p. 3; institutional profile | Retained |
| MSc CSE 2025, GPA 4.00; BSc CSE 2021, GPA 3.97 | Current CV p. 1 | Retained; do not use older CV's obsolete MSc end date |
| HCI, Human-Centered and Trustworthy AI, Usable Security and Privacy, Social Computing | Current CV p. 1; user-provided LinkedIn About | Retained |
| USENIX 2026 equal contribution among three marked authors | Current CV p. 1 | 'Co-first author' retained |
| CHI 2025 and COMPASS 2026 published papers | Current CV p. 1; DOI links | Retained |
| More than 50 thesis/project groups | Current CV p. 4; LinkedIn About | Retained as '>50', not expanded to a new exact count |
| S2S Principal Investigator, BDT 600,000 RSGI funding | Current CV pp. 2–3 | Retained as ongoing, with no effectiveness findings claimed |
| Asia SIGCHI Committee Vice Chair | Latest CV p. 3; LinkedIn About; SIGCHI directory | Retained |
| HCCS Co-Founder and Assistant Director | Direct user confirmation + BRACU profile supporting Assistant Director | Corrected on homepage and Community page |
| ACM SIGCHI Dhaka Treasurer | Latest CV p. 3; LinkedIn About | Retained |
| HCI Winter School 2027 involvement | Latest CV p. 3; LinkedIn About | Retained as planned/co-organizing initiative, no outcomes claimed |
| Both emails and research profile URLs | User-provided links + CVs | Retained |
| Earlier 2020–2025 publications | Detailed CV 2025, plus publicly indexed DOI/author metadata where available | Three missing entries added; bibliography now 18 items |

## Editorial safeguards
- The website's research questions and section headings are *editorial framing*, not study findings or claims of completed research outcomes.
- Work under review and manuscripts in preparation are not listed as published papers.
- All descriptions of ongoing studies are based on their documented aims and roles. Unpublished results are not displayed.
- The 2025 detailed CV differs from the 2026 CV on MSc completion dates; the current CV takes precedence.
- The public HCCS directory could not be fetched here. The exact Co-Founder wording is the user's direct confirmation, rather than an independently fetched institutional statement.
- Some 2022/2023 author listings in the old CV are abbreviated; restored BibTeX entries were cross-checked against BRACU/dblp/conference bibliographies and should still be checked before public launch.
- Publication data, project statuses, roles, and all external links should be checked at final release, especially when sources are updated.
- Source audit is for site maintenance, not intended to be published as a website page.
