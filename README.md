# languagetool-examples
This repository contains a few sample rules for the LanguageTool grammar checker (https://languagetool.org/)

To use these rules in your LanguageTool installation, complete the following steps.

 * Download the 'languagetool-examples.xml' file.
 * Navigate to <your-LanguageTool-install-directory>/org/languagetool/rules/en/
 * Open the grammar.xml file in an editor.
 * Find the DOCTYPE definition (<!DOCTYPE rules), and add a new entity:

        <!ENTITY myrules "org/languagetool/rules/en/myrules.xml">

   Note that the path must be relative to the location of the languagetool.jar file.
 * Include the following line under the line that begins with <rules lang=

        &myrules;

 * Restart LanguageTool.
