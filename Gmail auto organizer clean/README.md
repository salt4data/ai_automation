# Email Organization Automation

An n8n workflow that automatically classifies and organizes Gmail emails into folders.

## Overview
This workflow monitors my Gmail inbox and automatically sorts incoming emails into organized folders, keeping my primary inbox clean and manageable.

## Email Categories

### Job Search
- **Job Alerts** - Job posting notifications from LinkedIn, Indeed, Glassdoor, ZipRecruiter
- **Job Applications & Feedback** - Application confirmations and recruiter responses

### Organizations
- **Black Wallet** - All emails mentioning Black Wallet (including Otter.ai meeting recordings)
- **BDPA** - All emails mentioning BDPA (including Otter.ai meeting recordings)

### Other Categories
- **God/Faith** - Church, Bible studies, devotionals, prayer requests
- **Newsletters** - Emails with unsubscribe links
- **Social Media** - Facebook, LinkedIn, Twitter, Instagram notifications
- **Shopping** - Amazon, eBay, receipts, order confirmations
- **Promotions** - Sales, deals, discounts

### Smart Draft Responses
Emails requiring a reply automatically get an AI-generated draft response saved in Gmail drafts for review before sending.

## Setup

### Prerequisites
- n8n installed (cloud or self-hosted)
- Gmail account
- Gmail labels/folders created with the names above

### Installation
1. Import the workflow JSON file into n8n
2. Connect your Gmail account
3. Create the necessary Gmail labels
4. Activate the workflow

## How It Works
New Email Arrives
    ↓
Gmail Trigger Activates
    ↓
AI Analyzes Content & Sender
    ↓
Classification Logic Applied
    ↓
Email Moved to Appropriate Folder
    ↓
If Reply Needed → Generate Draft Response
    ↓
Draft Saved in Gmail

## Files
- `email-automation-workflow.json` - n8n workflow file
- `README.md` - This documentation

## Notes
- Workflow runs automatically on new emails
- Existing emails require manual run or separate cleanup workflow
- Draft responses are saved but not sent automatically
