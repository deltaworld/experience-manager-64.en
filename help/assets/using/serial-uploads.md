---
title: Serial Uploads
seo-title: Serial Uploads
description: Learn how AEM Assets one asset at a time when assets are uploaded in bulk and the benefits of serial uploads.
seo-description: Learn how AEM Assets one asset at a time when assets are uploaded in bulk and the benefits of serial uploads.
uuid: a023ed73-fbd6-4747-9295-8c860722e1c5
contentOwner: Chiradeep Majumdar
products: SG_EXPERIENCEMANAGER/6.4/ASSETS
topic-tags: administering
content-type: reference
discoiquuid: 477609c1-b066-4f62-8be0-3bfb42a367fd
---

# Serial Uploads{#serial-uploads}

Uploading numerous assets in bulk consumes significant I/O resources, which may adversely impact the performance of your AEM Assets instance. In particular, if you have a slow internet connection, the time to upload drastically increases due to a spike in disk I/O. Moreover, your web browser may introduce additional restrictions to the number of POST requests AEM Assets can handle for concurrent asset uploads. As a result, the upload operation fails or terminate prematurely. In other words, AEM assets may miss some files while ingesting a bunch of files or altogether fail to ingest any file.

To overcome this situation, AEM Assets ingests one asset at a time (serial upload) during a bulk upload operation, instead of the concurrently ingesting all the assets.

Serial uploading of assets is enabled by default. To disable the feature and allow concurrent uploading, overlay the `fileupload` node in Crx-de and set the value of the `parallelUploads` property to `true`.