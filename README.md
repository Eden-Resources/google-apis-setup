# How to set up google APIs
1. Go to [google developers console](https://console.developers.google.com/)
2. Create a new project
3. Press `+ENABLE APIA AND SERVICES`
4. Search for the API(s) that you want to enable and enable them
5. Go to back to the project page
6. Click on `Credentials` on the left menu bar
7. Click `+CREATE CREDENTIALS`
8. Select `Service account`
9. Fill in the details (does not matter) and press `CREATE`
10. Chose the role by hovering over the drop down > Basic > Owner
11. Press `Continue`
12. Press `Done`
13. Now click into the new service account that you created in the Credentials page
14. Click on `Keys`, then `Add Key`, then `Create New Key`
15. Chose `JSON`, and click `Create`
16. Rename the JSON file that you just downloaded to `client-secret.json` and place it inside your bot's foler

# How to get the service account's adress
1. Open the JSON file that you just downloaded
2. The email is in line 6, like this: `"client_email": "<email>"`

# Additional steps for some APIs
## Google Sheets
### Getting the SHEET ID
1. Go to your google sheet document in your browser
2. The URL should look something like this: `https://docs.google.com/spreadsheets/d/<DOC-ID>`
3. Copy the ID in the URL and paste it in the `config.json`

### Sharing the document to the service account
1. Return to your google sheet document
2. Press `Share`
3. Share the document to the service account's adress and give it editor perms

## Google Vision 
1. Enable billing for your project [here](https://cloud.google.com/billing/docs/how-to/modify-project?visit_id=637510599696575187-2745866112&rd=1#enable-billing).
