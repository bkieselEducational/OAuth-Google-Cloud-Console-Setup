# OAuth-Google-Cloud-Console-Setup

## Step 1: Create an account

## Step 2: Create a Project.
As you will want to setup a new project everytime that you incorporate Google OAuth into one of your applications, using the name of your application as the Google Project name is probably a straightforward naming convention.

<img width="1577" alt="oauth_landing" src="https://github.com/bkieselEducational/OAuth-Google-Cloud-Console-Setup/assets/131717897/4e40366f-76e0-40cd-9703-3d7cea9ed920">


## Step 3: Configure the OAuth Consent Screen
i. Click on the APIs and Services tile depicted above<br>
ii. Then, in the Navbar on the left, click on OAuth Consent Screen.<br>
iii. Once there, you will want to select a "User Type". In our case, we want to select the option "External" and then click the CREATE button below.<br>
<br>
<img width="916" alt="oauth_consent_type2" src="https://github.com/bkieselEducational/OAuth-Google-Cloud-Console-Setup/assets/131717897/58a2f6e0-c4c2-407d-bf68-eb4ecbdaed0b"><br>
<br>
iv. On the following screen (depicted below), we must enter some more data. The first piece of data is our App name. Followed by a User support email (our GCP user email is a fine choice.) and then all the way at the bottom, you will want to enter your Developer contact information (again, probably your GCP user email.). When you've done all of that, click SAVE AND CONTINUE at the bottom.<br>
<br>
<img width="1565" alt="consent" src="https://github.com/bkieselEducational/OAuth-Google-Cloud-Console-Setup/assets/131717897/aaabbc0c-f432-4c77-8318-bd3fdbb013fc"><br>
<br>
v. On the following page Scopes (depicted below), we do not need to make any changes here. We can simply click the SAVE AND CONTINUE button and continue our journey.<br>
<br>
<img width="1293" alt="oauth_scopes_screen" src="https://github.com/bkieselEducational/OAuth-Google-Cloud-Console-Setup/assets/131717897/daa6f679-8486-424c-845e-57d68a2add29"><br>
<br>
vi. Now on the Test User screen (depicted below) we must authorize a test user who can access the API on behalf of our app. Click the + ADD USERS button, which will open up a sidebar on the right of the screen. Within that sidebar you can now enter the email for your test user (Again, your GCP user is a good candidate!) and then click the blue ADD button. If things have gone well, you should see your user's email in the list of Test Users back on the left side of the screen. Click the SAVE AND CONTINUE button to proceed!<br>
<br>
<img width="1483" alt="oauth_test_user_entry" src="https://github.com/bkieselEducational/OAuth-Google-Cloud-Console-Setup/assets/131717897/6006ac30-ab3b-4e9f-acfa-fce2e2416f47"><br>
<br>
<img width="1345" alt="oauth_test_user_after" src="https://github.com/bkieselEducational/OAuth-Google-Cloud-Console-Setup/assets/131717897/a9a919f7-37e5-4041-844c-676630226d11"><br>
<br>
vii. The Summary page (depicted below) is just that! A summary!! Unless you will be adding things, such as an application Logo, etc. feel free to click the BACK TO DASHBOARD button at the bottom!<br>
<br>
<img width="1361" alt="oauth_consent_back_to_dash" src="https://github.com/bkieselEducational/OAuth-Google-Cloud-Console-Setup/assets/131717897/e1e2c4ab-c9a8-4d2a-af23-63ddb3d5482b"><br>
<br>
## Step 4: Client Credentials

i. Now click the Credentials button in the navbar on the left and then click the + CREATE CREDENTIALS button that appears at the top of the resultant screen.<br>
<br>
<img width="1572" alt="to_credentials" src="https://github.com/bkieselEducational/OAuth-Google-Cloud-Console-Setup/assets/131717897/6fc39252-cca8-4ada-89cc-3aeab525ec5d"><br>
<br>

ii. You should now see a drop-down menu displayed (as depicted below). Click the option OAuth Client ID.<br>
<br>
<img width="447" alt="credentials_dropdown" src="https://github.com/bkieselEducational/OAuth-Google-Cloud-Console-Setup/assets/131717897/22ec2807-9e5e-4399-9d55-e530b677fc73"><br>
<br>
iii. At this point you should be seeing the Create OAuth Client ID for Web Application page and will have some inputs to fill out. Firstly, from the drop-down menu at the top, select the Application Type, which should be set to the first option in the list Web Application.<br>
iv. Next, move down to the next box and give your Application a Name.<br>
v. Unless you are managing the OAuth from your client side Javascript code (Not Recommended), there is no reason to fill out the "Authorized Javascript Origins". You can go down to the Authorized Redirect URIs and make two entries there. the first should use localhost as the domain so that you can test locally. The other should use your Render domain so that OAuth will also work in production!<br>
<br>
<img width="1577" alt="client_credentials" src="https://github.com/bkieselEducational/OAuth-Google-Cloud-Console-Setup/assets/131717897/68a85732-074b-43dc-a4c0-cc9d1774ee07"><br>
<br>
vi. And finally, click the blue SAVE button down at the bottom of the page and you should now see a modal with your credentials in it. Save them somewhere safe (.env file, etc.) and you should be ready to move on to your application code! Congratulations on survivng the drudgery of the Google Cloud Console!!<br>
<br>
<img width="509" alt="credentials" src="https://github.com/bkieselEducational/OAuth-Google-Cloud-Console-Setup/assets/131717897/23fa0f2c-4fe3-44fa-a48a-3c909b2e94c0">




