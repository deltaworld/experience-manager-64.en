---
title: Authoring Mobile Applications
seo-title: Authoring Mobile Applications
description: he AEM Mobile Dashboard allows you to create, build and deploy your mobile application, create, delete and edit application metadata. Follow this page to learn more.
seo-description: he AEM Mobile Dashboard allows you to create, build and deploy your mobile application, create, delete and edit application metadata. Follow this page to learn more.
uuid: e3462050-90fa-4073-893a-151adeea55f9
contentOwner: User
content-type: reference
products: SG_EXPERIENCEMANAGER/6.4/MOBILE
topic-tags: authoring-adobe-phonegap-enterprise
discoiquuid: 24401495-d9c3-4bce-be7e-a92c5d7358ae
---

# Authoring Mobile Applications{#authoring-mobile-applications}

>[!NOTE]
>
>Adobe recommends using the SPA Editor for projects that require single page application framework-based client-side rendering (e.g. React). [Learn more](../../sites/developing/using/spa-overview.md).

The AEM Mobile Dashboard allows you to create, build and deploy your mobile application, create, delete and edit application metadata. Once your application is live, you can analyze application analytics including life cycle and usage metrics to improve customer conversion and brand loyalty. [](../../mobile/using/administer-phonegap.md)

To build your AEM Mobile Application, see the [Building Mobile Applications](../../mobile/using/building-app-mobile-phonegap.md) page.

To setup your environment and get started, see [Administering AEM to Use AEM PhoneGap Enterprise](../../mobile/using/administer-phonegap.md).

## The AEM Mobile Apps Catalog {#the-aem-mobile-apps-catalog}

The [AEM Mobile Apps Catalog](http://localhost:4502/aem/apps.html/content/phonegap) displays all of your mobile app managed in AEM.

Think of this catalog as the "landing page" for AEM Mobile, where administrators are able to start a new AEM Mobile application by either creating based off of a template, or uploading an existing app already started by a mobile developer.

Follow these steps to get to the apps catalog landing page:

1. Browse to **Navigation** and then choose **Mobile**.

1. Choose **Apps** to open the apps catalog.

![AEM Mobile Apps Catalog](assets/chlimage_1-140.png)

## The AEM Mobile App Dashboard {#the-aem-mobile-app-dashboard}

Selecting an AEM Mobile app from the catalog will display its dashboard. Here you can manage your application, view statistics, build, deploy and manage your mobile app content.

You can expand into each tile in the AEM Mobile Dashboard to view or edit details by clicking the '...' in the bottom right corner.

![AEM Mobile Applications Command Center](assets/chlimage_1-141.png)

### The Manage App Tile {#the-manage-app-tile}

The Manage App Tile displays your application icon, name, description, supported platforms, call home for updates URL and version information. You can drill into this tile to edit and maintain the PhoneGap Application Configuration (config.xml) and, prepare your application for submission to the varius application stores for distribution.

Click [here](../../mobile/using/phonegap-app-details-tile.md) for details.

![](assets/chlimage_1-142.png)

### The Manage Page Content Tile {#the-manage-page-content-tile}

Content can be created, updated and deleted in AEM Mobile in much the same way you do the same within AEM Sites. The **Manage Page Content Tile** displays the number of pages of managed content and last modified. You can drill-into content to create, copy, move, delete and update pages by clicking on each record in the tile. Once content has been updated, you can push a content update to your customers through the **Manage Content Packages Tile.**

![Content Tile](assets/chlimage_1-143.png)

### The Manage Content Packages Tile {#the-manage-content-packages-tile}

Once you have added or modified your content through the Manage Page Content Tile, you are able to push those changes out to your customers with a Content Release update.

Content Package allows the AEM App Author to manage page content in AEM and, have your development team make changes to your PhoneGap Shell Application (i.e. app framework or infrastructure) and then push those changes out to your customers quickly and without needing to enlist a developer to resubmit to the varios stores for distribution.

Content Package creates a ZIP file, considered a Content Release Package, for each update. These packages contain html resources and html pages that are generated while rendering the app and is intelligent enough to only package those files that have be modified since the last update.

The Manage Content Package Tile's **Type** column will display either 'App' to signify Application Shell content, for example framework or infrastructure of the app managed by a developer or, 'Content' which represents page content managed by the content author.

Content can be represented as a language or as a particular part of the app where multiple Content Release packages are consumed by the app. The choice of how you bundle your content is designed to be flexible and entirely up to how you want to manage content for your application.

The **Modified** column indicates when pages were most recently modified.

The **Staged** column shows when the last content update was created. To create a new content update and stage your changes open any record in the tile and create a new update.

The **Published** column shows when the last content update was published and made availble for consumption by your customers. To publish content, you must first stage that content and then publish the update by drilling into this tile and publishing from the Content Release details console.

![Content Release Tile](assets/chlimage_1-144.png) ![ContentSync package for the app shell](assets/chlimage_1-145.png)

This icon represents a Content Release package for the app shell

![](assets/chlimage_1-146.png)

These icons represents a Content Release package for app content

### The PhoneGap Build Tile {#the-phonegap-build-tile}

The **PhoneGap Build Tile** connects with [http://build.phonegap.com](http://build.phonegap.com) to build and host remote buids. Once built, the build is made available either as a download or directly to your device via a QR code.

Alternatively, you can download the device source to build locally through the [PhoneGap CLI](http://docs.phonegap.com/en/3.5.0/guide_cli_index.md.html).

![PhoneGap Build Tile](assets/chlimage_1-147.png)

### The Metrics Tile {#the-metrics-tile}

>[!CAUTION]
>
>The Metrics tile displays only after you configure the cloud service. 
>
>See [Configure your Adobe Mobile Services Cloud Service](../../mobile/using/configure-adobe-mobile-cloud-service.md) for details.

AEM Mobile integerates with Adobe Analytics through [Adobe Mobile Services SDK](http://www.adobe.com/ca/solutions/digital-marketing/mobile-services/app-sdk.html) (AMS).

The Control Center **Metrics Tile** displays summary analytics pulled from AMS for your application. You can drill into the analytics dashboard by clicking the '...' in the bottom right.

![Metrics Tile](assets/chlimage_1-148.png)

### The Manage Entity Content Tile {#the-manage-entity-content-tile}

The Manage Entity Content Tile allows you to add and manage app definitions. App definitions are a way to identify what spaces (and other configurations) are appropriate for the app. This way a new space can be added, without having to recompile the app. The app definition is updated and that will include the information for any new spaces.

Click [here](../../mobile/using/phonegap-app-definitions.md) to create and manage your app definitions.

You can drill into the manage entity content dashboard by clicking the '...' in the bottom right.

![](assets/chlimage_1-149.png)

#### Additional Resources {#additional-resources}

To learn about the roles and responsibilities of an Administrator and Developer, see the resources below:

* [Developing for Adobe PhoneGap Enterprise with AEM](../../mobile/using/developing-in-phonegap.md)
* [Administering Content for Adobe PhoneGap Enterprise with AEM](../../mobile/using/administer-phonegap.md)
