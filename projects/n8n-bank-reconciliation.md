# Automated bank reconciliation in n8n

| | |
|---|---|
| **Sector** | Finance, legal and compliance |
| **Source code** | not versioned on GitHub — available on request |

## What it is

Bank reconciliation automation in n8n, integrated with Supabase — the orchestrated version of the same problem that KPI Gestão solves as an application. It accepts statements in CSV, XLSX, XLS, PDF and image formats, with encoding detection, column mapping and OCR for formats that have no text layer. It matches by date and amount against what is already in Supabase, returns a preview before confirming, and sends a final report by webhook or email, with error handling at every step of the flow. It includes a monitoring dashboard and its own test suite.

## Stack

```
axios · form-data · xlsx
```

---

[← back to index](../README.md)
