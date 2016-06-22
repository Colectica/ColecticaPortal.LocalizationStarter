Colectica Portal Localization Starter Kit
==========================================

This project contains resource files for all the text used in the
Colectica Portal user interface.

To translate these resources to a new language, follow these steps.

1. Rename the two resource files with the appropriate language. For example, if
   you are translating to French, you can rename the two files in the Resources
   folder to `DdiItemStrings.fr.resx` and `PortalStrings.fr.resx`.

2. Edit the text in the resource files with your translations. If you want to keep
   the default text for any given string, simply delete the entry. Colectica Portal
   will fall back to the English text that is bundled with the application.

3. Build the project. This should create a file named 
   `bin\\Debug\\Colectica.Portal.resources.dll`.

4. To test your localized resources: 

   1. Create a folder inside your Colectica Portal deployment directory. 
      The folder should have the same name as your language (e.g., 
	  `fr` for French).

   2. Copy the `bin\\Debug\\Colectica.Portal.resources.dll` file into this 
      folder.

   3. Restart the Colectica Portal application in IIS.
