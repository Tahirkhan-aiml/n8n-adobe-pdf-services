 Adobe PDF Services API Wrapper for n8n

One workflow. All Adobe PDF operations. 
Extract text/tables, split, merge, OCR — no code.

> Input: PDF + operation → Output: JSON, ZIP, or files

![Adobe](https://img.shields.io/badge/Adobe%20PDF%20Services-FF0000?style=for-the-badge&logo=adobe) ![n8n](https://img.shields.io/badge/n8n-FF6B6B?style=for-the-badge&logo=n8n)



 Features

| Check | Feature |
|-------|--------|
| Check | Full Adobe PDF Services API support |
| Check | Authentication (OAuth token) |
| Check | Asset upload (PDF binary) |
| Check | Polling until job completes |
| Check | Download result (JSON, ZIP, etc.) |
| Check | Reusable sub-workflow |
| Check | No polling loops — Smart wait + retry |



 Supported Operations

| Operation | Endpoint | Output |
|---------|----------|--------|
| Extract Text & Tables | `extractpdf` | `extract.zip` |
| Split PDF | `splitpdf` | Multiple PDFs |
| Combine PDFs | `combinepdf` | Single PDF |
| OCR | `ocrpdf` | Searchable PDF |
| Compress | `compresspdf` | Smaller PDF |



 How to Use

 1. Import Workflow
→ Click [adobe-pdf-services-wrapper.json](adobe-pdf-services-wrapper.json) → Copy all  
→ In n8n: New → Import from Clipboard

 2. Setup Credentials

 1. Token Auth (Custom Auth)
- Name: `Adobe API`
- Type: Custom Auth
```json
{
  "headers": {
    "Content-Type": "application/x-www-form-urlencoded"
  },
  "body": {
    "client_id": "YOUR_CLIENT_ID",
    "client_secret": "YOUR_CLIENT_SECRET"
  }
}
Made by Tahir khan
