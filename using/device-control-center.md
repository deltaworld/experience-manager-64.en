---
title: Device Control Center
seo-title: Device Control Center
description: null
seo-description: null
uuid: e91ebd67-a359-42f7-8351-2a1eb8cd6046
content-encoding: UTF-8
aemsrcnodepath: /content/help/en/experience-manager/6-4/sites/deploying/using/device-control-center
contentOwner: Jyotika syal
cq-designpath: /etc/designs/help
cq-lastmodified: 2018-04-30T03 26 49.184-0400
cq-lastmodifiedby: carlino
cq-lastreplicated: 2018-04-03T08 40 40.335-0400
cq-lastreplicatedby: carlino
cq-lastreplicationaction: Activate
content-type: reference
products: SG_EXPERIENCEMANAGER/6.4/SITES
cq-template: /apps/help/templates/article-3
discoiquuid: 77ef9e11-82f7-43ad-a209-94664be2bbba
firstPublishExternalDate: 2018-04-03T08:40:39.077-0400
isreadyforlocalization: false
jcr-created: 2017-12-01T19 07 20.192-0500
jcr-createdby: admin
jcr-ischeckedout: true
jcr-language: en_us
lastPublishExternalDate: 2018-04-03T08:40:39.077-0400
lochandoffdate: 2018-04-30T03 26 49.184-0400
lr-lastreplicatedby: carlino@adobe.com
mwpw-migration-script-version: 2017-10-12T21 46 58.665-0400
publishexternaldate: 2018-04-03T08 40 39.077-0400
publishExternalURL: https://helpx.adobe.com/experience-manager/6-4/sites/deploying/using/device-control-center.html
qaDate: 2017-10-12T21:46:58.665-0400
qaNotes: /content/docs/en/aem/6-3/administer/administering-screens/device-control-center
sha1: 5216342d45e0be03435518cbcd8337b0dc162e00
topicBrowsingSortDate: 2018-04-03T08:40:39.077-0400
index: y
internal: n
snippet: y
---

# Device Control Center

This section shows the different consoles available and how to achieve basic actions.

## Projects
The Screens Projects console is available by selecting the Adobe Experience Manager link (top left) and then Screens.

