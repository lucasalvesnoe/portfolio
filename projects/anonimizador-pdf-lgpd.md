# PDF anonymiser for LGPD

| | |
|---|---|
| **Client** | State-owned urban transport company |
| **Sector** | Public sector |
| **Source code** | private repository — read access on request |

## What it is

An automatic PDF anonymiser for LGPD (Brazil's GDPR) compliance, built for an urban transport company and styled to match the original portal. The workflow is not regex-based: text is extracted with PyMuPDF and sent to Claude with an LGPD classification prompt, which returns JSON listing the sensitive entities found — taxpayer and ID numbers (CPF, CNPJ, RG), email, phone, postcode, name, address, bank details and card numbers — and each occurrence is applied back to the PDF as a real black redaction box via `add_redact_annot` + `apply_redactions`. This matters: the redaction is applied at the document layer, so the underlying text is destroyed, not merely covered. The response returns the anonymised PDF as base64 plus an auditable list of everything that was masked. Flask + Python 3, with login and a health check.

## Stack

```
flask · flask-cors · pymupdf · anthropic · python-dotenv · gunicorn
```

---

[← back to index](../README.md)
