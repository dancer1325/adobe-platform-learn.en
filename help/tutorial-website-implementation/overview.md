---
title: Implement the Experience Cloud in Websites with Tags
description: Implement the Experience Cloud in Websites with Tags is the perfect starting point for front-end developers or technical marketers who want to learn how to implement the Adobe Experience Cloud solutions on their website.
recommendations: catalog, noDisplay
exl-id: 1b95f0b2-3062-49d1-9b0b-e6824a54008f
---
# Overview

* goal
  * _Implement the Experience Cloud | Websites -- with -- Tags_
    * == how to implement Adobe Experience Cloud solutions | website
    * 👀== implement marketing solutions -- via -- tags | your own website 👀

* structure 
  * / EACH lesson 
    * how-to exercises 
    * foundational information

* steps
  * create a tag property
  * install a tag property | website
  * Add SOME Adobe Experience Cloud solutions
    * **[Adobe Experience Platform Identity Service](id-service.md)**
    * **[Adobe Target](target.md)**
    * **[Adobe Analytics](analytics.md)**
    * **[Adobe Audience Manager](audience-manager.md)**
  * create rules & data elements / send data -- to the -- Adobe solutions
  * Validate the implementation -- via -- Adobe Experience Cloud Debugger
  * Publish changes | SEVERAL environments (development, staging, and production) 

* Adobe Experience Platform Launch -- is being integrated into -- Adobe Experience Platform
  * -> SOME solutions are renamed
    * Platform Launch (Client Side) -- is renamed by -- **[[!DNL tags]](https://experienceleague.adobe.com/docs/experience-platform/tags/home.html)** 
    * Platform Launch Server Side -- is renamed by -- **[[!DNL event forwarding]](https://experienceleague.adobe.com/docs/experience-platform/tags/event-forwarding/overview.html)** 
    * Edge configurations -- is renamed by -- **[[!DNL datastreams]](https://experienceleague.adobe.com/docs/experience-platform/edge/fundamentals/datastreams.html)**

* == BUT DIFFERENT approach
  * / [Web SDK](../tutorial-web-sdk/overview.md)
  * / [Mobile SDK](../tutorial-mobile-sdk/overview.md)

## Prerequisites

* [demo Luma site](https://luma.enablementadobe.com/content/luma/us/en.html)
  [![Luma website](images/overview-luma.png)](https://luma.enablementadobe.com/content/luma/us/en.html)
* [rights -- to -- Develop, Approve, Publish, Manage Extensions, and Manage Environments](https://experienceleague.adobe.com/docs/experience-platform/tags/admin/user-permissions.html)
* ABOUT
  * Adobe Analytics, you must know
    * your tracking server
    * report suites / you will use
  * Audience Manager, you must know
    * your Audience Manager Subdomain (== "Partner Name" "Partner ID," or "Partner Subdomain")
* application-specific extensions
* libraries (AppMeasurement.js / Adobe Analytics & at.js / Adobe Target)
* Adobe Id

## Recommendations

1. use [Chrome Web Browser](https://www.google.com/chrome/)
   1. Reason: 🧠you will be using browser-specific extensions🧠 
2. add [Adobe Experience Platform Debugger](https://chromewebstore.google.com/detail/adobe-experience-platform/bfnnokhpnncpkdmbokanobigaccjkpob) extension | your Chrome browser
3. Copy the sample html page code

    +++Sample html page code
    
    ```html
    <!doctype html>
    <html lang="en">
    <head>
        <title>Tags: Sample HTML Page</title>
        <!--Preconnect and DNS-Prefetch to improve page load time. REPLACE "techmarketingdemos" WITH YOUR OWN AAM PARTNER ID, TARGET CLIENT CODE, AND ANALYTICS TRACKING SERVER-->
        <link rel="preconnect" href="//dpm.demdex.net">
        <link rel="preconnect" href="//fast.techmarketingdemos.demdex.net">
        <link rel="preconnect" href="//techmarketingdemos.demdex.net">
        <link rel="preconnect" href="//cm.everesttech.net">
        <link rel="preconnect" href="//techmarketingdemos.tt.omtrdc.net">
        <link rel="preconnect" href="//techmarketingdemos.sc.omtrdc.net">
        <link rel="dns-prefetch" href="//dpm.demdex.net">
        <link rel="dns-prefetch" href="//fast.techmarketingdemos.demdex.net">
        <link rel="dns-prefetch" href="//techmarketingdemos.demdex.net">
        <link rel="dns-prefetch" href="//cm.everesttech.net">
        <link rel="dns-prefetch" href="//techmarketingdemos.tt.omtrdc.net">
        <link rel="dns-prefetch" href="//techmarketingdemos.sc.omtrdc.net">
        <!--/Preconnect and DNS-Prefetch-->
        <!--Data Layer to enable rich data collection and targeting-->
        <script>
        var digitalData = {
            "page": {
                "pageInfo" : {
                    "pageName": "Home"
                    }
                }
        };
        </script>
        <!--/Data Layer-->
        <!--jQuery or other helper libraries-->
        <script src="https://code.jquery.com/jquery-3.3.1.min.js"></script>
        <!--/jQuery-->
        <!--Tags Header Embed Code: REPLACE THE NEXT LINE WITH THE EMBED CODE FROM YOUR OWN DEVELOPMENT ENVIRONMENT-->
        <script src="//assets.adobedtm.com/launch-EN93497c30fdf0424eb678d5f4ffac66dc.min.js" async></script>
        <!--/Tags Header Embed Code-->
    </head>
    <body>
        <h1>Tags: Sample HTML Page</h1>
        <p>This is a very simple page to demonstrate basic implementation concepts of Tags</p>
        <p>See <a href="https://docs.adobe.com/content/help/en/experience-cloud/implementing-in-websites-with-launch/index.html">Implementing the Experience Cloud in Websites with Tags</a> for the complete tutorial</p>
    </body>
    </html>

    ```

    +++

[Next "Create a tag property" >](create-a-property.md)
