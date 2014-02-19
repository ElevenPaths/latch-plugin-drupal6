﻿#LATCH INSTALLATION GUIDE FOR DRUPAL 6


##PREREQUISITES 
 * Drupal version 6.

 * Curl extensions active in PHP (uncomment **"extension=php_curl.dll"** or **"extension=curl.so"** in Windows or Linux php.ini respectively). 

 * To get the **"Application ID"** and **"Secret"**, (fundamental values for integrating Latch in any application), it’s necessary to register a developer account in [Latch's website](https://latch.elevenpaths.com"https://latch.elevenpaths.com"). On the upper right side, click on "Developer area".
 

##DOWNLOADING THE DRUPAL 6 PLUGIN
 * When the account is activated, the user will be able to create applications with Latch and access to developer documentation, including existing SDKs and plugins. The user has to access again to [Developer area](https://latch.elevenpaths.com/www/developerArea"https://latch.elevenpaths.com/www/developerArea"), and browse his applications from **"My applications"** section in the side menu.

* When creating an application, two fundamental fields are shown: **"Application ID"** and **"Secret"**, keep these for later use. There are some additional parameters to be chosen, as the application icon (that will be shown in Latch) and whether the application will support OTP  (One Time Password) or not.

* From the side menu in developers area, the user can access the **"Documentation & SDKs"** section. Inside it, there is a **"SDKs and Plugins"** menu. Links to different SDKs in different programming languages and plugins developed so far, are shown.


##INSTALLING THE MODULE IN DRUPAL 6
* Once the administrator has downloaded the plugin, it has to be added as a module in its administration panel in Drupal 6. Unzip the downloaded plugin and place the whole content inside **"modules"**.

* Go to **"Modules"**, following this menu: **"Administer"-"Site building"-"Modules"**. At the bottom of the web, the just installed **"latch"** module will be shown. It has to be enabled.

* Introduce **"Application ID"** and **"Secret"** data, generated before. Got to Latch configuration (**"Administer"-"Site configuration"-"Latch Config"**) fill the form.

* A new **"Latch Account"** button will be shown under **"My Account**". The token generated by the Latch app will be added there.

* Go to **"Permissions"** (**"Administer"-"User management"-"Permissions"**). Latch are all under **"latch module"**. At least  **"pairing enabled"** option should be enabled corresponding to **"authenticated user"** permissions.


##UNINSTALLING THE MODULE IN DRUPAL 6
* Go to **"Modules"**, through **"Administer"-"Site building"-"Modules"**. Below, **"latch"** module will appear. Administrator has to disable unchecking **"Enabled"**, and save changes.

* From **"Modules"** go to **"Uninstall"**, and activate **"Uninstall"** option from Latch. Press **"Uninstall"** and press again on **"Uninstall"** to confirm.

* Latch is still in the module list, but **"Application ID"** and **"Secret"** have been removed, so if activating it again they will have to be introduced again.
