---
title: Create a tag property
description: Learn how to log into the Data Collection interface and create a tag property. This lesson is part of the Implement the Experience Cloud in websites tutorial.
exl-id: f83d374a-a831-4598-b9d3-6f183224b589
---
# Create a tag property

* goal
  * configure & create your FIRST tag property
  * log | Data Collection UI

* tag property
  * == container / filled with 
    * extensions,
    * rules,
    * data elements,
    * libraries 
  * use cases
    * grouping >=1 domains & subdomains
      * _Example:_ track SAME assets | MULTIPLE websites

## Prerequisites

* [rights -- to -- Develop, Approve, Publish, Manage Extensions, and Manage Environments](https://experienceleague.adobe.com/docs/experience-platform/tags/admin/user-permissions.html)

## steps
### go | Data Collection interface

1. log | [Adobe Experience Cloud](https://experiencecloud.adobe.com)
2. click the ![Solution Switcher Icon](images/launch-solutionSwitcher.png), [!UICONTROL Launch/Data Collection]
  ![Open the solution switcher using the icon and click Launch/Data Collection](images/launch-solutionSwitcherActivation.png)
3. you should see the `Tags Properties` screen
   1. if NO properties have ever been created -> this screen is empty
     ![Properties Screen](images/launch-propertiesScreen.png)

### Create a Property
 
* see ["Companies and Properties"](https://experienceleague.adobe.com/docs/experience-platform/tags/admin/companies-and-properties.html)
* TODO:
**To Create a Property**

1. Click the **[!UICONTROL New Property]** button:

    ![Click New Property](images/launch-addNewProperty.png)

1. Name your property (e.g. `Luma Tutorial` or `Luma Tutorial - Daniel`)
1. As the domain, enter `enablementadobe.com` since this is the domain where the Luma demo site is hosted. Although the "Domain" field is required, the tag property will work on any domain where it's implemented. The main purpose of this field is to pre-populate menu options in the Rule builder.
1. Expand the **[!UICONTROL Advanced Options]** section and check the box to **[!UICONTROL Run rule components in sequence]**
1. Click the **[!UICONTROL Save]** button

   ![Create a new Property](images/launch-newProperty.png)

Your new property should display on the Properties page. Note that if you check the box next to the property name, options to **[!UICONTROL Configure]** or **[!UICONTROL Delete]** the property appear above the property list. Click on the name of your property (e.g. `Luma Tutorial`) to open the `Overview` screen.
![Click the name of the property to open it](images/launch-openProperty.png)

---

[Next "Add the Embed Code" >](add-embed-code.md)
