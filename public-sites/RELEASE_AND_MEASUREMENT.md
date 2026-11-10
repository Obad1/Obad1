# AVAMALE PUBLIC SITE RELEASE AND MEASUREMENT PLAN

Date: 2026-11-11

## Per-vertical site and lead measurement

| Product | Render static service | URL | Inquiry identifier |
|---|---|---|---|
| Evidence | srv-dbpq83ifngtc73851s70 | https://avamale-aa01-pilot.onrender.com/ | EVIDENCE |
| Reconcile | srv-dbpq848u01pc738sgkv0 | https://avamale-aa02-pilot.onrender.com/ | RECONCILE |
| FreightCheck | srv-dbpq850u01pc738sgocg | https://avamale-aa03-pilot.onrender.com/ | FREIGHTCHECK |
| AP Match | srv-dbpq866k1f9s73cl3av0 | https://avamale-aa04-pilot.onrender.com/ | AP MATCH |

Each service has an independent Render request-count metric. Capture daily HTTP request counts, but do not mistake requests (including bots or refreshes) for unique humans. Count inbound email and WhatsApp enquiries separately, using the Service line in the prepared messages; manual qualification and deduplication are required. Track: inquiry received / reply sent / sample accepted / report delivered / diagnostic quoted / paid / case study consented. Stop outreach to a contact upon reply. Do not infer form submissions from click counts.

## Privacy and attribution

Do not add Google Analytics, Meta pixels, trackers or third-party intake scripts without privacy and consent review. There are no tracking cookies in the static sites as authored. The four sites currently have noindex,nofollow metadata until one has distinct positioning, live funnel verification and permission to begin SEO. Avoid UTM parameters in links shared with prospects unless there is a deliberately approved measurement plan.

## Release checks before outreach

1. Confirm Render has deployed a commit containing updated index.html, privacy.html, terms.html, 404.html, sample-report.csv and engagement-template.html. Earlier Render get_deploy returned the initial deployment only; do not claim these files live until verified.
2. From an unauthenticated device on cellular data, test homepage, sample CSV download, privacy, terms, SOW print view, email CTA, WhatsApp CTA and mobile responsiveness on each site.
3. Verify readable contrast and keyboard navigation at narrow widths and throttled connection. Verify the site responds 200 and that the source displays the new text.
4. Send a synthetic inquiry using each channel and confirm it lands with a recognizable service identifier. Never send personal financial documents for testing.
5. Ensure finance offers state document comparison, not audit assurance; all source-excerpt and fictional disclaimers are retained.
6. Before customer paid work: verify legal entity/CAC details, named qualified reviewers, a signed engagement letter, fixed payment and refund terms, secure file intake, NDA/DPA as applicable, documented storage, access, retention and deletion, and an actual backup/recovery test.
7. Review whether the first three founding pilots receive a 30% discount and whether it applies to the proposed domestic fee or another agreed quote; do not promise it without a signed quote.

## AskDocs

The source repository includes a fictional sample document and a Gradio sample loader; its source display now formats passage snippets using chunk references. The user-facing production Render service is a separate application path and must be tested for applicability before calling this change live. No verified file size, non-English fidelity, browser-storage ceiling, adaptive quiz engine or full restore guarantee is represented.

## Decision rule

Keep four standalone test sites for outreach and per-vertical measurement, but do not index four near-identical variants for SEO. Consider consolidating strong-performing verticals under a shared branded domain after meaningful inquiry and conversion data exists.
