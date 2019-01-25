---
title: Ressourcentyp teamGuestSettings
description: Einstellungen konfigurieren können, ob Gäste erstellen, aktualisieren oder Löschen von Kanälen im Team können.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 4d76ffcbc5ec675ee670394854183c07721c0af9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522308"
---
# <a name="teamguestsettings-resource-type"></a><span data-ttu-id="afe2c-103">Ressourcentyp teamGuestSettings</span><span class="sxs-lookup"><span data-stu-id="afe2c-103">teamGuestSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="afe2c-104">Einstellungen konfigurieren können, ob Gäste erstellen, aktualisieren oder Löschen von Kanälen im [Team](team.md)können.</span><span class="sxs-lookup"><span data-stu-id="afe2c-104">Settings to configure whether guests can create, update, or delete channels in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="afe2c-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="afe2c-105">Properties</span></span>
| <span data-ttu-id="afe2c-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="afe2c-106">Property</span></span>     | <span data-ttu-id="afe2c-107">Typ</span><span class="sxs-lookup"><span data-stu-id="afe2c-107">Type</span></span>   |<span data-ttu-id="afe2c-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="afe2c-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="afe2c-109">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="afe2c-109">allowCreateUpdateChannels</span></span>|<span data-ttu-id="afe2c-110">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="afe2c-110">Boolean</span></span>|<span data-ttu-id="afe2c-111">Wenn Festlegung auf "true" Gäste hinzufügen und Kanäle aktualisieren kann.</span><span class="sxs-lookup"><span data-stu-id="afe2c-111">If set to true, guests can add and update channels.</span></span>|
|<span data-ttu-id="afe2c-112">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="afe2c-112">allowDeleteChannels</span></span>|<span data-ttu-id="afe2c-113">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="afe2c-113">Boolean</span></span>|<span data-ttu-id="afe2c-114">Bei Festlegung auf "true" Gäste Kanäle löschen kann.</span><span class="sxs-lookup"><span data-stu-id="afe2c-114">If set to true, guests can delete channels.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="afe2c-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="afe2c-115">JSON representation</span></span>

<span data-ttu-id="afe2c-116">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="afe2c-116">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "team's guestSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamguestsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
