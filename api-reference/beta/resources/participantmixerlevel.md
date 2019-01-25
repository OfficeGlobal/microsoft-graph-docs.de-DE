---
title: Ressourcentyp participantMixerLevel
description: Konfiguration der Mixer Ebenen zur angegebenen audio-Teilnehmer
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 14804e02766e375568fac03cb97d2eaf76142353
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513767"
---
# <a name="participantmixerlevel-resource-type"></a><span data-ttu-id="e550e-103">Ressourcentyp participantMixerLevel</span><span class="sxs-lookup"><span data-stu-id="e550e-103">participantMixerLevel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e550e-104">Konfiguration der Mixer Ebenen zur angegebenen audio-Teilnehmer</span><span class="sxs-lookup"><span data-stu-id="e550e-104">Configuration of mixer levels for given audio participant</span></span>

## <a name="properties"></a><span data-ttu-id="e550e-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e550e-105">Properties</span></span>

| <span data-ttu-id="e550e-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e550e-106">Property</span></span>               | <span data-ttu-id="e550e-107">Typ</span><span class="sxs-lookup"><span data-stu-id="e550e-107">Type</span></span>                                                      | <span data-ttu-id="e550e-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e550e-108">Description</span></span>                                                                                         |
| :--------------------- | :-------------------------------------------------------- | :---------------------------------------------------------------------------------------------------|
| <span data-ttu-id="e550e-109">Vermeiden von</span><span class="sxs-lookup"><span data-stu-id="e550e-109">ducking</span></span>                | [<span data-ttu-id="e550e-110">audioDuckingConfiguration</span><span class="sxs-lookup"><span data-stu-id="e550e-110">audioDuckingConfiguration</span></span>](audioduckingconfiguration.md) | <span data-ttu-id="e550e-111">Konfiguration der benutzerdefinierte Mischung (welchen Phasen an- und Abmelden) andere Quellen für diese Teilnehmer zu vermeiden.</span><span class="sxs-lookup"><span data-stu-id="e550e-111">Configuration of ducking (phasing in and out) of other sources for this partipant custom mix.</span></span>       |
| <span data-ttu-id="e550e-112">exclusiveMode</span><span class="sxs-lookup"><span data-stu-id="e550e-112">exclusiveMode</span></span>          | <span data-ttu-id="e550e-113">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e550e-113">boolean</span></span>                                                   | <span data-ttu-id="e550e-114">Gibt an, ob von der Mischung Quellen ohne explizite Quellebene entfernt werden soll.</span><span class="sxs-lookup"><span data-stu-id="e550e-114">Whether sources without explicit source level should be removed from the mix.</span></span>                       |
| <span data-ttu-id="e550e-115">Teilnehmer</span><span class="sxs-lookup"><span data-stu-id="e550e-115">participant</span></span>            | <span data-ttu-id="e550e-116">String</span><span class="sxs-lookup"><span data-stu-id="e550e-116">String</span></span>                                                    | <span data-ttu-id="e550e-117">Die Teilnehmer für den Mischer konfiguriert wird.</span><span class="sxs-lookup"><span data-stu-id="e550e-117">The participant for whom the mixer is being configured.</span></span>                                             |
| <span data-ttu-id="e550e-118">sourceLevels</span><span class="sxs-lookup"><span data-stu-id="e550e-118">sourceLevels</span></span>           | <span data-ttu-id="e550e-119">[AudioSourceLevel](audiosourcelevel.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="e550e-119">[audioSourceLevel](audiosourcelevel.md) collection</span></span>        | <span data-ttu-id="e550e-120">Konfiguration für andere Datenquellen.</span><span class="sxs-lookup"><span data-stu-id="e550e-120">Level configuration for other sources.</span></span>                                                              |

## <a name="json-representation"></a><span data-ttu-id="e550e-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e550e-121">JSON representation</span></span>

<span data-ttu-id="e550e-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e550e-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.participantMixerLevel"
}-->
```json
{
  "ducking": { "@odata.type": "#microsoft.graph.audioDuckingConfiguration" },
  "exclusiveMode": true,
  "participant": "String",
  "sourceLevels": [ { "@odata.type": "#microsoft.graph.audioSourceLevel" } ]
}
```

## <a name="example---mixer-level"></a><span data-ttu-id="e550e-123">Beispiel - Mixer-Ebene</span><span class="sxs-lookup"><span data-stu-id="e550e-123">Example - Mixer level</span></span>

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
