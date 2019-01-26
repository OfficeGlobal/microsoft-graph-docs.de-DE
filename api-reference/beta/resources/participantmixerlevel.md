---
title: Ressourcentyp participantMixerLevel
description: Konfiguration der Mixer Ebenen zur angegebenen audio-Teilnehmer
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: bb5d28ac45d510a715dcc5001c8ee02b8352bb8c
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575419"
---
# <a name="participantmixerlevel-resource-type"></a><span data-ttu-id="3d9ed-103">Ressourcentyp participantMixerLevel</span><span class="sxs-lookup"><span data-stu-id="3d9ed-103">participantMixerLevel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d9ed-104">Konfiguration der Mixer Ebenen zur angegebenen audio-Teilnehmer</span><span class="sxs-lookup"><span data-stu-id="3d9ed-104">Configuration of mixer levels for given audio participant</span></span>

## <a name="properties"></a><span data-ttu-id="3d9ed-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3d9ed-105">Properties</span></span>

| <span data-ttu-id="3d9ed-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3d9ed-106">Property</span></span>               | <span data-ttu-id="3d9ed-107">Typ</span><span class="sxs-lookup"><span data-stu-id="3d9ed-107">Type</span></span>                                                      | <span data-ttu-id="3d9ed-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3d9ed-108">Description</span></span>                                                                                         |
| :--------------------- | :-------------------------------------------------------- | :---------------------------------------------------------------------------------------------------|
| <span data-ttu-id="3d9ed-109">Vermeiden von</span><span class="sxs-lookup"><span data-stu-id="3d9ed-109">ducking</span></span>                | [<span data-ttu-id="3d9ed-110">audioDuckingConfiguration</span><span class="sxs-lookup"><span data-stu-id="3d9ed-110">audioDuckingConfiguration</span></span>](audioduckingconfiguration.md) | <span data-ttu-id="3d9ed-111">Konfiguration der benutzerdefinierte Mischung (welchen Phasen an- und Abmelden) andere Quellen für diese Teilnehmer zu vermeiden.</span><span class="sxs-lookup"><span data-stu-id="3d9ed-111">Configuration of ducking (phasing in and out) of other sources for this partipant custom mix.</span></span>       |
| <span data-ttu-id="3d9ed-112">exclusiveMode</span><span class="sxs-lookup"><span data-stu-id="3d9ed-112">exclusiveMode</span></span>          | <span data-ttu-id="3d9ed-113">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3d9ed-113">boolean</span></span>                                                   | <span data-ttu-id="3d9ed-114">Gibt an, ob von der Mischung Quellen ohne explizite Quellebene entfernt werden soll.</span><span class="sxs-lookup"><span data-stu-id="3d9ed-114">Whether sources without explicit source level should be removed from the mix.</span></span>                       |
| <span data-ttu-id="3d9ed-115">Teilnehmer</span><span class="sxs-lookup"><span data-stu-id="3d9ed-115">participant</span></span>            | <span data-ttu-id="3d9ed-116">String</span><span class="sxs-lookup"><span data-stu-id="3d9ed-116">String</span></span>                                                    | <span data-ttu-id="3d9ed-117">Die Teilnehmer für den Mischer konfiguriert wird.</span><span class="sxs-lookup"><span data-stu-id="3d9ed-117">The participant for whom the mixer is being configured.</span></span>                                             |
| <span data-ttu-id="3d9ed-118">sourceLevels</span><span class="sxs-lookup"><span data-stu-id="3d9ed-118">sourceLevels</span></span>           | <span data-ttu-id="3d9ed-119">[AudioSourceLevel](audiosourcelevel.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="3d9ed-119">[audioSourceLevel](audiosourcelevel.md) collection</span></span>        | <span data-ttu-id="3d9ed-120">Konfiguration für andere Datenquellen.</span><span class="sxs-lookup"><span data-stu-id="3d9ed-120">Level configuration for other sources.</span></span>                                                              |

## <a name="json-representation"></a><span data-ttu-id="3d9ed-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3d9ed-121">JSON representation</span></span>

<span data-ttu-id="3d9ed-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3d9ed-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.participantMixerLevel"
}-->
```json
{
  "ducking": { "@odata.type": "microsoft.graph.audioDuckingConfiguration" },
  "exclusiveMode": true,
  "participant": "String",
  "sourceLevels": [ { "@odata.type": "microsoft.graph.audioSourceLevel" } ]
}
```

## <a name="example---mixer-level"></a><span data-ttu-id="3d9ed-123">Beispiel - Mixer-Ebene</span><span class="sxs-lookup"><span data-stu-id="3d9ed-123">Example - Mixer level</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.participantMixerLevel"
}-->
```json
{
  "ducking": {
    "@odata.type": "#microsoft.graph.audioDuckingParameters",
    "rampActive": 1000,
    "rampInactive": 1000,
    "lowerLevel": 20,
    "upperLevel": 100
  },
  "exclusiveMode": true,
  "participant": "123456W77E24E4D85F80597083CB830",
  "sourceLevels": [
    {
      "@odata.type": "#microsoft.graph.audioSourceLevel",
      "duckOthers": false,
      "level": 100,
      "participant": "8A34A46B3D174ADC8DCEDC4E7D572698"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "participantMixerLevel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/participantmixerlevel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
