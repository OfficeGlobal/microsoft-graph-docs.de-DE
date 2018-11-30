---
title: Ressourcentyp teamGuestSettings
description: Einstellungen konfigurieren können, ob Gäste erstellen, aktualisieren oder Löschen von Kanälen im Team können.
ms.openlocfilehash: 3c59c84e0baa9db580a81eeb72a405ec5097c478
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018675"
---
# <a name="teamguestsettings-resource-type"></a><span data-ttu-id="a654f-103">Ressourcentyp teamGuestSettings</span><span class="sxs-lookup"><span data-stu-id="a654f-103">teamGuestSettings resource type</span></span>



<span data-ttu-id="a654f-104">Einstellungen konfigurieren können, ob Gäste erstellen, aktualisieren oder Löschen von Kanälen im [Team](team.md)können.</span><span class="sxs-lookup"><span data-stu-id="a654f-104">Settings to configure whether guests can create, update, or delete channels in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a654f-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a654f-105">Properties</span></span>
| <span data-ttu-id="a654f-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a654f-106">Property</span></span>     | <span data-ttu-id="a654f-107">Typ</span><span class="sxs-lookup"><span data-stu-id="a654f-107">Type</span></span>   |<span data-ttu-id="a654f-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a654f-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a654f-109">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="a654f-109">allowCreateUpdateChannels</span></span>|<span data-ttu-id="a654f-110">Boolesch</span><span class="sxs-lookup"><span data-stu-id="a654f-110">Boolean</span></span>|<span data-ttu-id="a654f-111">Wenn Festlegung auf "true" Gäste hinzufügen und Kanäle aktualisieren kann.</span><span class="sxs-lookup"><span data-stu-id="a654f-111">If set to true, guests can add and update channels.</span></span>|
|<span data-ttu-id="a654f-112">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="a654f-112">allowDeleteChannels</span></span>|<span data-ttu-id="a654f-113">Boolesch</span><span class="sxs-lookup"><span data-stu-id="a654f-113">Boolean</span></span>|<span data-ttu-id="a654f-114">Bei Festlegung auf "true" Gäste Kanäle löschen kann.</span><span class="sxs-lookup"><span data-stu-id="a654f-114">If set to true, guests can delete channels.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a654f-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a654f-115">JSON representation</span></span>

<span data-ttu-id="a654f-116">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a654f-116">The following is a JSON representation of the resource.</span></span>

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
