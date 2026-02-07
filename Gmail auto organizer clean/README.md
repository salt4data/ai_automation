# Email Organization Automation 
# An n8n workflow that automatically classifies and organizes Gmail emails into folders.


![image alt](https://github.com/salt4data/ai_automation/blob/main/Gmail%20auto%20organizer%20clean/gmail_automation.png)

## 💡 Why I Built This
Email mismanagement can quietly undermine reliability and coordination in professional settings. Important follow ups and time sensitive messages can easily get buried.

This project creates structure without removing control. Automation supports organization and drafting, but the human remains in the lead and fully accountable for every reply.

The goal is simple: reduce friction, protect opportunities, and communicate with intention.

## Email Categories

### Job Search
- **Job Alerts** - Job posting notifications from LinkedIn, Indeed, Glassdoor, ZipRecruiter
- **Job Applications & Feedback** - Application confirmations and recruiter responses

### Organizations
- **Black Wallet** - All emails mentioning Black Wallet (including Otter.ai meeting recordings)
- **BDPA** - All emails mentioning BDPA (including Otter.ai meeting recordings)

### Other Categories
- **Financial** - Bills, invoices, bank statements, spending statements, financial documents from banks or service providers
- **God/Faith** - Church, Bible studies, devotionals, prayer requests
- **Newsletters** - Emails with unsubscribe links
- **Social Media** - Facebook, LinkedIn, Twitter, Instagram notifications
- **Shopping** - Amazon, eBay, receipts, order confirmations
- **Promotions** - Sales, deals, discounts

### Smart Draft Responses
Emails requiring a reply automatically get an AI-generated draft response saved in Gmail drafts for review before sending.
- AI analyzes the email content
- Generates a professional, contextual draft response
- Saves draft in Gmail (email stays in inbox for visibility)
- Ready for review and editing before sending

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
- Existing emails require a manual run or a separate cleanup workflow
- Draft responses are saved but not sent automatically
