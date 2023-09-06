Colectica Portal Localization Starter Kit
==========================================

This project contains resource files for all the text used in the
Colectica Portal user interface.

To translate these resources to a new language, follow these steps.

1. In the DdiItemStrings project, rename the ``DdiItemStrings.en-US.resx`` file with the appropriate language.
   For example, if you are translating to French, you can rename the file to ``DdiItemStrings.fr.resx``.

2. In the PortalStrings project, rename the ``PortalStrings.en-US.resx`` file with the appropriate language.
   For example, if you are translating to French, you can rename the file to ``PortalStrings.fr.resx``.

3. Edit the text in the resource files with your translations. If you want to keep
   the default text for any given string, simply delete the entry. Colectica Portal
   will fall back to the English text that is bundled with the application.

4. Build the two projects using `dotnet` or `msbuild`.
   This should create files named ``bin/Debug/net6.0/{lang}/ColecticaRepository.resources.dll`` and ``bin/Debug/net6.0/{lang}/Algenta.Colectica.Model.Ddi.resources.dll``.

5. To test your localized resources: 

   1. Create a folder inside your Colectica Repository deployment directory. 
      The folder should have the same name as your language (e.g., ``fr`` for French).

   2. Copy the two ``*.resources.dll`` files into this folder.

   3. Restart the Colectica Portal application in IIS.
