---
title: iosWebContentFilterSpecificWebsitesAccess-Ressourcentyp
description: Stellt einen iOS Web Content Filter-Einstellungstyp dar, der URL-Lesezeichen in den integrierten iOS-Browser installiert. Ein Beispielszenario befindet sich in der Unterrichtsumgebung, in der Lehrer möchten, dass die Schüler Websites über auf Ihren iOS-Geräten konfigurierte Browser-Lesezeichen navigieren und keinen Zugriff auf andere Websites haben.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c5ddd834ccd24d60e2696d49b64685d432f47196
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30150309"
---
# <a name="ioswebcontentfilterspecificwebsitesaccess-resource-type"></a><span data-ttu-id="c519c-104">iosWebContentFilterSpecificWebsitesAccess-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c519c-104">iosWebContentFilterSpecificWebsitesAccess resource type</span></span>

> <span data-ttu-id="c519c-105">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c519c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c519c-106">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c519c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c519c-107">Stellt einen iOS Web Content Filter-Einstellungstyp dar, der URL-Lesezeichen in den integrierten iOS-Browser installiert.</span><span class="sxs-lookup"><span data-stu-id="c519c-107">Represents an iOS Web Content Filter setting type, which installs URL bookmarks into iOS built-in browser.</span></span> <span data-ttu-id="c519c-108">Ein Beispielszenario befindet sich in der Unterrichtsumgebung, in der Lehrer möchten, dass die Schüler Websites über auf Ihren iOS-Geräten konfigurierte Browser-Lesezeichen navigieren und keinen Zugriff auf andere Websites haben.</span><span class="sxs-lookup"><span data-stu-id="c519c-108">An example scenario is in the classroom where teachers would like the students to navigate websites through browser bookmarks configured on their iOS devices, and no access to other sites.</span></span>


<span data-ttu-id="c519c-109">Erbt von [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span><span class="sxs-lookup"><span data-stu-id="c519c-109">Inherits from [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c519c-110">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c519c-110">Properties</span></span>
|<span data-ttu-id="c519c-111">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c519c-111">Property</span></span>|<span data-ttu-id="c519c-112">Typ</span><span class="sxs-lookup"><span data-stu-id="c519c-112">Type</span></span>|<span data-ttu-id="c519c-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c519c-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c519c-114">specificWebsitesOnly</span><span class="sxs-lookup"><span data-stu-id="c519c-114">specificWebsitesOnly</span></span>|<span data-ttu-id="c519c-115">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="c519c-115">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md) collection</span></span>|<span data-ttu-id="c519c-116">URL-Lesezeichen, die in integrierten Browser und Benutzer installiert werden, dürfen nur über Lesezeichen auf Websites zugreifen.</span><span class="sxs-lookup"><span data-stu-id="c519c-116">URL bookmarks which will be installed into built-in browser and user is only allowed to access websites through bookmarks.</span></span> <span data-ttu-id="c519c-117">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="c519c-117">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="c519c-118">Website</span><span class="sxs-lookup"><span data-stu-id="c519c-118">websiteList</span></span>|<span data-ttu-id="c519c-119">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="c519c-119">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md) collection</span></span>|<span data-ttu-id="c519c-120">URL-Lesezeichen, die in integrierten Browser und Benutzer installiert werden, dürfen nur über Lesezeichen auf Websites zugreifen.</span><span class="sxs-lookup"><span data-stu-id="c519c-120">URL bookmarks which will be installed into built-in browser and user is only allowed to access websites through bookmarks.</span></span> <span data-ttu-id="c519c-121">Diese Sammlung darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="c519c-121">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c519c-122">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c519c-122">Relationships</span></span>
<span data-ttu-id="c519c-123">Keine</span><span class="sxs-lookup"><span data-stu-id="c519c-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c519c-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c519c-124">JSON Representation</span></span>
<span data-ttu-id="c519c-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c519c-125">Here is a JSON representation of the resource.</span></span>
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




