1. How to fix the redirect_uri_mismatch
   If you already have a Client ID and Secret in your
   .env
   , follow these steps to fix the mismatch:

Go to the Google Cloud Console.
Select your project from the top dropdown.
Go to APIs & Services > Credentials.
Under OAuth 2.0 Client IDs, click the edit icon (pencil) for your Web Client.
Find the Authorized redirect URIs section.
Click ADD URI and paste: http://localhost:5000/api/v1/auth/google/callback
Click SAVE.
Wait about 1-2 minutes for the changes to propagate, then try logging in again. 2. How to create a NEW Google Client ID and Secret
If you need to create your own credentials from scratch, follow these steps:

Create a Project:
Go to Google Cloud Console.
Click the project dropdown at the top and select New Project. Name it (e.g., "JobSea").
Configure OAuth Consent Screen (Required before creating credentials):
Go to APIs & Services > OAuth consent screen.
Select External and click Create.
Fill in the required fields: App name, User support email, and Developer contact info.
Click Save and Continue through the next steps until you finish.
Create Credentials:
Go to APIs & Services > Credentials.
Click + Create Credentials at the top and select OAuth client ID.
Set Application type to Web application.
Under Authorized JavaScript origins, add: http://localhost:5000 (and http://localhost:3000 for the frontend).
Under Authorized redirect URIs, add: http://localhost:5000/api/v1/auth/google/callback
Click Create.
Update your
.env
:
Copy the Client ID and Client Secret from the popup.
Paste them into your
.env
file in the backend:
env
GOOGLE_CLIENT_ID=your_new_client_id
GOOGLE_CLIENT_SECRET=your_new_client_secret
GOOGLE_CALLBACK_URL=http://localhost:5000/api/v1/auth/google/callback
Restart your backend server (pnpm dev).
