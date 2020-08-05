# App for J2store

In the following guide, we are going to cover the following topics related to plugin development:

Introduction App Structure Naming Conventions The Manifest Creating app class App Model Class App controller

## Introduction <a id="introduction"></a>

Developing a app for J2Store is very simple process if you are good in PHP and the Joomla MVC structure.

J2Store comes with a app library and wrappers that makes creating a app for J2Store.

## App Structure <a id="app-structure"></a>

There is a folder structure and a few naming conventions, that should be followed during the development of a app for J2Store.

A typical app should look like this:

```text
├── app_example/
│   ├── app_example.php
│   ├── app_example.xml
│   ├── languages/
│   │   ├── en-GB.plg_j2store_app_example.ini
│   ├── app_example/
│   │   ├── tmpl/
│   │   │   ├── form.php
│   │   │   ├── default.php
│   │   ├── controller.php
│   │   ├── models/
│   │   │   ├── appexample.php
```

## Naming Conventions <a id="naming-conventions"></a>

The name of the app folder should start with the prefix “app_”. Otherwise, J2Store will not recognise your app. So our example app is named as:app_example

Make sure that the name of the file and folder is in lower case and there are no spaces or any other characters in the name.

## Manifest <a id="manifest"></a>

An example manifest should look like this:



```text
<?xml version="1.0" encoding="utf-8"?>
<extension version="3.0" type="plugin" group="j2store" method="upgrade">
	<name>Example</name>
	<version>1.0</version>
	<creationDate>July 2015</creationDate>
	<author>J2Store</author>
	<authorEmail>supports@j2store.org</authorEmail>
	<authorUrl>http://www.j2store.org</authorUrl>
	<copyright>2015 Weblogicx India</copyright>
	<license>GNU General Public License v2</license>
	<description>PLG_J2STORE_APP_DONATION_DESC</description>
	<files>
		<filename plugin="app_example">app_example.php</filename>
		<folder>app_example</folder>
		<folder>languages</folder>		
		<filename>index.html</filename>
	</files>
	<languages>
		<language tag="en-GB">languages/en-GB.plg_j2store_app_example.ini</language>		
	</languages>
	<config>
		<fields name="params">
			<fieldset name="basic" label="J2STORE_BASIC_SETTINGS" 
				addfieldpath="/administrator/components/com_j2store/models/fields">		
			
			</fieldset>
		</fields>
	</config>		
</extension>
```

## Creating app class <a id="creating-app-class"></a>

Make sure the name of the class suffix is same as your app file’s name. And it should extend the J2StoreAppPlugin class.

```text
defined('_JEXEC') or die('Restricted access');
    require_once(JPATH_ADMINISTRATOR.'/components/com_j2store/library/plugins/app.php');
    class plgJ2StoreApp_Example extends J2StoreAppPlugin
    {
    	/**
    	 * @var $_element  string  Should always correspond with the plugin's filename,
    	 *                         forcing it to be unique
    	 */
    	var $_element    = 'app_example';```

This file should have following two methods:

**onJ2StoreGetAppView** - This method is used to check if it is a app_example or not.

viewList - A controller for this plugin.
	```$html = $this->_getLayout('default', $vars);```

The above line will call the template layout for the app_example from /app_example/app_example/tmpl/default.php

**App Model Class**

App's model should have file named with appexample.php and it should be like below
```

defined\(’_JEXEC’\) or die\(‘Restricted access’\); require_once \(JPATH_ADMINISTRATOR . ‘/components/com_j2store/library/appmodel.php’\); class J2StoreModelAppExample extends J2StoreAppModel {

```text
public $_element = 'app_example';
```

}

```text
**App controller**

Controller.php file should be located in /app_donation/app_donation/controller.php and you must include the J2Store's library appcontroller and it should be written like below
```

defined\(’_JEXEC’\) or die\(‘Restricted access’\); require_once\(JPATH_ADMINISTRATOR.’/components/com_j2store/library/appcontroller.php’\);

class J2StoreControllerAppexample extends J2StoreAppController{

```text
var $_element   = 'app_example';
```

}

