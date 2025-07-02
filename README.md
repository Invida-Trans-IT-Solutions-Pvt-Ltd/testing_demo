# OCR Correction Labeling Project testing

## Overview

This repository contains examples for OCR document correction and labeling tasks. The goal is to correct and improve OCR-processed PDF documents to produce high-quality Markdown output.

## Repository Structure

Each `exemple X/` directory contains three files:

```
exemple X/
├── document.pdf     # Original source document
├── ocr-result.md   # OCR output with automated corrections
└── corrected.md    # Expected final corrected version
```

## File Descriptions

- **`document.pdf`**: Original reference document - the single source of truth
- **`ocr-result.md`**: OCR output with partial AI corrections, contains errors and missing data
- **`corrected.md`**: Target quality standard showing expected final result

## Common OCR Issues

### Missing Data
- Complete tables not OCR'd
- Missing table columns or rows
- Omitted contextual notes and annotations

### Value Errors
- Incorrect numbers, percentages, dates
- Misinterpreted text and terminology
- Wrong units (€ vs %, per day vs per year)

### Formatting Issues
- Malformed Markdown tables
- Inconsistent section organization
- Poor table alignment and structure

## Task Requirements

1. **Data Verification**: Compare all values against the original PDF
2. **Completeness**: Add missing tables, columns, rows, and contextual information
3. **Accuracy**: Correct all erroneous values and text
4. **Formatting**: Ensure proper Markdown syntax and table structure
5. **Quality Control**: Validate output using the provided preview tool

## Markdown Standards

- Use proper table syntax: `| Column 1 | Column 2 |`
- Maintain consistent header hierarchy (`###` for main sections)
- Include blank lines between sections
- Ensure all tables are properly aligned
- Transcribe all terms accurately from source documents

## Validation Tool

A Markdown preview tool is available for quality control. The following video demonstrates the correction interface and preview functionality:

<!-- markdownlint-disable MD033 -->
./app-demo.mp4
<!-- markdownlint-enable MD033 -->

**Important**: Always validate your work using the preview tool before submission.

## Quality Expectations

- All data must match the original PDF exactly
- No missing tables, columns, or contextual information
- Proper Markdown formatting throughout
- Professional presentation suitable for production use
