# Clickwrap test page

This project includes two HTML files, index.html and agree.html.

There is no application server for the files. The 
[GitHub pages](https://pages.github.com/) feature is used to
serve the pages. 

## index.html
The index.html file is a form to collect Clickwrap parameters. It makes a
GET request on the **agree.html** page. Since there is no 
application server, parameters are passed using the 
fragment (#) string.

### The Clickwrap parameters
1. **ClientUser ID** An id for the user. Can be the user's name, email,
   an id number in your user database, etc.
   
2. **Environment hostname** The hostname section of the DocuSign environment
   used for your account.

   Available from: your Clickwrap code popup window.

3. **Account ID** The DocuSign account for your Clickwrap.

   Available from: your Clickwrap code popup window.

3. **Clickwrap ID** The id of your Clickwrap.

   Available from: your Clickwrap code popup window.

## agree.html
The agree.html file is an example web page that loads the DocuSign
clickwrap SDK.

## Using the test page
Fill in the form, and click the button `Show the Clickwrap page`

**Remember** that the agreement ceremony is only shown once per 
ClientUser ID. To show the agreement ceremony again, either 
change the ClientUser ID or update the Clickwrap settings
on DocuSign.


## Support, Contributions, License

Submit support questions to [StackOverflow](https://stackoverflow.com). Use tag `docusignapi`.

Contributions via Pull Requests are appreciated.
All contributions must use the MIT License.

This repository uses the MIT license, see the
[LICENSE](https://github.com/docusign/eg-01-php-jwt/blob/master/LICENSE) file.
