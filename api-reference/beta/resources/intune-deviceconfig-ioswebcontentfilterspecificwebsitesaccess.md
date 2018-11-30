---
title: Ressourcentyp iosWebContentFilterSpecificWebsitesAccess
description: Stellt eine iOS Web Content Filter Einstellungstyp, mit dem URL Textmarken in integrierten iOS-Browser installiert werden. Ein Beispielszenario ist im Kursraum, in dem Lehrer die Teilnehmer auf Websites durch Browser Lesezeichen in ihrer iOS-Geräte und keinen Zugriff auf andere Websites konfiguriert navigieren soll.
ms.openlocfilehash: c5e23905ab9e5b692500544161fc052dd606da5d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062437"
---
# <a name="ioswebcontentfilterspecificwebsitesaccess-resource-type"></a><span data-ttu-id="d3153-104">Ressourcentyp iosWebContentFilterSpecificWebsitesAccess</span><span class="sxs-lookup"><span data-stu-id="d3153-104">iosWebContentFilterSpecificWebsitesAccess resource type</span></span>

> <span data-ttu-id="d3153-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d3153-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d3153-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d3153-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d3153-107">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d3153-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d3153-108">Stellt eine iOS Web Content Filter Einstellungstyp, mit dem URL Textmarken in integrierten iOS-Browser installiert werden.</span><span class="sxs-lookup"><span data-stu-id="d3153-108">Represents an iOS Web Content Filter setting type, which installs URL bookmarks into iOS built-in browser.</span></span> <span data-ttu-id="d3153-109">Ein Beispielszenario ist im Kursraum, in dem Lehrer die Teilnehmer auf Websites durch Browser Lesezeichen in ihrer iOS-Geräte und keinen Zugriff auf andere Websites konfiguriert navigieren soll.</span><span class="sxs-lookup"><span data-stu-id="d3153-109">An example scenario is in the classroom where teachers would like the students to navigate websites through browser bookmarks configured on their iOS devices, and no access to other sites.</span></span>

<span data-ttu-id="d3153-110">Erbt vom [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span><span class="sxs-lookup"><span data-stu-id="d3153-110">Inherits from [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d3153-111">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d3153-111">Properties</span></span>
|<span data-ttu-id="d3153-112">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d3153-112">Property</span></span>|<span data-ttu-id="d3153-113">Typ</span><span class="sxs-lookup"><span data-stu-id="d3153-113">Type</span></span>|<span data-ttu-id="d3153-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d3153-114">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3153-115">specificWebsitesOnly</span><span class="sxs-lookup"><span data-stu-id="d3153-115">specificWebsitesOnly</span></span>|<span data-ttu-id="d3153-116">[IosBookmark](../resources/intune-deviceconfig-iosbookmark.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="d3153-116">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md) collection</span></span>|<span data-ttu-id="d3153-117">URL Textmarken, die in integrierten Browser und Benutzer installiert werden darf nur durch Lesezeichen Websites zugreifen.</span><span class="sxs-lookup"><span data-stu-id="d3153-117">URL bookmarks which will be installed into built-in browser and user is only allowed to access websites through bookmarks.</span></span> <span data-ttu-id="d3153-118">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="d3153-118">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="d3153-119">websiteList</span><span class="sxs-lookup"><span data-stu-id="d3153-119">websiteList</span></span>|<span data-ttu-id="d3153-120">[IosBookmark](../resources/intune-deviceconfig-iosbookmark.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="d3153-120">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md) collection</span></span>|<span data-ttu-id="d3153-121">URL Textmarken, die in integrierten Browser und Benutzer installiert werden darf nur durch Lesezeichen Websites zugreifen.</span><span class="sxs-lookup"><span data-stu-id="d3153-121">URL bookmarks which will be installed into built-in browser and user is only allowed to access websites through bookmarks.</span></span> <span data-ttu-id="d3153-122">Diese Sammlung darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="d3153-122">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d3153-123">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d3153-123">Relationships</span></span>
<span data-ttu-id="d3153-124">Keine</span><span class="sxs-lookup"><span data-stu-id="d3153-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d3153-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d3153-125">JSON Representation</span></span>
<span data-ttu-id="d3153-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d3153-126">Here is a JSON representation of the resource.</span></span>
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





