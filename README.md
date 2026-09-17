# OuraDataAnalysis

Personal tools for importing and reviewing my own Oura data. The existing Windows application stores data locally and synchronizes selected records to my Google Sheets. A separate Google Apps Script application, **Oura GAS Verification**, is being tested with another Google account that I own. Neither application is currently offered as a public service.

## Privacy Policy

The applications access Oura data only after my explicit authorization. The Windows application stores OAuth credentials locally in a .env file excluded from version control and stores retrieved records locally. Selected health records are synchronized to my own Google Sheets.

The GAS verification application requests Personal and Daily permissions to test daily and individual sleep record retrieval. Client credentials are stored in Apps Script Script Properties, and OAuth tokens are stored in User Properties. Google executes the script and processes these stored credentials and data. Properties are not a separate secret vault against project editors; access to the script and spreadsheet should be restricted to their owner.

The GAS test is intended to store selected daily and sleep records in a separate spreadsheet owned by my test Google account. Credentials and health records are not published in this repository. The GAS test does not send data to an AI service. If I separately choose to connect my spreadsheet to ChatGPT, the selected data will be processed by that service under its own settings and policies.

I can revoke Oura access at any time. To stop collection, I can also remove the Apps Script triggers. Stored records remain until I delete them from the relevant local storage, spreadsheet or Drive files; revoking access does not automatically delete previously collected data. I can remove stored credentials from local configuration or Apps Script properties.

## Terms of Service

These are personal, experimental tools provided as-is, without warranties of accuracy, reliability or availability. They are intended for personal reflection, not medical advice, diagnosis or treatment. They are not affiliated with or endorsed by Oura. Any future distribution will require separate review of the applicable terms and an updated description of the service.

## Contact

https://github.com/netsplaygames
