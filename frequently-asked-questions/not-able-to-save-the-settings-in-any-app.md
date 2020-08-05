# Unable to save the settings in any app

If you are not able to save the settings at the backend of the site, it might be because of the following reasons:

* Database type 
* Browser 

## Database type: <a id="database-type"></a>

Please make sure that you have set the Database type as MySQLi and not MySQL\(PDO\).

MySQLi is the supported database type.

You could check this under System-&gt;Global configuration-&gt;Server tab-&gt;Database type.

![Database type in Joomla configuration](https://raw.githubusercontent.com/j2store/doc-images/master/frequently-asked-questions/not-able-to-save-settings/database-type.png)

## Browser type: <a id="browser-type"></a>

Please make sure that the browser you are using is not Safari.

There is a joomla issue while trying to save settings with Safari.

There has been an issue in the core.js file of Joomla which causes this issue.

We have this issue raised in the Joomla forum and we are yet to receive a solution for this concern.

If issue prevails, you could reach us through the [support form](https://www.j2store.org/support/support-request-form.html) or [ticket system](https://www.j2store.org/my-account/priority-ticket-system.html) available for PRO users.

