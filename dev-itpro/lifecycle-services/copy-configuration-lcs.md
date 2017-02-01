---
# required metadata

title: Copy a configuration | Microsoft Docs
description: 
author: kfend
manager: AnnBe
ms.date: 2015-12-03 20:22:34
ms.topic: article
ms.prod: 
ms.service: Lifecycle Services
ms.technology: 

# optional metadata

# keywords: 
# ROBOTS: 
audience: Developer, IT Pro
# ms.devlang: 
ms.reviewer: 51
ms.suite: AX 2012
# ms.tgt_pltfrm: 
ms.custom: 15541
ms.assetid: 4ec2d6d5-d52e-4420-9ea3-ed972f365a97
ms.region: Global
# ms.industry: 
ms.author: kfend

---

# Copy a configuration



You can use the Configuration manager (beta) functionality in Microsoft Dynamics Lifecycle Services to copy a configuration from one instance of Microsoft Dynamics AX 2012 R3 to another.
| **Important**                                                                                                                                                                                                                                                                                                     |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| This feature is **not** supported for production use. Configuration manager (beta) relies on entities from the Data Import Export Framework in your environment. Because these entities do not currently include all the functionality in AX 2012 R3, some configuration data is not copied between environments. |

Before you begin, you must set up Configuration manager (beta). For more information, see [Set up Configuration manager (Lifecycle Services, LCS)](https://docs.microsoft.com/en-us/dynamics365/operations/dev-itpro/lifecycle-services/set-up-configuration-manager-lifecycle-services-lcs).

## Export a configuration
You can create a stored configuration by exporting it from a specified legal entity and entities.
1.  In the **Configurations to export** list, click the plus sign (+).
2.  Enter a name for the configuration, and then click **Start**.
3.  Select a storage location, and then click **Continue**. You can store your configuration locally, in the cloud, or in both locations.
4.  Select an environment to connect to, and then click **Continue**.
5.  Review the legal entities that are available in the partitions in your environment. Select the legal entities to work with, and then click **Continue**.
6.  Select the entities to copy to a stored configuration.
7.  Optional: Tables that contain configuration data but are not in entities can't be copied to a stored configuration. To see these tables, click the **Missing tables** tab.
8.  Click **Continue** to create your stored configuration. After a configuration has been created, you can review what it contains.

## Import a configuration
1.  In the **Configurations to import** list, select an existing configuration.
2.  Use the default name, or enter a new name. If the configuration was stored both locally and in the cloud, you can select which location to import the stored configuration from. Click **Continue**.
3.  Select the environment to import the configuration to, and then click **Continue**.
4.  Review the companies that are available in the partitions in your environment. Select the companies to work with by selecting the location of the company that you are importing from (for example, initialDAT), and then click **Continue**.
5.  Select the entities to copy to a stored configuration.
6.  Click **Continue** to import your stored configuration. After a configuration has been created, you can review what it contains.


