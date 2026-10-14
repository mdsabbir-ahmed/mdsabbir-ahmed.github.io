# Archived V3 release notes

This document describes the previous iteration. The current verified roles and any title corrections are documented in `RELEASE-NOTES-V4.md` and `SOURCE-AUDIT-V4.md`.

# v3 revision: Academic community and visual identity

## Design

- Revised theme from teal-heavy modern UI to deep navy (#19273A), warm ivory (#F6F4F0), and restrained bronze (#785339).
- Switched headings to Source Serif 4 (Georgia fallback) and body copy to Source Sans 3 (system fallback).
- Reduced visual noise: flatter cards, lighter borders and shadows, reduced rounded corners, clearer headings.
- Improved mobile homepage reading order (research introduction before portrait).
- Preserved contrast on white backgrounds: navy 15.08:1, body slate 6.1:1, bronze links 6.79:1.

## Community leadership

- Added `/community/` page with individual entries for Asia SIGCHI Committee Vice Chair, HCCS Co-Founder and Associate Director, ACM SIGCHI Dhaka Chapter Treasurer, and HCI Winter School 2027 organizing leadership.
- Added homepage affiliation strip and extended leadership cards, all with contextual links.
- Split institutional roles, scholarly reviewing, and recognition into distinct `/service/` page.
- Updated navbar order and homepage text.

## Editorial verification

- Official SIGCHI committee directory confirms `Vice Chair`: https://sigchi.org/people/committees/asia-committee/
- HCCS web pages provided by the user are linked, but were not accessible through website retrieval during revision.
- BRAC University public profile still says `Assistant Director & Communications Lead` for HCCS. The more recent user-provided history says `Co-Founder and Assistant Director (corrected in v4)`. Confirm current HCCS wording before going live. Homepage uses neutral `Co-Founder and Assistant Director (corrected in v4)`; detailed Community page uses `Co-Founder and Assistant Director (corrected in v4)` pending confirmation.
- Existing publications and research pages remain unchanged aside from global typography/color styling.

## Checks performed

- YAML parsed for configuration and profile data.
- No missing relative links across site pages and local media.
- Responsive static HTML preview at 1440 px and 390 px widths showed no horizontal overflow.
- Production Jekyll build is **not** verified locally because gems are not installed; check GitHub Actions first-run logs.
