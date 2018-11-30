---
title: Ressourcentyp participantMixerLevel
description: Konfiguration der Mixer Ebenen zur angegebenen audio-Teilnehmer
ms.openlocfilehash: 920c22cf423391d2efcdf7177fdc7491250d0f19
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065793"
---
# <a name="participantmixerlevel-resource-type"></a><span data-ttu-id="b7b1a-103">Ressourcentyp participantMixerLevel</span><span class="sxs-lookup"><span data-stu-id="b7b1a-103">participantMixerLevel resource type</span></span>

> <span data-ttu-id="b7b1a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b7b1a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b7b1a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b7b1a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b7b1a-106">Konfiguration der Mixer Ebenen zur angegebenen audio-Teilnehmer</span><span class="sxs-lookup"><span data-stu-id="b7b1a-106">Configuration of mixer levels for given audio participant</span></span>

## <a name="properties"></a><span data-ttu-id="b7b1a-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b7b1a-107">Properties</span></span>

| <span data-ttu-id="b7b1a-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b7b1a-108">Property</span></span>               | <span data-ttu-id="b7b1a-109">Typ</span><span class="sxs-lookup"><span data-stu-id="b7b1a-109">Type</span></span>                                                      | <span data-ttu-id="b7b1a-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b7b1a-110">Description</span></span>                                                                                         |
| :--------------------- | :-------------------------------------------------------- | :---------------------------------------------------------------------------------------------------|
| <span data-ttu-id="b7b1a-111">Vermeiden von</span><span class="sxs-lookup"><span data-stu-id="b7b1a-111">ducking</span></span>                | [<span data-ttu-id="b7b1a-112">audioDuckingConfiguration</span><span class="sxs-lookup"><span data-stu-id="b7b1a-112">audioDuckingConfiguration</span></span>](audioduckingconfiguration.md) | <span data-ttu-id="b7b1a-113">Konfiguration der benutzerdefinierte Mischung (welchen Phasen an- und Abmelden) andere Quellen für diese Teilnehmer zu vermeiden.</span><span class="sxs-lookup"><span data-stu-id="b7b1a-113">Configuration of ducking (phasing in and out) of other sources for this partipant custom mix.</span></span>       |
| <span data-ttu-id="b7b1a-114">exclusiveMode</span><span class="sxs-lookup"><span data-stu-id="b7b1a-114">exclusiveMode</span></span>          | <span data-ttu-id="b7b1a-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="b7b1a-115">boolean</span></span>                                                   | <span data-ttu-id="b7b1a-116">Gibt an, ob von der Mischung Quellen ohne explizite Quellebene entfernt werden soll.</span><span class="sxs-lookup"><span data-stu-id="b7b1a-116">Whether sources without explicit source level should be removed from the mix.</span></span>                       |
| <span data-ttu-id="b7b1a-117">Teilnehmer</span><span class="sxs-lookup"><span data-stu-id="b7b1a-117">participant</span></span>            | <span data-ttu-id="b7b1a-118">String</span><span class="sxs-lookup"><span data-stu-id="b7b1a-118">String</span></span>                                                    | <span data-ttu-id="b7b1a-119">Die Teilnehmer für den Mischer konfiguriert wird.</span><span class="sxs-lookup"><span data-stu-id="b7b1a-119">The participant for whom the mixer is being configured.</span></span>                                             |
| <span data-ttu-id="b7b1a-120">sourceLevels</span><span class="sxs-lookup"><span data-stu-id="b7b1a-120">sourceLevels</span></span>           | <span data-ttu-id="b7b1a-121">[AudioSourceLevel](audiosourcelevel.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="b7b1a-121">[audioSourceLevel](audiosourcelevel.md) collection</span></span>        | <span data-ttu-id="b7b1a-122">Konfiguration für andere Datenquellen.</span><span class="sxs-lookup"><span data-stu-id="b7b1a-122">Level configuration for other sources.</span></span>                                                              |

## <a name="json-representation"></a><span data-ttu-id="b7b1a-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b7b1a-123">JSON representation</span></span>

<span data-ttu-id="b7b1a-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b7b1a-124">The following is a JSON representation of the resource.</span></span>

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

## <a name="example---mixer-level"></a><span data-ttu-id="b7b1a-125">Beispiel - Mixer-Ebene</span><span class="sxs-lookup"><span data-stu-id="b7b1a-125">Example - Mixer level</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "participantMixerLevel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
