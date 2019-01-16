---
title: Components Console
seo-title: Components Console
description: null
seo-description: null
uuid: 6ef0ed8e-e1e5-439c-8538-1d6cbbcede94
contentOwner: Chris Bohnert
products: SG_EXPERIENCEMANAGER/6.4/SITES
topic-tags: page-authoring
content-type: reference
discoiquuid: 8c06d184-c216-41a4-a937-67748c41950a
isreadyforlocalization: false
index: y
internal: n
snippet: y
---

# Components Console{#components-console}

The Components console allows you to browse through all components defined for your instance and view key information for each component.

It can be accessed from **Tools -&gt;** **General -&gt;** **Components**. In the console, card and list view are available. Because there is no tree structure for components, column view is not available.

![](assets/chlimage_1-374.png)

>[!NOTE]
>
>The Component Console shows all components in the system. The [Component Browser](../../authoring/using/author-environment-tools.md#main-pars-title-17) shows components that are available to authors and hides any component groups that begin with a period ( `.`).

### Search {#search}

With the **Content Only** icon (top left) you can open the **Search** panel to search and/or filter the components:

![](assets/chlimage_1-375.png) 

### Component Details {#component-details}

To view details about a specific component tap/click on the required resource. Three tabs provide:

* **Properties**

  ![](assets/screen_shot_2018-03-27at165847.png)

  On the Properties tab you can:

    * View the general properties of the component.  
    * View how the [icon or abbreviation has been defined](../../developing/using/components-basics.md#main-pars-title-4779) for the component.

        * Clicking the source of the icon will take you to that component.

    * View the **Resource Type** and **Resource Super Type** (if defined) for the component.

        * Clicking the Resource Super Type will take you to that component.

  >[!NOTE]
  >
  >Because `/apps` is not editable at runtime, the Components Console is read-only.

* **Policies**

  ![](assets/chlimage_1-376.png)

* **Live Usage**

  ![](assets/chlimage_1-377.png)

  >[!CAUTION]
  >
  >Due to the nature of the information being collected for this view, it can take a while to be collated/displayed.

* **Documentation**

  If the developer has provided [documentation for the component](../../developing/using/developing-components.md#main-pars-title-121f), it will appear on the **Documentation** tab. If there is no documentation available, the **Documentation** tab will not be shown.

  ![](assets/chlimage_1-378.png)
