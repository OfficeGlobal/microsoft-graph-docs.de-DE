---
title: Ressourcentyp audioSourceLevel
description: Konfiguration für andere Datenquellen.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c91a4c57b283f7669b2be22bba5de5d958b437ad
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528375"
---
# <a name="audiosourcelevel-resource-type"></a><span data-ttu-id="d27c7-103">Ressourcentyp audioSourceLevel</span><span class="sxs-lookup"><span data-stu-id="d27c7-103">audioSourceLevel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d27c7-104">Konfiguration für andere Datenquellen.</span><span class="sxs-lookup"><span data-stu-id="d27c7-104">Level configuration for other sources.</span></span>

## <a name="properties"></a><span data-ttu-id="d27c7-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d27c7-105">Properties</span></span>

| <span data-ttu-id="d27c7-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d27c7-106">Property</span></span>               | <span data-ttu-id="d27c7-107">Typ</span><span class="sxs-lookup"><span data-stu-id="d27c7-107">Type</span></span>    | <span data-ttu-id="d27c7-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d27c7-108">Description</span></span>                                                                                         |
| :--------------------- | :------ | :---------------------------------------------------------------------------------------------------|
| <span data-ttu-id="d27c7-109">duckOthers</span><span class="sxs-lookup"><span data-stu-id="d27c7-109">duckOthers</span></span>             | <span data-ttu-id="d27c7-110">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d27c7-110">Boolean</span></span> | <span data-ttu-id="d27c7-111">Dieser Quelle zu anderen Quellen, während es aktiv Wildenten ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="d27c7-111">Enables this source to duck other sources while active.</span></span> <span data-ttu-id="d27c7-112">Wenn auf true festgelegt ist, vermeiden Ebene festgelegt ist festgelegt werden soll.</span><span class="sxs-lookup"><span data-stu-id="d27c7-112">If set to true, ducking level has to be set.</span></span>|
| <span data-ttu-id="d27c7-113">Ebene</span><span class="sxs-lookup"><span data-stu-id="d27c7-113">level</span></span>                  | <span data-ttu-id="d27c7-114">Int64</span><span class="sxs-lookup"><span data-stu-id="d27c7-114">Int64</span></span>   | <span data-ttu-id="d27c7-115">Ebene der Quelle vermeiden, wenn `duckOthers` auf festgelegt ist `true`.</span><span class="sxs-lookup"><span data-stu-id="d27c7-115">Ducking level of the source if `duckOthers` is set to `true`.</span></span>                                     |
| <span data-ttu-id="d27c7-116">Teilnehmer</span><span class="sxs-lookup"><span data-stu-id="d27c7-116">participant</span></span>            | <span data-ttu-id="d27c7-117">String</span><span class="sxs-lookup"><span data-stu-id="d27c7-117">String</span></span>  | <span data-ttu-id="d27c7-118">Die Teilnehmer Audiostream von Quelle.</span><span class="sxs-lookup"><span data-stu-id="d27c7-118">The source participant audio stream.</span></span>                                                                |

## <a name="json-representation"></a><span data-ttu-id="d27c7-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d27c7-119">JSON representation</span></span>

<span data-ttu-id="d27c7-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d27c7-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioSourceLevel"
}-->
```json
{
  "duckOthers": true,
  "level": 100,
  "participant": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "audioSourceLevel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/audiosourcelevel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
