---
title: Selecting your UI
seo-title: Selecting your UI
description: null
seo-description: Configure which interface you will use to work in AEM
uuid: 599a85a4-07d0-4dca-9384-0d0c2511d9ad
contentOwner: Chris Bohnert
products: SG_EXPERIENCEMANAGER/6.4/SITES
topic-tags: introduction
content-type: reference
discoiquuid: eaae13c2-370c-4568-a010-ef43aacfe6f9
isreadyforlocalization: false
jcr-lastmodifiedby: remove-legacypath-6-1
index: y
internal: n
snippet: y
---

# Selecting your UI{#selecting-your-ui}

Although the touch-enabled UI is now the standard UI and feature parity has been nearly reached with the administration and editing of sites, there may be times when the user wishes to switch to the [classic UI](../../classic-ui-authoring/using/classicui.md). There are several options for doing this.

>[!NOTE]
>
>For details on the status of feature parity with the classic UI, see the [Touch UI Feature Parity](/content/help/en/experience-manager/6-4/release-notes/touch-ui-features-status) document.

There are various locations where you can define which UI is to be used:

* [Configuring the default UI for your instance](#configuringthedefaultuiforyourinstance)  
  This will set the default UI to be shown at user login, although the user may be able to override this and select a different UI for their account or current session.  

* [Setting Classic UI Authoring for your account](../../authoring/using/select-ui.md#main-pars-title)  
  This will set the UI to be used as default when editing pages, although the user can override this and select a different UI for their account or current session.  

* [Switching to classic UI for the current session](#switchingtoclassicuiforthecurrentsession)  
  This switches to the classic UI for the current session.

* For the case of [page authoring the system makes certain overrides in the relation to the UI](#uioverridesfortheeditor).

>[!NOTE]
>
>Instances upgraded from a previous version will retain the classic UI for page authoring.
>
>After upgrade, page authoring will not be automatically switched to the touch-enabled UI, but you can configure this using the the [OSGi configuration](../../deploying/using/configuring-osgi.md) of the **WCM Authoring UI Mode Service** ( `AuthoringUIMode` service). See [UI Overrides for the Editor](#uioverridesfortheeditor).

## Configuring the Default UI for Your Instance {#configuring-the-default-ui-for-your-instance}

A system administrator can configure the UI that is seen at startup and login by using [Root Mapping](../../deploying/using/osgi-configuration-settings.md#daycqrootmapping).

This can be overridden by user defaults or session settings.

## Setting Classic UI Authoring for Your Account {#setting-classic-ui-authoring-for-your-account}

Each user can access his/her [user preferences](../../authoring/using/user-properties.md#userpreferences) to define if he/she wishes to use the classic UI for page authoring (instead of the default UI).

This can be overridden by session settings.

## Switching to Classic UI for the Current Session {#switching-to-classic-ui-for-the-current-session}

When using the touch-enabled UI desktop users might want to revert to the classic (desktop only) UI. There are several methods to switch to the classic UI for the current session:

* **Navigation Links**

  If required, a system administrator can enable the option **Classic UI** for various consoles in the global navigation. See the article [Enabling Access to Classic UI](../../administering/using/enable-classic-ui.md) for more information.

  If this is enabled, whenever you mouseover an applicable console, an icon appears (symbol of a monitor), tapping/clicking this will open the appropriate location in the classic UI.

  For examples, the links from **Sites** to **siteadmin**:

  ![](assets/screen_shot_2018-03-23at111924.png)

* **URL**

  The classic UI can be accessed using the URL for the welcome screen at `welcome.html`. For example:

  `http://localhost:4502/welcome.html`

  >[!NOTE]
  >
  >The touch-enabled UI can be accessed via `sites.html`. For example:
  >
  >
  >`http://localhost:4502/sites.html`

### Switching to Classic UI when Editing a Page {#switching-to-classic-ui-when-editing-a-page}

If required, a system administrator can enable the **Open the Classic UI** from the **Page Information** dialog. See the article [Enabling Access to Classic UI](../../administering/using/enable-classic-ui.md) for more information.

![](assets/chlimage_1-373.png)

### UI Overrides for the Editor {#ui-overrides-for-the-editor}

<!-- 

Comment Type: remark
Last Modified By: Alison Heimoz (aheimoz)
Last Modified Date: 2017-11-30T04:52:33.207-0500

<p>6.1 Review - is the info about cookies and their effects still valid?</p>

 -->

The settings defined by a user or system administrator can be overriden by the system in the case of page authoring.

* When authoring pages:

    * Use of the classic editor is forced when accessing the page using `cf#` in the URL. For example:  
      `http://localhost:4502/cf#/content/geometrixx/en/products/triangle.html`
    
    * Use of the touch-enabled editor is forced when using `/editor.html` in the URL or when using a touch device. For example:  
      `http://localhost:4502/editor.html/content/geometrixx/en/products/triangle.html`

* Any forcing is temporary and only valid for the browser session

    * A cookie set will be set dependent on whether touch-enabled ( `editor.html`) or classic ( `cf#`) is used.

* When opening pages through `siteadmin`, checks will be made for the existence of:

    * The cookie
    * A user preference  
    * If neither exist, it will default to the definitions set in the [OSGi configuration](../../deploying/using/configuring-osgi.md) of the **WCM Authoring UI Mode Service** ( `AuthoringUIMode` service).

>[!NOTE]
>
>If [a user has already defined a preference for page authoring](#settingthedefaultauthoringuiforyouraccount), that will not be overridden by changing the OSGi property.

>[!CAUTION]
>
>Due to the use of cookies, as already described, it is not recommended to either:
>
>* Manually edit the URL - A non-standard URL could result in an unknown situation and lack of functionality.
>* Have both editors open at the same time - For example, in separate windows.  
>
