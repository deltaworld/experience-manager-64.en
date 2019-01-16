---
title: Authoring a Page for Mobile Devices
seo-title: Authoring a Page for Mobile Devices
description: null
seo-description: When authoring for mobile, you can switch between several emulators to see what the end-user sees
uuid: 2f56954a-eea4-4ab7-8f64-0bbf1b3b7fc0
contentOwner: Chris Bohnert
products: SG_EXPERIENCEMANAGER/6.4/SITES
content-type: reference
topic-tags: site-features
discoiquuid: bde75bfd-ad1e-4d31-88a2-be96a860446a
isreadyforlocalization: false
jcr-lastmodifiedby: remove-legacypath-6-1
index: y
internal: n
snippet: y
---

# Authoring a Page for Mobile Devices{#authoring-a-page-for-mobile-devices}

When authoring a mobile page, the page is displayed in a way that emulates the mobile device. When authoring the page, you can switch between several emulators to see what the end-user sees when accessing the page.

Devices are grouped into the categories feature, smart, and touch according to the capabilities of the devices to render a page. When the end-user accesses a mobile page, AEM detects the device and sends the representation that corresponds to its device group.

>[!NOTE]
>
>To create a mobile site based on an existing standard site, create a live copy of the standard site. (See [Creating a Live Copy for Different Channels](../../administering/using/msm-livecopy.md).)
>
>AEM developers can create new device groups. (See [Creating Device Group Filters](../../developing/using/groupfilters.md).)

Use the following procedure to author a mobile page:

1. From global navigation open the **Sites** console.
1. Open the page **We.Retail** -&gt; **United States ** -&gt; **English**.  

1. Switch to **Preview** mode.
1. Switch to the desired emulator by clicking the device icon at the top of the page.
1. Drag and drop components from the component browser to the page.

The page looks similar to the following:

![](assets/mobileipademu.png)

>[!NOTE]
>
>The emulators are disabled when a page on the author instance is requested from a mobile device.
