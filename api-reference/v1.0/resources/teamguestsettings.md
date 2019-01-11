---
title: Ressourcentyp teamGuestSettings
description: Einstellungen konfigurieren können, ob Gäste erstellen, aktualisieren oder Löschen von Kanälen im Team können.
localization_priority: Normal
ms.openlocfilehash: f0947101fc8de83d1a56ffa922d9b1e2d79d520f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844876"
---
# <a name="teamguestsettings-resource-type"></a><span data-ttu-id="2dfc0-103">Ressourcentyp teamGuestSettings</span><span class="sxs-lookup"><span data-stu-id="2dfc0-103">teamGuestSettings resource type</span></span>



<span data-ttu-id="2dfc0-104">Einstellungen konfigurieren können, ob Gäste erstellen, aktualisieren oder Löschen von Kanälen im [Team](team.md)können.</span><span class="sxs-lookup"><span data-stu-id="2dfc0-104">Settings to configure whether guests can create, update, or delete channels in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="2dfc0-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2dfc0-105">Properties</span></span>
| <span data-ttu-id="2dfc0-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2dfc0-106">Property</span></span>     | <span data-ttu-id="2dfc0-107">Typ</span><span class="sxs-lookup"><span data-stu-id="2dfc0-107">Type</span></span>   |<span data-ttu-id="2dfc0-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2dfc0-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2dfc0-109">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="2dfc0-109">allowCreateUpdateChannels</span></span>|<span data-ttu-id="2dfc0-110">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="2dfc0-110">Boolean</span></span>|<span data-ttu-id="2dfc0-111">Wenn Festlegung auf "true" Gäste hinzufügen und Kanäle aktualisieren kann.</span><span class="sxs-lookup"><span data-stu-id="2dfc0-111">If set to true, guests can add and update channels.</span></span>|
|<span data-ttu-id="2dfc0-112">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="2dfc0-112">allowDeleteChannels</span></span>|<span data-ttu-id="2dfc0-113">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="2dfc0-113">Boolean</span></span>|<span data-ttu-id="2dfc0-114">Bei Festlegung auf "true" Gäste Kanäle löschen kann.</span><span class="sxs-lookup"><span data-stu-id="2dfc0-114">If set to true, guests can delete channels.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2dfc0-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2dfc0-115">JSON representation</span></span>

<span data-ttu-id="2dfc0-116">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2dfc0-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamGuestSettings"
}-->

```json
{
  "allowCreateUpdateChannels": true,
  "allowDeleteChannels": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's guestSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
