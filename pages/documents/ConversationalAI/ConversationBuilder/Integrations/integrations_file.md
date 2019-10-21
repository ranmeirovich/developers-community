---
pagename: File integrations
Keywords:
sitesection: Documents
categoryname: "Conversational AI"
documentname: Conversation Builder
subfoldername: Integrations
permalink: conversation-builder-integrations-file-integrations.html
indicator: both
---

File integrations support the ability of consumers to upload files that you require.

In the dialog, first, you add a [File Upload](conversation-builder-interactions-integrations.html#file-upload-integrations) interaction; it handles upload of the file to LiveEngage. Second, you immediately follow the File Upload interaction with an Integration interaction that invokes a *File integration* in particular. It's this second interaction that performs the work of taking the file in the LiveEngage environment and uploading it to your external file share or system.

<img class="fancyimage" style="width:550px" src="img/ConvoBuilder/integrations_file.png">

**To add a File integration**

1. Open the bot, and click **Integrations** in the upper-right corner.
2. Configure the integration settings (required fields are marked with asterisks):
    - **Integration Name**: Enter the name of integration. Enter a name that's meaningful (it describes well the integration's purpose), concise, and follows a consistent pattern. This helps with organization, and it makes it easier for bot developers to work with the integration during bot development.
    - **Response Data Variable Name**: Enter the name of the response data variable.
    - **Integration Type**: Select **File**.
    - **Method**: Select the type of HTTP request method. PUT and POST are industry standards and commonly used.
    - **URL**: Enter the request target, i.e., the URL for your external upload service that can accept the file stream.
    - **Credential**: Select the [credential](bot-accounts-credentials.html) to use for authentication if applicable. The bot will automatically enhance the request based on the credential's type and data.
    - **Request Headers**: Add any message headers to include in the request.
    - **Request Parameters**: Add the request parameters to pass in the URL’s query string.
    - **Post Body**: Enter the payload to send.
    - **Transform Result Script**: If applicable, use this section to write JavaScript code that transforms the raw result (typically in JSON format), so you can use the information in the bot's dialog. For more on this, see [Transform an API result](conversation-builder-integrations-integration-basics.html#transform-an-api-result).
    - **Custom Data Fields**: Add the fields that will store the result data in key/value pairs. Users who are tasked with creating bots can use and display this data in interactions by referencing these fields as described [here](conversation-builder-interactions-interaction-basics.html#display-variables-in-interactions).
3. Click **Save**.