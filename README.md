# Recuiter-Response
Auto-reads new Gmail, detects real recruiter emails, drafts a polished reply with AI, and sends it for you.
Recruiter Response — n8n Workflow README

This guide walks a brand-new user through logging in to n8n, importing the provided workflow JSON, adding the required credentials, and testing the automation. No prior n8n experience needed.

1. Import the workflow
    1. Open your n8n Editor (Cloud, Desktop, or local).
    2. Click Workflows → Import from File/Clipboard.
    3. Paste or upload the Recruiter Response.json code.
    4. Click Save.
2. Add Gmail credentials:
    1. In the left menu, go to Credentials → New → Gmail OAuth2.
    2. Log in with your Gmail account and approve access.
    3. Name it (e.g., “Gmail account”).
    4. Go back to the workflow:
         - Open nodes like Gmail Trigger1, Get a message, Send a message2.
         - Select your Gmail credential from the Credentials dropdown.
         - Save each node.
4. Add AI credential:
   - If you want to use Google Gemini, also create a Google Gemini API credential in n8n and link it to the Google Gemini Chat Model nodes.
5. Activate the workflow
   - Toggle Active in the top-right corner.
   - The workflow will now check Gmail for unread recruiter emails and draft/send replies automatically.
  
