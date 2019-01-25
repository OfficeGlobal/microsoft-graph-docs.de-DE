---
title: Ressourcentyp teamMemberSettings
description: Einstellungen konfigurieren können, ob Mitglieder bestimmter Aktionen ausführen können beispielsweise Kanäle erstellen und Hinzufügen von Programmen, im Team.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: e6fae4d81ac005c1830d5bed9e05a4675e1a8ad0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522644"
---
# <a name="teammembersettings-resource-type"></a><span data-ttu-id="944d9-103">Ressourcentyp teamMemberSettings</span><span class="sxs-lookup"><span data-stu-id="944d9-103">teamMemberSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="944d9-104">Einstellungen konfigurieren können, ob Mitglieder bestimmter Aktionen ausführen können beispielsweise Kanäle erstellen und Hinzufügen von Programmen, im [Team](team.md).</span><span class="sxs-lookup"><span data-stu-id="944d9-104">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="944d9-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="944d9-105">Properties</span></span>
| <span data-ttu-id="944d9-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="944d9-106">Property</span></span>     | <span data-ttu-id="944d9-107">Typ</span><span class="sxs-lookup"><span data-stu-id="944d9-107">Type</span></span>   |<span data-ttu-id="944d9-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="944d9-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="944d9-109">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="944d9-109">allowCreateUpdateChannels</span></span>|<span data-ttu-id="944d9-110">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="944d9-110">Boolean</span></span>|<span data-ttu-id="944d9-111">Wenn es sich bei Festlegung auf true fest, Mitglieder hinzufügen und Aktualisieren von Kanäle kann.</span><span class="sxs-lookup"><span data-stu-id="944d9-111">If set to true, members can add and update channels.</span></span>|
|<span data-ttu-id="944d9-112">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="944d9-112">allowDeleteChannels</span></span>|<span data-ttu-id="944d9-113">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="944d9-113">Boolean</span></span>|<span data-ttu-id="944d9-114">Bei Festlegung auf "true" Mitglieder Kanäle löschen kann.</span><span class="sxs-lookup"><span data-stu-id="944d9-114">If set to true, members can delete channels.</span></span>|
|<span data-ttu-id="944d9-115">allowAddRemoveApps</span><span class="sxs-lookup"><span data-stu-id="944d9-115">allowAddRemoveApps</span></span>|<span data-ttu-id="944d9-116">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="944d9-116">Boolean</span></span>|<span data-ttu-id="944d9-117">Wenn es sich bei Festlegung auf "true" Mitglieder hinzufügen und Entfernen von apps.</span><span class="sxs-lookup"><span data-stu-id="944d9-117">If set to true, members can add and remove apps.</span></span>|
|<span data-ttu-id="944d9-118">allowCreateUpdateRemoveTabs</span><span class="sxs-lookup"><span data-stu-id="944d9-118">allowCreateUpdateRemoveTabs</span></span>|<span data-ttu-id="944d9-119">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="944d9-119">Boolean</span></span>|<span data-ttu-id="944d9-120">Wenn es sich bei Festlegung auf true fest, Mitglieder hinzufügen kann, aktualisieren und Entfernen von Registerkarten.</span><span class="sxs-lookup"><span data-stu-id="944d9-120">If set to true, members can add, update, and remove tabs.</span></span> |
|<span data-ttu-id="944d9-121">allowCreateUpdateRemoveConnectors</span><span class="sxs-lookup"><span data-stu-id="944d9-121">allowCreateUpdateRemoveConnectors</span></span>|<span data-ttu-id="944d9-122">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="944d9-122">Boolean</span></span>|<span data-ttu-id="944d9-123">Wenn es sich bei Festlegung auf true fest, Mitglieder hinzufügen kann, aktualisieren und Entfernen von Connectors.</span><span class="sxs-lookup"><span data-stu-id="944d9-123">If set to true, members can add, update, and remove connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="944d9-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="944d9-124">JSON representation</span></span>

<span data-ttu-id="944d9-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="944d9-125">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "team's memberSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/teammembersettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
