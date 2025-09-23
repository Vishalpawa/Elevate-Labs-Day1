# Task 2 — Phishing Email Analysis (Simulated Samples)

## Objective
Analyze simulated phishing emails and identify phishing indicators for defensive training.

## Samples used
- `sim_phish_account_verification.txt` — Account verification simulation.
- `sim_phish_invoice.txt` — Fake invoice simulation.
- `sim_phish_delivery.txt` — Delivery attempt simulation.

_All samples are explicitly marked `[SIMULATION - DO NOT RESPOND]` and use test/example domains and benign attachments._

## Steps performed
1. Obtained the three simulated samples (created for training).
2. Examined displayed sender addresses for spoofing and typos.
3. Analyzed synthetic raw headers using a header analyzer to inspect Received paths and Return-Path.
4. Inspected URLs in the email body (hovered / inspected) to check for mismatched or suspicious domains.
5. Examined attachment names and file types (all plain text for safety).
6. Reviewed email body for urgency, generic greetings, and grammar issues.
7. Documented indicators and wrote this summary.

## Findings (summary)
- **Account verification sample:** Urgent verification request; link points to an example-training domain; generic greeting; synthetic headers show origin IP `203.0.113.45` (test IP).
- **Invoice sample:** Overdue payment scare tactic; attachment named `invoice_INV-7834.txt` (benign); link uses an example domain with query string; synthetic headers show `203.0.113.46`.
- **Delivery sample:** Delivery threat with short deadline; tracking link points to simulated-tracking.example; generic greeting; synthetic headers show `203.0.113.47`.

All three messages contain common phishing indicators: urgency, link-based call-to-action, generic greetings, and suspicious sending origins (in a realistic scenario).

## Conclusion
These samples are confirmed as simulated phishing training material. The indicators identified (spoofed-looking senders, urgent language, mismatched URLs, and suspicious headers) align with typical phishing techniques. Use only in controlled environments with test accounts.

## Safety notes
- Do not send these samples to real, uninformed users.
- For large-scale realistic simulations, use a professional platform that handles consent and reporting.
- Always perform header analysis and link inspection in a safe environment (no clicking unknown links on production machines).
