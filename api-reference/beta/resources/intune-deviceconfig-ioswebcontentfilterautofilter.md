---
title: Ressourcentyp iosWebContentFilterAutoFilter
description: Stellt eine iOS Webinhaltsfilter Einstellungstyp, der ermöglicht automatische Filterfunktion iOS und zusätzliche URL-Zugriffssteuerung. Wenn keine-Eigenschaft Werte erstellt wird, wird das Gerät iOS den automatischen Filter unabhängig aktivieren.
ms.openlocfilehash: 04a221ac512ab3934702a2a9e3178ba23a2ac3ef
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063746"
---
# <a name="ioswebcontentfilterautofilter-resource-type"></a><span data-ttu-id="1ccb2-104">Ressourcentyp iosWebContentFilterAutoFilter</span><span class="sxs-lookup"><span data-stu-id="1ccb2-104">iosWebContentFilterAutoFilter resource type</span></span>

> <span data-ttu-id="1ccb2-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1ccb2-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1ccb2-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1ccb2-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1ccb2-107">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1ccb2-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1ccb2-108">Stellt eine iOS Webinhaltsfilter Einstellungstyp, der ermöglicht automatische Filterfunktion iOS und zusätzliche URL-Zugriffssteuerung.</span><span class="sxs-lookup"><span data-stu-id="1ccb2-108">Represents an iOS Web Content Filter setting type, which enables iOS automatic filter feature and allows for additional URL access control.</span></span> <span data-ttu-id="1ccb2-109">Wenn keine-Eigenschaft Werte erstellt wird, wird das Gerät iOS den automatischen Filter unabhängig aktivieren.</span><span class="sxs-lookup"><span data-stu-id="1ccb2-109">When constructed with no property values, the iOS device will enable the automatic filter regardless.</span></span>

<span data-ttu-id="1ccb2-110">Erbt vom [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span><span class="sxs-lookup"><span data-stu-id="1ccb2-110">Inherits from [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1ccb2-111">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1ccb2-111">Properties</span></span>
|<span data-ttu-id="1ccb2-112">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1ccb2-112">Property</span></span>|<span data-ttu-id="1ccb2-113">Typ</span><span class="sxs-lookup"><span data-stu-id="1ccb2-113">Type</span></span>|<span data-ttu-id="1ccb2-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1ccb2-114">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ccb2-115">allowedUrls</span><span class="sxs-lookup"><span data-stu-id="1ccb2-115">allowedUrls</span></span>|<span data-ttu-id="1ccb2-116">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="1ccb2-116">String collection</span></span>|<span data-ttu-id="1ccb2-117">Zusätzliche URLs für den Zugriff zulässig</span><span class="sxs-lookup"><span data-stu-id="1ccb2-117">Additional URLs allowed for access</span></span>|
|<span data-ttu-id="1ccb2-118">blockedUrls</span><span class="sxs-lookup"><span data-stu-id="1ccb2-118">blockedUrls</span></span>|<span data-ttu-id="1ccb2-119">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="1ccb2-119">String collection</span></span>|<span data-ttu-id="1ccb2-120">Zusätzliche URLs für den Zugriff blockiert</span><span class="sxs-lookup"><span data-stu-id="1ccb2-120">Additional URLs blocked for access</span></span>|

## <a name="relationships"></a><span data-ttu-id="1ccb2-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="1ccb2-121">Relationships</span></span>
<span data-ttu-id="1ccb2-122">Keine</span><span class="sxs-lookup"><span data-stu-id="1ccb2-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1ccb2-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1ccb2-123">JSON Representation</span></span>
<span data-ttu-id="1ccb2-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1ccb2-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosWebContentFilterAutoFilter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosWebContentFilterAutoFilter",
  "allowedUrls": [
    "String"
  ],
  "blockedUrls": [
    "String"
  ]
}
```





