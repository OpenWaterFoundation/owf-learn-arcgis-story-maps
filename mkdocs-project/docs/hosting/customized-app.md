# Learn ArcGIS Story Maps / Hosting a Customized Story Map #

**To be completed.  Notes below need to be added somewhere in the text.**


The source code comes with documentation on how to build a compiled version of the code; developers must 
do this to build a deployable version of the customized Story Map.

You can run the app from your local machine from the source code while developing your customized Story 
Map, but you should never deploy the source code to a production web server for the following reasons:

* Your Story Map will take longer to load and run slower since the code isn't minified or optimized

* Readers may see an *Edit* button when viewing the Story Map that would let them open it in Builder 
(they would not be able to save changes though)

* Your custom code will be exposed since the JavaScript isn't obfuscated
