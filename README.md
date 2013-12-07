Apigee PhoneGap 3.2 Training (12/4/2013)
========================

Based on Apigee PhoneGap 3.2 Training in Atlanta (Steve Traut)


Prerequisites
- Node installed
- JDK installed (and in PATH)
- ANT installed (and in PATH)
- Android/Eclipse SDK
- PhoneGap installed (via Node)


Section 1
========================

App: List based app for Restaurants.  App connects to Cassandra database via Apigee account to pull a list of restaurants.  You can also add restaurants to the list and GeoLocation is used to sort this list based on proximity.


Technologies used: HTML5, Javascript, jQuery, jQueryMobile, CSS, JSON

Codiqa is a web-based interface to build the UI for the app.  After it is built, you can export the project to a jQuery Mobile project that you can manually edit.  There will be one index.html file that contains all the pages (as DIVs).




Section 2
========================

Apigee App Service (UserGrid OSS)
- Sign up for an Apigee account (j.mp/apigee-sign-up)
- Create app (data context, like a database)
- Create collections (like tables)
- Cassandra is an unstructured db (nosql)
- Download Apigee SDK (javascript) and add to project



Section 3
========================

Apigee's SDK uses Async Javascript to fetch data from Cassandra via web service calls.
Apigee service talks in JSON.



Section 4
========================

PhoneGap 3.2 Instruction
* Create PhoneGap Project

        phonegap create <foldername>  <com.domain.projectname>  <ProjectName>
* In this folder, there will be a www folder.  Delete all files/folders from www folder EXCEPT `config.xml`
* Paste your UI code here (css folder, js folder, index.html, etc)
* Homepage MUST be index.html (unless changed in config file)
* Change config.xml access to "*" for TESTING ONLY

                phonegap local build android  (You will probably have some issues here you will need to resolve)
                
* Goto platforms/android directory
* Import this into Eclipse
* Done
