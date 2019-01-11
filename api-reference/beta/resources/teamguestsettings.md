---
title: Ressourcentyp teamGuestSettings
description: Einstellungen konfigurieren können, ob Gäste erstellen, aktualisieren oder Löschen von Kanälen im Team können.
localization_priority: Normal
ms.openlocfilehash: 15644f3761329589a4d770e777ae5fd63751e6be
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851541"
---
# <a name="teamguestsettings-resource-type"></a><span data-ttu-id="aaabe-103">Ressourcentyp teamGuestSettings</span><span class="sxs-lookup"><span data-stu-id="aaabe-103">teamGuestSettings resource type</span></span>

> <span data-ttu-id="aaabe-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="aaabe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aaabe-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="aaabe-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="aaabe-106">Einstellungen konfigurieren können, ob Gäste erstellen, aktualisieren oder Löschen von Kanälen im [Team](team.md)können.</span><span class="sxs-lookup"><span data-stu-id="aaabe-106">Settings to configure whether guests can create, update, or delete channels in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="aaabe-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="aaabe-107">Properties</span></span>
| <span data-ttu-id="aaabe-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="aaabe-108">Property</span></span>     | <span data-ttu-id="aaabe-109">Typ</span><span class="sxs-lookup"><span data-stu-id="aaabe-109">Type</span></span>   |<span data-ttu-id="aaabe-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aaabe-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aaabe-111">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="aaabe-111">allowCreateUpdateChannels</span></span>|<span data-ttu-id="aaabe-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="aaabe-112">Boolean</span></span>|<span data-ttu-id="aaabe-113">Wenn Festlegung auf "true" Gäste hinzufügen und Kanäle aktualisieren kann.</span><span class="sxs-lookup"><span data-stu-id="aaabe-113">If set to true, guests can add and update channels.</span></span>|
|<span data-ttu-id="aaabe-114">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="aaabe-114">allowDeleteChannels</span></span>|<span data-ttu-id="aaabe-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="aaabe-115">Boolean</span></span>|<span data-ttu-id="aaabe-116">Bei Festlegung auf "true" Gäste Kanäle löschen kann.</span><span class="sxs-lookup"><span data-stu-id="aaabe-116">If set to true, guests can delete channels.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aaabe-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="aaabe-117">JSON representation</span></span>

<span data-ttu-id="aaabe-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="aaabe-118">The following is a JSON representation of the resource.</span></span>

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
