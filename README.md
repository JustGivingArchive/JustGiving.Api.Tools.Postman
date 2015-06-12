JustGiving.Api.Tools.Postman
changed on branch aa
============================

Configuration and Collection files for the [Postman Chrome app](https://chrome.google.com/webstore/detail/postman-rest-client/fdmmgilgnpjigdojojpjoooidkmcomcm?hl=en).

Importing the `*.postman_collection.json` files found here into Postman will add JustGiving API methods categorized by resource, aligning with the JustGiving [API documentation](https://api.justgiving.com/docs).

Additionally we have provided two environment config files, this will help you switch between sandbox and production environments quickly.

### Install Postman

[![available in the Chrome web store](https://developer.chrome.com/webstore/images/ChromeWebStore_Badge_v2_206x58.png)](https://chrome.google.com/webstore/detail/postman-rest-client/fdmmgilgnpjigdojojpjoooidkmcomcm?hl=en)

### Usage

1. Import collections into Postman **HINT:** Rather than dragging a single file at a time, click "Choose Files" and do multi-select (SHIFT-Click/CTRL-Click)
2. Import environments into Postman, click on the Environments drop down, select **Manage environments/Import/Choose Files** and select `sandbox.environment.config.justgiving.json` and `live.environment.config.justgiving.json`
3. Click **back** and do the following for both of the environments
  * Change `yourAppID` to be the applicationId you are using for that environment **HINT:** an applicationId will work in both Sandbox and Production but we recommend using a different applicationId in each environment
  * Change `yourBasicAuthToken` to be the base 64 encoded username/password combination of your login to the JustGiving website in that environment (not the credentials for https://apimanagement.justgiving.com). You can encode your credentials here: [https://api.justgiving.com/docs/usage#credsTo64Username](https://api.justgiving.com/docs/usage#credsTo64Username) **HINT:** Only use the actual encoded value, do not include "Basic " when replacing yourBasicAuthToken
4. Some methods include values that we can not pre-populate such as pageSize, in these cases you will see the parameter within single braces e.g. {email}, {charityId},{pageSize}, {pageId}, {pageShortName}   Replace with the value you require.
