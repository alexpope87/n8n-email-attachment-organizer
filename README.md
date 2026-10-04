# n8n Email Attachment Organizer

A simple n8n automation that automatically organizes Gmail attachments into Google Drive folders based on file type.

## Problem

Email attachments often need to be downloaded and manually organized into folders.

The goal of this project was to automate that process.

## Workflow

1. Gmail Trigger detects new emails with attachments.
2. Attachments are downloaded as binary files.
3. A Switch node checks the file type.
4. Files are routed automatically to the correct Google Drive folder.

## File Routing

- PDF → PDFs
- JPG / JPEG / PNG → Images
- XLS / XLSX / CSV → Spreadsheets

## Workflow

![n8n Attachment Organizer](workflow.png)

## Tech Stack

- n8n
- Gmail
- Google Drive

## Key Concepts Practiced

- Event-driven workflows
- Binary file handling
- Conditional routing
- MIME type and file extension detection
- Google Drive integration

## Result

Incoming email attachments are automatically categorized and saved in the appropriate Google Drive folder.

## Security

Authentication credentials and private Google Drive folder IDs are not included in this repository.
