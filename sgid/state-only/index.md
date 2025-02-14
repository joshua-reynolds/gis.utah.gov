---
tags:
  - how to
  - sgid
author:
  display_name: Zach Beck
  email: zbeck@utah.gov
date: 2012-04-10 13:58:58 -0600
title: How to Connect to the SGID via ArcSDE
layout: page_nocrumb
categories: []
---

**Heads up!** As hinted at [earlier this year]({% link _posts/2020-05-04-introducing-open-sgid.md %}), we will be replacing the state-only SGID10 Enterprise Geodatabase with the [Open SGID]({% link sgid/open-sgid/index.md %}) on **December 31st, 2020**. After this date, the SGID10 database will no longer be accessible. While some datasets have been [shelved](http://utah.maps.arcgis.com/home/group.html?id=8765687b7b0545668fff02d1b750f7a9#overview) (old but still relevant data) or removed (out-of-date and unmaintained data), the Open SGID contains substantially the same datasets and is available to anyone with an internet connection. Please take time now to review the [introduction]({% link _posts/2020-05-04-introducing-open-sgid.md %}) and update your data references.
{: .pop .text-center}

The SGID is a collection of vector-format GIS feature classes. Its' content is available for download from the [data pages]({% link data/index.html %}) on this website or via an ArcSDE database connection **for users within the State of Utah network**. Users with ArcGIS desktop clients that are at 10.2.1 or higher can use this resource.

The SGID's organization is based on ISO Topic Categories. UGRC treats the ISO categories as a guideline, and the main goal is to maximize usability for GIS users.

#### When to use

Using a database connection to the most current ArcSDE server can be advantageous as users will see and query the most updated version of all feature classes housed at UGRC. Live connections are excellent for browsing, exploring, or making quick maps with SGID data layers. However, users are encouraged to download or export data files where editing, archiving project data, or optimal performance is required. Additionally, it is recommended and in some cases required that users' ArcMap release version be at or above the level of UGRC's ArcSDE server.

#### Connecting

1. In ArcCatalog or ArcMap (from Add Data), browse to `Add Spatial Database Connections`
  - <img src="{% link images/connect_tree.png %}" alt="ArcMap Add Spatial Connection Screenshot" loading="lazy" />
1. Provide the following connection information, including the password `agrc`.
  - <img src="{% link images/sgidconnect.png %}" title="database connection dialog" alt="database connection dialog" loading="lazy" />

After these steps you will be able to browse the entire SGID catalog and add data to your projects.
