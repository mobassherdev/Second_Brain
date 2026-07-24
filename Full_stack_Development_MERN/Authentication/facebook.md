1. Facebook App ID and Secret Setup
   Setting up Facebook is very similar to Google. Here is the step-by-step guide:

Create a Meta Developer Account: Go to Meta for Developers and log in with your Facebook account.
Create an App:
Click My Apps > Create App.
Select Allow people to log in with their Facebook account (or "Consumer").
Give your app a name (e.g., "JobSea Local").
Get Credentials:
In the left sidebar, go to App Settings > Basic.
You will see your App ID and App Secret (click "Show").
Copy these into your .env:
env
FACEBOOK_APP_ID=your_facebook_app_id
FACEBOOK_APP_SECRET=your_facebook_app_secret
Add Website Platform:
Scroll to the bottom of the Basic Settings page.
Click + Add Platform and select Website.
Enter your backend URL: http://localhost:5000.
Click Save Changes.
Configure Facebook Login:
In the sidebar, click Dashboard or Add Product.
Find Facebook Login and click Set Up.
Go to Facebook Login > Settings (in the sidebar).
Under Valid OAuth Redirect URIs, paste: http://localhost:5000/api/v1/auth/facebook/callback
Click Save Changes. 2. Regarding the pnpm dev Output
I checked your terminal logs, and your server is actually running correctly!

The messages like 🐱‍🏍 globalErrorHandler ~~ message: Userr not found! are not a crash. They are simply logs from the "Forgot Password" feature we just updated.

Because we changed the logic to throw an error when a user doesn't exist, the server logs this error whenever someone tries an invalid email.
As long as you see Server running on port 5000, the application is healthy.
