---
title: Ressourcentyp iosWebContentFilterSpecificWebsitesAccess
description: Stellt eine iOS Web Content Filter Einstellungstyp, mit dem URL Textmarken in integrierten iOS-Browser installiert werden. Ein Beispielszenario ist im Kursraum, in dem Lehrer die Teilnehmer auf Websites durch Browser Lesezeichen in ihrer iOS-Geräte und keinen Zugriff auf andere Websites konfiguriert navigieren soll.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 964ade2d2b46755fbba2903c6e9607340f60aedf
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424763"
---
# <a name="ioswebcontentfilterspecificwebsitesaccess-resource-type"></a><span data-ttu-id="ad216-104">Ressourcentyp iosWebContentFilterSpecificWebsitesAccess</span><span class="sxs-lookup"><span data-stu-id="ad216-104">iosWebContentFilterSpecificWebsitesAccess resource type</span></span>

> <span data-ttu-id="ad216-105">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="ad216-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ad216-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ad216-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ad216-107">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ad216-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ad216-108">Stellt eine iOS Web Content Filter Einstellungstyp, mit dem URL Textmarken in integrierten iOS-Browser installiert werden.</span><span class="sxs-lookup"><span data-stu-id="ad216-108">Represents an iOS Web Content Filter setting type, which installs URL bookmarks into iOS built-in browser.</span></span> <span data-ttu-id="ad216-109">Ein Beispielszenario ist im Kursraum, in dem Lehrer die Teilnehmer auf Websites durch Browser Lesezeichen in ihrer iOS-Geräte und keinen Zugriff auf andere Websites konfiguriert navigieren soll.</span><span class="sxs-lookup"><span data-stu-id="ad216-109">An example scenario is in the classroom where teachers would like the students to navigate websites through browser bookmarks configured on their iOS devices, and no access to other sites.</span></span>


<span data-ttu-id="ad216-110">Erbt vom [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span><span class="sxs-lookup"><span data-stu-id="ad216-110">Inherits from [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ad216-111">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ad216-111">Properties</span></span>
|<span data-ttu-id="ad216-112">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ad216-112">Property</span></span>|<span data-ttu-id="ad216-113">Typ</span><span class="sxs-lookup"><span data-stu-id="ad216-113">Type</span></span>|<span data-ttu-id="ad216-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ad216-114">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad216-115">specificWebsitesOnly</span><span class="sxs-lookup"><span data-stu-id="ad216-115">specificWebsitesOnly</span></span>|<span data-ttu-id="ad216-116">[IosBookmark](../resources/intune-deviceconfig-iosbookmark.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="ad216-116">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md) collection</span></span>|<span data-ttu-id="ad216-117">URL Textmarken, die in integrierten Browser und Benutzer installiert werden darf nur durch Lesezeichen Websites zugreifen.</span><span class="sxs-lookup"><span data-stu-id="ad216-117">URL bookmarks which will be installed into built-in browser and user is only allowed to access websites through bookmarks.</span></span> <span data-ttu-id="ad216-118">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="ad216-118">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="ad216-119">websiteList</span><span class="sxs-lookup"><span data-stu-id="ad216-119">websiteList</span></span>|<span data-ttu-id="ad216-120">[IosBookmark](../resources/intune-deviceconfig-iosbookmark.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="ad216-120">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md) collection</span></span>|<span data-ttu-id="ad216-121">URL Textmarken, die in integrierten Browser und Benutzer installiert werden darf nur durch Lesezeichen Websites zugreifen.</span><span class="sxs-lookup"><span data-stu-id="ad216-121">URL bookmarks which will be installed into built-in browser and user is only allowed to access websites through bookmarks.</span></span> <span data-ttu-id="ad216-122">Diese Sammlung darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="ad216-122">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ad216-123">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ad216-123">Relationships</span></span>
<span data-ttu-id="ad216-124">Keine</span><span class="sxs-lookup"><span data-stu-id="ad216-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ad216-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ad216-125">JSON Representation</span></span>
<span data-ttu-id="ad216-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ad216-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosWebContentFilterSpecificWebsitesAccess"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosWebContentFilterSpecificWebsitesAccess",
  "specificWebsitesOnly": [
    {
      "@odata.type": "microsoft.graph.iosBookmark",
      "url": "String",
      "bookmarkFolder": "String",
      "displayName": "String"
    }
  ],
  "websiteList": [
    {
      "@odata.type": "microsoft.graph.iosBookmark",
      "url": "String",
      "bookmarkFolder": "String",
      "displayName": "String"
    }
  ]
}
```




