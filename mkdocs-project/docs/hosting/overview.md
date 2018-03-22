# Learn ArcGIS Story Maps / Hosting Your Own Story Map #
Story Maps are open source.  This means you can download the code for any Story Map app for free from 
[GitHub](https://github.com/Esri?q=Storytelling), host it on your own server and perform further 
customization of the Story Map.  In this section we'll discuss why you might want to host your own Story 
Map, how the app works when it runs on your server and instructions for hosting your own Story Map.

This section is adapted from [this](https://developerscorner.storymaps.arcgis.com/an-introduction-to-hosting-your-own-story-map-e2450181ad2f) 
Esri article.

## Reasons for Hosting Your Own Story Map ##
There are several reasons or benefits to hosting your own Story Map app on your own server:

* You can give your story a custom URL on your organization's domain
* You can set up web analytics to obtain statistics about who's reading the story
* You can enhance how your story looks when it's shared on social networking sites
* You can style the story to change its appearance beyond what is possible in the Story Map Builder 
(as long as you know HTML and CSS)
* You can customize the story to add new features, such as background audio or a cover page.  Esri's 
[developer blog](https://developerscorner.storymaps.arcgis.com/) has many articles about how to make 
specific customizations

**If you choose to host your own story map, it is highly recommended that your hosting environment 
supports secure web standards (https rather than http).**

------------------
## How the App Works When it Runs on Your Server ##
When you host a Story Map on your own server, you only host the app code; your story content is still 
hosted on ArcGIS Online.  Story content is saved in ArcGIS as a web mapping application item that has 
a unique ID.  The ID is the number that can be seen in the URL when you are viewing a Story Map, for 
example:  
``https://www.arcgis.com/apps/MapSeries/index.html?appid=5664b970f6154193a1dab3b5d4f27336``  
The Story Map app requires a parameter called the appid.  By specifying an appid in your hosted story 
you're letting it know what story you want it to load.  When a reader opens a link to your story, the 
app code is loaded into their browser from your server.  Then the appid you've specified in the code is 
used to find and load the story's content from ArcGIS.

------------------
## Source Code vs. Compiled Code ##
There are two versions of code available to download from GitHub for each Story Map app:  source code 
and compiled code.

* **Source code** - what a developer needs to customize a Story Map app.  The best way to get the code 
is to clone or fork it from GitHub.  By doing this you'll also be notified of any updates made to the 
code by Esri.  
* **Compiled code** - also called minified code; is an optimized version of the source code and is what 
you should use to deploy the app to your web server.  If you only plan to make style changes to your Story 
Map, you should download the compiled code.  This will be discussed in greater detail in later subsections.

------------------
## Hosting Scenarios ##
There are three common situations in which a person may desire to self-host a Story Map app:

* A person may want to simply host the app on their own server without making any additional changes to 
the app  
* A person may want to change the style of the app beyond what is possible in the builder  
* A person may want to customize the app further by adding new features

We will discuss each scenario in subsequent subsections and provide step-by-step instructions for how to 
host an app and get it running under each scenario.

**Regardless of which scenario is chosen, the Story Map must first be built via the Story Maps Builder. 
This is because the Story Map must have a unique ID, which can only be created using the Builder.**

------------------
## Next Steps ##
The next step is to host our previously created Story Map on our own server without making any changes 
to the Story Map.
