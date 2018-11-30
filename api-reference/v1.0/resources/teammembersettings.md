---
title: Ressourcentyp teamMemberSettings
description: Einstellungen konfigurieren können, ob Mitglieder bestimmter Aktionen ausführen können beispielsweise Kanäle erstellen und Hinzufügen von Programmen, im Team.
ms.openlocfilehash: 74d88e1d87c65745fe98da9b1ee21b26824dc4e6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018766"
---
# <a name="teammembersettings-resource-type"></a><span data-ttu-id="b585c-103">Ressourcentyp teamMemberSettings</span><span class="sxs-lookup"><span data-stu-id="b585c-103">teamMemberSettings resource type</span></span>



<span data-ttu-id="b585c-104">Einstellungen konfigurieren können, ob Mitglieder bestimmter Aktionen ausführen können beispielsweise Kanäle erstellen und Hinzufügen von Programmen, im [Team](team.md).</span><span class="sxs-lookup"><span data-stu-id="b585c-104">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b585c-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b585c-105">Properties</span></span>
| <span data-ttu-id="b585c-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b585c-106">Property</span></span>     | <span data-ttu-id="b585c-107">Typ</span><span class="sxs-lookup"><span data-stu-id="b585c-107">Type</span></span>   |<span data-ttu-id="b585c-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b585c-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b585c-109">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="b585c-109">allowCreateUpdateChannels</span></span>|<span data-ttu-id="b585c-110">Boolesch</span><span class="sxs-lookup"><span data-stu-id="b585c-110">Boolean</span></span>|<span data-ttu-id="b585c-111">Wenn es sich bei Festlegung auf true fest, Mitglieder hinzufügen und Aktualisieren von Kanäle kann.</span><span class="sxs-lookup"><span data-stu-id="b585c-111">If set to true, members can add and update channels.</span></span>|
|<span data-ttu-id="b585c-112">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="b585c-112">allowDeleteChannels</span></span>|<span data-ttu-id="b585c-113">Boolesch</span><span class="sxs-lookup"><span data-stu-id="b585c-113">Boolean</span></span>|<span data-ttu-id="b585c-114">Bei Festlegung auf "true" Mitglieder Kanäle löschen kann.</span><span class="sxs-lookup"><span data-stu-id="b585c-114">If set to true, members can delete channels.</span></span>|
|<span data-ttu-id="b585c-115">allowAddRemoveApps</span><span class="sxs-lookup"><span data-stu-id="b585c-115">allowAddRemoveApps</span></span>|<span data-ttu-id="b585c-116">Boolesch</span><span class="sxs-lookup"><span data-stu-id="b585c-116">Boolean</span></span>|<span data-ttu-id="b585c-117">Wenn es sich bei Festlegung auf "true" Mitglieder hinzufügen und Entfernen von apps.</span><span class="sxs-lookup"><span data-stu-id="b585c-117">If set to true, members can add and remove apps.</span></span>|
|<span data-ttu-id="b585c-118">allowCreateUpdateRemoveTabs</span><span class="sxs-lookup"><span data-stu-id="b585c-118">allowCreateUpdateRemoveTabs</span></span>|<span data-ttu-id="b585c-119">Boolesch</span><span class="sxs-lookup"><span data-stu-id="b585c-119">Boolean</span></span>|<span data-ttu-id="b585c-120">Wenn es sich bei Festlegung auf true fest, Mitglieder hinzufügen kann, aktualisieren und Entfernen von Registerkarten.</span><span class="sxs-lookup"><span data-stu-id="b585c-120">If set to true, members can add, update, and remove tabs.</span></span> |
|<span data-ttu-id="b585c-121">allowCreateUpdateRemoveConnectors</span><span class="sxs-lookup"><span data-stu-id="b585c-121">allowCreateUpdateRemoveConnectors</span></span>|<span data-ttu-id="b585c-122">Boolesch</span><span class="sxs-lookup"><span data-stu-id="b585c-122">Boolean</span></span>|<span data-ttu-id="b585c-123">Wenn es sich bei Festlegung auf true fest, Mitglieder hinzufügen kann, aktualisieren und Entfernen von Connectors.</span><span class="sxs-lookup"><span data-stu-id="b585c-123">If set to true, members can add, update, and remove connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b585c-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b585c-124">JSON representation</span></span>

<span data-ttu-id="b585c-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b585c-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamMemberSettings"
}-->

```json
{
  "allowCreateUpdateChannels": true,
  "allowDeleteChannels": true,
  "allowAddRemoveApps": true,
  "allowCreateUpdateRemoveTabs": true,
  "allowCreateUpdateRemoveConnectors": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's memberSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
