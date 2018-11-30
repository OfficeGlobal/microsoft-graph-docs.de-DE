---
title: Ressourcentyp teamMemberSettings
description: Einstellungen konfigurieren können, ob Mitglieder bestimmter Aktionen ausführen können beispielsweise Kanäle erstellen und Hinzufügen von Programmen, im Team.
ms.openlocfilehash: fa673e050ab3362ae7b132f30cfc4caf16d96dcc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058558"
---
# <a name="teammembersettings-resource-type"></a><span data-ttu-id="2e6c3-103">Ressourcentyp teamMemberSettings</span><span class="sxs-lookup"><span data-stu-id="2e6c3-103">teamMemberSettings resource type</span></span>

> <span data-ttu-id="2e6c3-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2e6c3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2e6c3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2e6c3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2e6c3-106">Einstellungen konfigurieren können, ob Mitglieder bestimmter Aktionen ausführen können beispielsweise Kanäle erstellen und Hinzufügen von Programmen, im [Team](team.md).</span><span class="sxs-lookup"><span data-stu-id="2e6c3-106">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="2e6c3-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2e6c3-107">Properties</span></span>
| <span data-ttu-id="2e6c3-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2e6c3-108">Property</span></span>     | <span data-ttu-id="2e6c3-109">Typ</span><span class="sxs-lookup"><span data-stu-id="2e6c3-109">Type</span></span>   |<span data-ttu-id="2e6c3-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2e6c3-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2e6c3-111">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="2e6c3-111">allowCreateUpdateChannels</span></span>|<span data-ttu-id="2e6c3-112">Boolesch</span><span class="sxs-lookup"><span data-stu-id="2e6c3-112">Boolean</span></span>|<span data-ttu-id="2e6c3-113">Wenn es sich bei Festlegung auf true fest, Mitglieder hinzufügen und Aktualisieren von Kanäle kann.</span><span class="sxs-lookup"><span data-stu-id="2e6c3-113">If set to true, members can add and update channels.</span></span>|
|<span data-ttu-id="2e6c3-114">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="2e6c3-114">allowDeleteChannels</span></span>|<span data-ttu-id="2e6c3-115">Boolesch</span><span class="sxs-lookup"><span data-stu-id="2e6c3-115">Boolean</span></span>|<span data-ttu-id="2e6c3-116">Bei Festlegung auf "true" Mitglieder Kanäle löschen kann.</span><span class="sxs-lookup"><span data-stu-id="2e6c3-116">If set to true, members can delete channels.</span></span>|
|<span data-ttu-id="2e6c3-117">allowAddRemoveApps</span><span class="sxs-lookup"><span data-stu-id="2e6c3-117">allowAddRemoveApps</span></span>|<span data-ttu-id="2e6c3-118">Boolesch</span><span class="sxs-lookup"><span data-stu-id="2e6c3-118">Boolean</span></span>|<span data-ttu-id="2e6c3-119">Wenn es sich bei Festlegung auf "true" Mitglieder hinzufügen und Entfernen von apps.</span><span class="sxs-lookup"><span data-stu-id="2e6c3-119">If set to true, members can add and remove apps.</span></span>|
|<span data-ttu-id="2e6c3-120">allowCreateUpdateRemoveTabs</span><span class="sxs-lookup"><span data-stu-id="2e6c3-120">allowCreateUpdateRemoveTabs</span></span>|<span data-ttu-id="2e6c3-121">Boolesch</span><span class="sxs-lookup"><span data-stu-id="2e6c3-121">Boolean</span></span>|<span data-ttu-id="2e6c3-122">Wenn es sich bei Festlegung auf true fest, Mitglieder hinzufügen kann, aktualisieren und Entfernen von Registerkarten.</span><span class="sxs-lookup"><span data-stu-id="2e6c3-122">If set to true, members can add, update, and remove tabs.</span></span> |
|<span data-ttu-id="2e6c3-123">allowCreateUpdateRemoveConnectors</span><span class="sxs-lookup"><span data-stu-id="2e6c3-123">allowCreateUpdateRemoveConnectors</span></span>|<span data-ttu-id="2e6c3-124">Boolesch</span><span class="sxs-lookup"><span data-stu-id="2e6c3-124">Boolean</span></span>|<span data-ttu-id="2e6c3-125">Wenn es sich bei Festlegung auf true fest, Mitglieder hinzufügen kann, aktualisieren und Entfernen von Connectors.</span><span class="sxs-lookup"><span data-stu-id="2e6c3-125">If set to true, members can add, update, and remove connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2e6c3-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2e6c3-126">JSON representation</span></span>

<span data-ttu-id="2e6c3-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2e6c3-127">The following is a JSON representation of the resource.</span></span>

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
