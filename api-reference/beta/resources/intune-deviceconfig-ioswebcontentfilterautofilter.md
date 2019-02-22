---
title: iosWebContentFilterAutoFilter-Ressourcentyp
description: Stellt einen iOS Web Content Filter-Einstellungstyp dar, der die automatische iOS-Filterfunktion ermöglicht und eine zusätzliche URL-Zugriffssteuerung ermöglicht. Wenn das iOS-Gerät ohne Eigenschaftswerte erstellt wird, wird der automatische Filter unabhängig davon aktiviert.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 74e281a4cbc08467730680b556e6e8026535ff3a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30155664"
---
# <a name="ioswebcontentfilterautofilter-resource-type"></a><span data-ttu-id="1cc51-104">iosWebContentFilterAutoFilter-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="1cc51-104">iosWebContentFilterAutoFilter resource type</span></span>

> <span data-ttu-id="1cc51-105">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1cc51-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1cc51-106">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="1cc51-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1cc51-107">Stellt einen iOS Web Content Filter-Einstellungstyp dar, der die automatische iOS-Filterfunktion ermöglicht und eine zusätzliche URL-Zugriffssteuerung ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="1cc51-107">Represents an iOS Web Content Filter setting type, which enables iOS automatic filter feature and allows for additional URL access control.</span></span> <span data-ttu-id="1cc51-108">Wenn das iOS-Gerät ohne Eigenschaftswerte erstellt wird, wird der automatische Filter unabhängig davon aktiviert.</span><span class="sxs-lookup"><span data-stu-id="1cc51-108">When constructed with no property values, the iOS device will enable the automatic filter regardless.</span></span>


<span data-ttu-id="1cc51-109">Erbt von [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span><span class="sxs-lookup"><span data-stu-id="1cc51-109">Inherits from [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1cc51-110">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1cc51-110">Properties</span></span>
|<span data-ttu-id="1cc51-111">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1cc51-111">Property</span></span>|<span data-ttu-id="1cc51-112">Typ</span><span class="sxs-lookup"><span data-stu-id="1cc51-112">Type</span></span>|<span data-ttu-id="1cc51-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1cc51-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1cc51-114">allowedUrls</span><span class="sxs-lookup"><span data-stu-id="1cc51-114">allowedUrls</span></span>|<span data-ttu-id="1cc51-115">String collection</span><span class="sxs-lookup"><span data-stu-id="1cc51-115">String collection</span></span>|<span data-ttu-id="1cc51-116">Für den Zugriff zugelassene zusätzliche URLs</span><span class="sxs-lookup"><span data-stu-id="1cc51-116">Additional URLs allowed for access</span></span>|
|<span data-ttu-id="1cc51-117">BlockierteURLs</span><span class="sxs-lookup"><span data-stu-id="1cc51-117">blockedUrls</span></span>|<span data-ttu-id="1cc51-118">String collection</span><span class="sxs-lookup"><span data-stu-id="1cc51-118">String collection</span></span>|<span data-ttu-id="1cc51-119">Für Access blockierte zusätzliche URLs</span><span class="sxs-lookup"><span data-stu-id="1cc51-119">Additional URLs blocked for access</span></span>|

## <a name="relationships"></a><span data-ttu-id="1cc51-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="1cc51-120">Relationships</span></span>
<span data-ttu-id="1cc51-121">Keine</span><span class="sxs-lookup"><span data-stu-id="1cc51-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1cc51-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1cc51-122">JSON Representation</span></span>
<span data-ttu-id="1cc51-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1cc51-123">Here is a JSON representation of the resource.</span></span>
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