Alternatively, you can ﻿go directly to: [http://localhost:4502/screens.html/content/screens](http://localhost:4502/screens.html/content/screens)

![](assets/chlimage_1-76.png)

The Screens project is the top node of your project. Different projects could be differents brands, deployments, customers, and so on.

![](assets/chlimage_1-77.png)

To create a new Screens project:

1. Tap/click **Create**, a wizard will open.  

1. Select the required template and tap/click **Next**.

   ![](assets/chlimage_1-78.png)

1. Enter the properties as required and tap/click **Create**.

   ![](assets/chlimage_1-79.png)

   >[!NOTE]
   >
   >By default, the initial structure will contain the Applications, Channels, Devices and Locations master pages, but this can be manually adjusted if needed.

The project is created and it brings you back to the Screens Project console. You can now select your project.

In a project, there are four kind of folders:

* Applications
* Locations
* Channels
* Devices

![](assets/chlimage_1-80.png)

## Applications
The applications console allows you to preview the applications built for AEM Screens that will run on your display.

![](assets/chlimage_1-81.png)

For example, you can navigate to [http://localhost:4502/screens.html/content/screens/geometrixx/apps]( http://localhost:4502/screens.html/content/screens/geometrixx/apps) and select the **Preview **icon of the **Geometrixx Virtual Showroom Experience**.

The preview of the application should open in a new tab.

## Locations
The locations host the configuration of the displays according to where the various screens are.

![](assets/chlimage_1-82.png)

For an example of a configuration, navigate to [http://localhost:4502/screens/dashboard/display.html/content/screens/geometrixx/locations/demo/flagship/dual](http://localhost:4502/screens/dashboard/display.html/content/screens/geometrixx/locations/demo/flagship/dual).

![](assets/chlimage_1-83.png)

In the **Devices/Screens** section you see:

* What AEM Screens Player hardware and software is running. The heartbeat is active if the player is running. The version shown is the Firmware version. If a newer version is available on the server, there is an option to update the Firmware on the AEM Screens Player.
* The **eye icon** allows to play the content of the device on your local browser ("browser" or "web" version of the Firmware)
* The **camera icon** allows to create a remote screenshot.

**Assigned Channels** shows how the content is getting assigned to Displays. If you click the **pencil** icon of one channel, you'll see:

![](assets/chlimage_1-84.png)

You can configure:

* **Role**: any name
* **Channel**: browse one of the channels created
* **Supported Events**

    * **Initial Load**: will load this channel when the player is started. It can be assigned to multiple in combination with schedule
    * **Idle Screen**: is loaded when the screen is idle. It can be assigned to multiple in combination with schedule
    * **Timer**: needs to be set when a schedule is provided
    * **User Interaction**: will be loaded when the screen is touched

* **Schedule**: you can describe in text when the channel should appear. See [http://bunkat.github.io/later/parsers.html#text](http://bunkat.github.io/later/parsers.html#text) to know how to write.

* **Show Attraction Tooltip**: defines if the attraction tooltip ("Touch anywhere to begin") must be shown or not while the channel is running

>[!NOTE]
>
>By default, changes made here are live instantly.

### Creating a New Location
To create a new location:

1. Navigate to your Locations folder, for example [http://localhost:4502/screens.html/content/screens/sample/locations](http://localhost:4502/screens.html/content/screens/sample/locations).
1. Select the locations folder and tap/click **Create** next to the plus icon in the action bar. A wizard will open.

   ![](assets/chlimage_1-85.png)

1. Select the required template and tap/click **Next**.

   ![](assets/chlimage_1-86.png)

1. Enter the properties as required and tap/click **Create**.

   ![](assets/chlimage_1-87.png)

The location is created and added to your locations folder.

![](assets/chlimage_1-88.png)

### Creating a New Display
To create a new display:

1. Navigate to the appropriate location, for example [http://localhost:4502/screens.html/content/screens/sample/locations/sample-location](http://localhost:4502/screens.html/content/screens/sample/locations/sample-location).
1. Select your location folder and tap/click **Create** next to the plus icon in the action bar. A wizard will open.

   ![](assets/chlimage_1-89.png)

1. Select the required template and tap/click **Next**.

   ![](assets/chlimage_1-90.png)

1. Enter the properties as required and tap/click **Create**.

   ![](assets/chlimage_1-91.png)

The display is created and added to the location you chose.

![](assets/chlimage_1-92.png)

### Creating a New Device Config
To create a new device config:

1. Navigate to the appropriate display, for example [http://localhost:4502/screens.html/content/screens/sample/locations/sample-location/sample-display](http://localhost:4502/screens.html/content/screens/sample/locations/sample-location/sample-display).
1. Select your display folder and tap/click **View Dashboard** in the action bar.

   ![](assets/chlimage_1-93.png)

1. Tap/click the **+** button on the top right of the **Devices / Screens** panel.

   ![](assets/chlimage_1-94.png)

1. Select the required template and tap/click **Next**.

   ![](assets/chlimage_1-95.png)

1. Enter the properties as required and tap/click **Create**.

   ![](assets/chlimage_1-96.png)

The device config is created and added to the current display.

![](assets/chlimage_1-97.png)

### Channel assignment
To assign a channel to a display:

1. Navigate to the required display, for example [http://localhost:4502/screens.html/content/screens/sample/locations/sample-location/sample-display](http://localhost:4502/screens.html/content/screens/sample/locations/sample-location/sample-display).
1. Select the display folder and tap/click **View Dashboard **in the action bar.

   ![](assets/chlimage_1-98.png)

1. Tap/click the link button at the top right of the Assigned Channels panel.

   ![](assets/chlimage_1-99.png)

1. Enter the properties as required and tap/click **Save** button.

   ![](assets/chlimage_1-100.png)

The link to the channel should be created and added to the panel.

![](assets/chlimage_1-101.png)

## Channels
The channels will display a sequence of content.

The channels could display just some images, but they could also display an application.

![](assets/chlimage_1-102.png)

From the Channels console, you can preview your channel on your browser.

You can also open the Channel for authoring. For more information about authoring these channels, see [Screens Authoring Capabilites](/content/docs/en/aem/6-3/author/screens).

### Creating a New Channel
To create a new channel:

1. Navigate to your Channels folder, for example [http://localhost:4502/screens.html/content/screens/sample/channels](http://localhost:4502/screens.html/content/screens/sample/channels).
1. Select the channels folder and tap/click **Create** next to the plus icon in the action bar. A wizard will open.

   ![](assets/chlimage_1-103.png)

1. Select the required template and tap/click **Next**.

   ![](assets/chlimage_1-104.png)

1. Enter the properties as required and click **Create**.

   ![](assets/chlimage_1-105.png)

The channel is created and added to your channels folder.

![](assets/chlimage_1-106.png)

## Devices
The devices console allows you to access the device manager to assign your device to a display.

![](assets/chlimage_1-107.png)

>[!NOTE]
>
>Before assigning your device, you need to register it. For more information, see [Device Registration](/content/docs/en/aem/6-3/deploy/screens#Device Registration).

### Device Assignment
To assign your device to a display:

1. Navigate to the Devices folder of your project, for example [http://localhost:4502/screens.html/content/screens/sample/devices](http://localhost:4502/screens.html/content/screens/sample/devices).
1. Select your **Devices** folder and tap/click **Device Manager** in the action bar.

   ![](assets/chlimage_1-108.png)

1. Select an unassigned device from the list, and tap/click the **Assign Device** button in the action bar.

   ![](assets/chlimage_1-109.png)

1. Select the display you want to assign the device to from the list, and tap/click the **Assign** button

   ![](assets/chlimage_1-110.png)

1. Tap/click the **Finish** button to complete the assignment process.

   ![](assets/chlimage_1-111.png)

The display dashboard opens and you should see the device you just added.

![](assets/chlimage_1-112.png)

On your device, the player should automatically show the default channel for the display, for example an image if it is a sequence channel.

![](assets/chlimage_1-113.png)
