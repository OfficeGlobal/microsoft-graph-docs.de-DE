---
title: Ressourcentyp teamMemberSettings
description: Einstellungen konfigurieren können, ob Mitglieder bestimmter Aktionen ausführen können beispielsweise Kanäle erstellen und Hinzufügen von Programmen, im Team.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 3854481e89f04fa727b77c6b4f8699c62a16d739
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978249"
---
# <a name="teammembersettings-resource-type"></a><span data-ttu-id="9bec8-103">Ressourcentyp teamMemberSettings</span><span class="sxs-lookup"><span data-stu-id="9bec8-103">teamMemberSettings resource type</span></span>

> <span data-ttu-id="9bec8-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9bec8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9bec8-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9bec8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9bec8-106">Einstellungen konfigurieren können, ob Mitglieder bestimmter Aktionen ausführen können beispielsweise Kanäle erstellen und Hinzufügen von Programmen, im [Team](team.md).</span><span class="sxs-lookup"><span data-stu-id="9bec8-106">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="9bec8-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9bec8-107">Properties</span></span>
| <span data-ttu-id="9bec8-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9bec8-108">Property</span></span>     | <span data-ttu-id="9bec8-109">Typ</span><span class="sxs-lookup"><span data-stu-id="9bec8-109">Type</span></span>   |<span data-ttu-id="9bec8-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9bec8-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9bec8-111">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="9bec8-111">allowCreateUpdateChannels</span></span>|<span data-ttu-id="9bec8-112">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9bec8-112">Boolean</span></span>|<span data-ttu-id="9bec8-113">Wenn es sich bei Festlegung auf true fest, Mitglieder hinzufügen und Aktualisieren von Kanäle kann.</span><span class="sxs-lookup"><span data-stu-id="9bec8-113">If set to true, members can add and update channels.</span></span>|
|<span data-ttu-id="9bec8-114">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="9bec8-114">allowDeleteChannels</span></span>|<span data-ttu-id="9bec8-115">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9bec8-115">Boolean</span></span>|<span data-ttu-id="9bec8-116">Bei Festlegung auf "true" Mitglieder Kanäle löschen kann.</span><span class="sxs-lookup"><span data-stu-id="9bec8-116">If set to true, members can delete channels.</span></span>|
|<span data-ttu-id="9bec8-117">allowAddRemoveApps</span><span class="sxs-lookup"><span data-stu-id="9bec8-117">allowAddRemoveApps</span></span>|<span data-ttu-id="9bec8-118">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9bec8-118">Boolean</span></span>|<span data-ttu-id="9bec8-119">Wenn es sich bei Festlegung auf "true" Mitglieder hinzufügen und Entfernen von apps.</span><span class="sxs-lookup"><span data-stu-id="9bec8-119">If set to true, members can add and remove apps.</span></span>|
|<span data-ttu-id="9bec8-120">allowCreateUpdateRemoveTabs</span><span class="sxs-lookup"><span data-stu-id="9bec8-120">allowCreateUpdateRemoveTabs</span></span>|<span data-ttu-id="9bec8-121">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9bec8-121">Boolean</span></span>|<span data-ttu-id="9bec8-122">Wenn es sich bei Festlegung auf true fest, Mitglieder hinzufügen kann, aktualisieren und Entfernen von Registerkarten.</span><span class="sxs-lookup"><span data-stu-id="9bec8-122">If set to true, members can add, update, and remove tabs.</span></span> |
|<span data-ttu-id="9bec8-123">allowCreateUpdateRemoveConnectors</span><span class="sxs-lookup"><span data-stu-id="9bec8-123">allowCreateUpdateRemoveConnectors</span></span>|<span data-ttu-id="9bec8-124">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9bec8-124">Boolean</span></span>|<span data-ttu-id="9bec8-125">Wenn es sich bei Festlegung auf true fest, Mitglieder hinzufügen kann, aktualisieren und Entfernen von Connectors.</span><span class="sxs-lookup"><span data-stu-id="9bec8-125">If set to true, members can add, update, and remove connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9bec8-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9bec8-126">JSON representation</span></span>

<span data-ttu-id="9bec8-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9bec8-127">The following is a JSON representation of the resource.</span></span>

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
