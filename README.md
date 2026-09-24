# ScanHeaders.com Changelog

Curated development history for [ScanHeaders.com](https://scanheaders.com/), a lightweight HTTP response-header scanner and technical reference.

Current version: **v1.0.1**

**Project links:** [Live scanner](https://scanheaders.com/) · [Knowledge Base](https://scanheaders.com/knowledge-base/) · [How Scans Work](https://scanheaders.com/how-scans-work/) · [About](https://scanheaders.com/about/) · [Contact](https://scanheaders.com/contact/)

> This changelog intentionally records meaningful product, architecture, content, security, and design milestones. Minor back-and-forth spacing, padding, alignment, color experiments, and other temporary visual adjustments have been omitted.

---

## v1.0.1 - September 24, 2026
### Final contact and presentation refinements

- Refined the [Contact form](https://scanheaders.com/contact/) while preserving the already-tested SMTP delivery, CSRF protection, honeypot, rate limiting, validation, and Reply-To behavior.
- Applied the ScanHeaders label typography consistently and balanced input/select sizing and spacing.
- Placed Name and Email side by side on wider screens with a clean responsive one-column layout on mobile.
- Changed Contact email output to use the human-readable selected topic, such as `General question`, instead of internal values such as `question`.
- Removed the divider directly below the Contact form without affecting dividers elsewhere.
- Standardized the production SMTP configuration path to `/home/customer/www/scanheaders.com/data/smtp.php`, kept outside the public website ZIP.
- Kept the visitor's address as Reply-To while mail is sent from the ScanHeaders project mailbox.
- Updated Knowledge Base Open Graph type to `article` while retaining `TechArticle` JSON-LD.
- Improved the footer/socket text contrast.
- Optimized remaining SVG brand assets and removed unnecessary editor metadata.
- Normalized remaining brand-red asset values to `#d10000`.
- Preserved scanner rules, ReScan behavior, caching, JavaScript, structured data, navigation, and the rest of the finished site.

---

## v1.0.0 - September 23, 2026
### First stable release

- Promoted [ScanHeaders.com](https://scanheaders.com/) from the development series to the first stable release.
- Removed the final obsolete development-era homepage wording.
- Completed the historical project changelog and stable-release documentation.
- Aligned the animated and reduced-motion scanner line with the final brand red.
- Preserved the completed scanner core, ReScan system, cached self-report, SEO/schema layer, social metadata, Contact architecture, and responsive design.
- Kept the project lightweight and deployment-friendly with no database, analytics, user accounts, tracking, or scan-history service.

---

## v0.13.0 - September 23, 2026
### Final launch-readiness pass

- Updated obsolete scanner-development wording across public pages and local search content.
- Expanded the [About](https://scanheaders.com/about/) page and rewrote [How Scans Work](https://scanheaders.com/how-scans-work/) around the real implemented scanner.
- Added centralized Open Graph metadata and X/Twitter large-image cards.
- Added factual JSON-LD across public pages, including `WebSite`, `WebPage`, `CollectionPage`, `TechArticle`, `AboutPage`, `ContactPage`, and real-route breadcrumbs where appropriate.
- Reviewed titles, meta descriptions, canonicals, indexing, sitemap behavior, Search/404 noindex handling, and internal route consistency.
- Integrated the final 1200 × 630 social image, SVG favicon with PNG fallback, animated scanner icon, and updated ScanHeaders wordmark.
- Added reduced-motion handling for the scanner animation and corrected mobile wordmark/menu stacking.
- Replaced the old minimal `llms.txt` with a comprehensive live-service reference file.
- Preserved the supplied `.htaccess` security and custom response headers while extending protection for credential/configuration and backup files.
- Replaced native PHP `mail()` delivery with authenticated SMTP using a minimal PHPMailer source set.
- Preserved Contact validation, CSRF, honeypot, rate limiting, safe Reply-To behavior, and generic public delivery errors.
- Reframed homepage sample content as guidance for interpreting scan findings.
- Updated the footer copyright identity to MILAN INNOVATIONS LLC.
- Preserved the existing scanner engine and rule behavior unchanged.

---

## v0.12.2 - September 20, 2026
### ReScan for every completed report

- Added the inline ReScan control to every completed live report on the [scanner](https://scanheaders.com/), not only the cached ScanHeaders.com self-report.
- Preserved the exact normalized original target, including query strings, independently of the editable scanner field and any redirected final URL.
- Successful rescans replace the current result; failed rescans keep the previous successful report visible.
- Prevented duplicate rescan requests while a scan is already running.
- Kept cached-default refresh behavior isolated from normal visitor scans.
- Reused the existing endpoint, protections, rate limiting, renderer, and loading behavior without scanner-rule changes.

---

## v0.12.1 - September 20, 2026
### Cached self-report and launch UX

- Replaced the synthetic default example report with support for a persistent cached [ScanHeaders.com](https://scanheaders.com/) self-report.
- Added the inline ReScan control for refreshing the cached homepage result.
- Made cache replacement failure-safe so an unsuccessful refresh does not erase the previous report.
- Enabled normal public pages for indexing while keeping Search, scanner/API, 404, tests, and internal utility routes appropriately non-indexed.
- Improved scan completion and error focus/scroll behavior.
- Added reduced-motion support.
- Capitalized the report explanation labels: `Why Good?`, `Why Improve?`, `Why Issue?`, and `Why Info?`.
- Preserved the live scanner rules, network protections, raw-header handling, redaction, and rate limiting.

---

## v0.12.0 - September 20, 2026
### Live scanner integration

The previously static report interface became the real [ScanHeaders.com live scanner](https://scanheaders.com/).

- Connected the homepage form to a same-origin asynchronous PHP scanner.
- Added bare-hostname support with HTTPS as the default scheme.
- Added loading states, duplicate-submission prevention, retries, errors, and accessible result focus.
- Built modular scanner components for request collection, validation, redirect handling, normalized headers, rule evaluation, report rendering, and rate limiting.
- Added SSRF protection for private, loopback, link-local, reserved, and other non-public destinations.
- Revalidated every redirect destination and kept TLS certificate verification enabled.
- Added bounded GET handling, redirect limits, header/body limits, and request timeouts.
- Added database-free filesystem rate limiting.
- Implemented the production status model: **Good / Improve / Issue / Info**.
- Added contextual analysis for [Security Headers](https://scanheaders.com/security-headers/), [Caching Headers](https://scanheaders.com/caching-headers/), [CORS & Cookies](https://scanheaders.com/cors-cookies/), cross-origin controls, and server/response metadata.
- Added expandable explanations and request-path details.
- Preserved repeated and unknown final-response headers in Raw Response Headers.
- Kept `Set-Cookie` lines separate and redacted cookie values and obvious credentials.
- HTML-escaped remote values before rendering.
- Preserved the lightweight PHP/HTML/CSS/vanilla-JavaScript architecture.

---

## v0.11.0 - September 18, 2026
### Content completion, accessibility, and Contact expansion

- Expanded the [Knowledge Base](https://scanheaders.com/knowledge-base/) from the initial article set to the full 37-article catalog.
- Added additional header references, troubleshooting guides, server examples, and configuration material.
- Improved accessibility, navigation behavior, link semantics, and internal routing.
- Added the protected [Contact form](https://scanheaders.com/contact/) foundation with validation, CSRF, honeypot, rate limiting, safe headers, and no database.
- Finalized legal/responsibility document presentation and dates, including the [Vulnerability Disclosure](https://scanheaders.com/vulnerability-disclosure/) policy.
- Improved sitemap/canonical handling and protected internal/handoff files from public access.
- Completed X-Powered-By suppression.
- Preserved the established homepage and report design while the live scanner implementation was still pending.

---

## v0.10.0 - September 18, 2026
### Informational site and Knowledge Base foundation

- Completed the major informational-site phase.
- Added the first 17 articles to the [Knowledge Base](https://scanheaders.com/knowledge-base/) across Header Reference, Configuration Guides, Common Problems, and Server Examples.
- Added practical Apache, Nginx, Caddy, and PHP examples.
- Completed the four Knowledge Base section landing pages.
- Added lightweight local documentation search.
- Added the custom 404 page.
- Completed [About](https://scanheaders.com/about/), [How Scans Work](https://scanheaders.com/how-scans-work/), [Contact](https://scanheaders.com/contact/), Knowledge Base, and supporting informational pages.
- Updated sitemap coverage and internal documentation links.
- Preserved the established visual design and approved legal/responsibility wording.

---

## v0.9.x - September 17, 2026
### Interface, legal, and topic-page refinement series

The v0.9 development series contained many small visual iterations. This condensed entry keeps only the meaningful results.

- Refined the report summary into the final balanced split layout used by later scanner releases.
- Established the final status presentation, icon set, report typography, and Raw Response Headers styling.
- Improved request-path presentation and overall report readability.
- Performed a safe CSS/responsive cleanup and removed obsolete styling without redesigning the site.
- Added and organized the Responsibility section.
- Added [Environmental Responsibility](https://scanheaders.com/environmental-responsibility/) and [Diversity & Inclusion Statement](https://scanheaders.com/diversity-inclusion-statement/).
- Integrated the approved [Terms of Use](https://scanheaders.com/terms-of-use/), [Privacy Policy](https://scanheaders.com/privacy-policy/), [Data & Risk](https://scanheaders.com/data-and-risk/), Environmental Responsibility, Diversity & Inclusion Statement, and Vulnerability Disclosure content.
- Unified Legal and Responsibility document navigation.
- Rebuilt [Security Headers](https://scanheaders.com/security-headers/), [Caching Headers](https://scanheaders.com/caching-headers/), and [CORS & Cookies](https://scanheaders.com/cors-cookies/) into consistent overview pages with concepts, key controls, and Knowledge Base links.
- Added social-profile metadata and refined project/footer structure.

---

## v0.5 - v0.8 - September 15-16, 2026
### Branding and site-structure foundation

- Integrated the ScanHeaders SVG wordmark and inverse/footer variant.
- Established responsive logo behavior.
- Expanded the site's primary navigation, documentation structure, footer, legal sections, and Knowledge Base foundation.
- Added the project's social-profile links.
- Refined the homepage visual identity and report icon system.
- Established the 990 px scanner-form width and reusable content/page templates.
- Removed RSS because ScanHeaders.com is a technical service rather than a blog.

---

## v0.4 - September 15, 2026
### Report interface redesign

- Redesigned the early dummy report into the structure that became the basis of the production scanner.
- Added the report summary card and grouped findings for Security Headers, Caching Headers, CORS & Cookies, and Server & Response.
- Added clearer status pills and table-like responsive rows.
- Expanded the Raw Response Headers area.
- Improved report behavior on smaller screens.

---

## v0.1 - v0.3 - September 15, 2026
### Initial build and report prototype

- Adapted the lightweight PHP site template into ScanHeaders.com.
- Established plain PHP, HTML, CSS, and vanilla JavaScript as the project stack.
- Designed the homepage around HTTP response-header scanning.
- Added the scanner input as an initial non-functional interface.
- Built the first Website Header Report prototype, empty state, grouped sample findings, and Raw Response Headers area.
- Added development preview states used while the report UI was being designed.
- Applied development noindex protection while the project was not ready for public launch.

---

## Project origins - September 4-8, 2026

- Selected [ScanHeaders.com](https://scanheaders.com/) as the project and domain.
- Defined the service as a lightweight HTTP response-header scanner with clear explanations rather than a generic vulnerability scanner.
- Expanded the scope beyond security headers to include caching, CORS, cookies, redirects, server/response metadata, and raw response headers.
- Chose PHP + cURL with HTML/CSS/vanilla JavaScript and rejected WordPress and heavyweight frameworks.
- Defined SSRF protection, redirect validation, protocol restrictions, timeouts, response limits, and abuse resistance as mandatory requirements for any live scanner.
- Established the long-term preference for no accounts, minimal data collection, no behavioral tracking, contextual findings, and practical technical guidance.
- Early numeric/letter scoring ideas were replaced by the more contextual **Good / Improve / Issue / Info** model.

---

## Development principles

- Lightweight implementation.
- PHP, HTML, CSS, and vanilla JavaScript.
- SiteGround shared-hosting compatibility.
- US spelling and vocabulary.
- No unnecessary database.
- No behavioral analytics or tracking.
- Minimal data collection and no user scan-history service.
- Preserve unknown/custom fields in Raw Response Headers.
- Explain HTTP behavior in context rather than treating every optional header as mandatory.
- Keep overview pages approachable and use the [Knowledge Base](https://scanheaders.com/knowledge-base/) for deeper technical material.
- Prefer stable, focused refinements over unnecessary architectural rewrites.

---

## More about ScanHeaders

- [ScanHeaders.com](https://scanheaders.com/)
- [Security Headers](https://scanheaders.com/security-headers/)
- [Caching Headers](https://scanheaders.com/caching-headers/)
- [CORS & Cookies](https://scanheaders.com/cors-cookies/)
- [Knowledge Base](https://scanheaders.com/knowledge-base/)
- [How Scans Work](https://scanheaders.com/how-scans-work/)
- [About ScanHeaders](https://scanheaders.com/about/)
- [Contact](https://scanheaders.com/contact/)
