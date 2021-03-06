Apigee PhoneGap 3.2 Training (12/4/2013)
========================

Based on Apigee PhoneGap 3.2 Training in Atlanta (Steve Traut)


Prerequisites
- Node installed (should place it in the PATH)
- JDK installed (and \bin in PATH)
- ANT installed (and \bin in PATH)
- Android/Eclipse SDK (and Android\sdk\tools directory in PATH)
- PhoneGap installed (via Node)
- Pre-requisites: https://dl.dropboxusercontent.com/u/348446/trainings/android.html
- Steve Traut reference app: https://github.com/stevetraut/training/tree/master/restaurant_app_1


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
* Apigee Documentation:  http://apigee.com/docs/



Section 4
========================

PhoneGap 3.2 Instruction

1. Create PhoneGap Project

        phonegap create <foldername>  <com.domain.projectname>  <ProjectName>
2. In this folder, there will be a www folder.  Delete all files/folders from www folder EXCEPT config.xml
3. Paste your UI code here (css folder, js folder, index.html, etc)
4. Homepage MUST be index.html (unless changed in config file)
5. Change config.xml access to "*" for TESTING ONLY
6. Build the Project in your platform (You will probably have some issues here you will need to resolve)

        phonegap local build android  
7. Goto platforms/android directory
8. Import this into Eclipse
9. Done






