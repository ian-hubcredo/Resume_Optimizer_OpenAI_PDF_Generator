# Resume Optimizer - OpenAI + pdf.co

## Overview

A resume optimization pipeline using OpenAI and pdf.co. It accepts a resume (PDF or DOCX) via webhook, extracts the text, analyzes and improves the resume content using OpenAI, formats the optimized version to markdown, generates new PDF and DOCX documents via Gamma, downloads both formats, and emails the optimized resume with attachments. It handles both PDF and DOCX input formats with separate extraction paths.

## How It Works

```
Webhook (resume file) -> Detect format (PDF/DOCX) -> Extract text (pdf.co) -> OpenAI analyze + improve -> Format to Markdown -> Gamma create document -> Download PDF + DOCX -> Email with attachments
```

## Integrations

- **OpenAI** - Resume analysis and improvement
- **pdf.co** - PDF/DOCX text extraction
- **Gamma** - Document generation (PDF + DOCX)
- **Email** - Send optimized resume with attachments

## Setup

1. Import `Resume_Optimizer_OpenAI_pdf_co.json` into your n8n instance.
2. Configure OpenAI credentials and pdf.co API key.
3. Activate and send POST requests with resume files.
