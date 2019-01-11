---
title: Ressourcentyp audioSourceLevel
description: Konfiguration für andere Datenquellen.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: adf3c4805271d0a8d02d25fc8e7ecb547db10215
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880640"
---
# <a name="audiosourcelevel-resource-type"></a><span data-ttu-id="976ec-103">Ressourcentyp audioSourceLevel</span><span class="sxs-lookup"><span data-stu-id="976ec-103">audioSourceLevel resource type</span></span>

> <span data-ttu-id="976ec-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="976ec-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="976ec-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="976ec-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="976ec-106">Konfiguration für andere Datenquellen.</span><span class="sxs-lookup"><span data-stu-id="976ec-106">Level configuration for other sources.</span></span>

## <a name="properties"></a><span data-ttu-id="976ec-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="976ec-107">Properties</span></span>

| <span data-ttu-id="976ec-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="976ec-108">Property</span></span>               | <span data-ttu-id="976ec-109">Typ</span><span class="sxs-lookup"><span data-stu-id="976ec-109">Type</span></span>    | <span data-ttu-id="976ec-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="976ec-110">Description</span></span>                                                                                         |
| :--------------------- | :------ | :---------------------------------------------------------------------------------------------------|
| <span data-ttu-id="976ec-111">duckOthers</span><span class="sxs-lookup"><span data-stu-id="976ec-111">duckOthers</span></span>             | <span data-ttu-id="976ec-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="976ec-112">Boolean</span></span> | <span data-ttu-id="976ec-113">Dieser Quelle zu anderen Quellen, während es aktiv Wildenten ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="976ec-113">Enables this source to duck other sources while active.</span></span> <span data-ttu-id="976ec-114">Wenn auf true festgelegt ist, vermeiden Ebene festgelegt ist festgelegt werden soll.</span><span class="sxs-lookup"><span data-stu-id="976ec-114">If set to true, ducking level has to be set.</span></span>|
| <span data-ttu-id="976ec-115">Ebene</span><span class="sxs-lookup"><span data-stu-id="976ec-115">level</span></span>                  | <span data-ttu-id="976ec-116">Int64</span><span class="sxs-lookup"><span data-stu-id="976ec-116">Int64</span></span>   | <span data-ttu-id="976ec-117">Ebene der Quelle vermeiden, wenn `duckOthers` auf festgelegt ist `true`.</span><span class="sxs-lookup"><span data-stu-id="976ec-117">Ducking level of the source if `duckOthers` is set to `true`.</span></span>                                     |
| <span data-ttu-id="976ec-118">Teilnehmer</span><span class="sxs-lookup"><span data-stu-id="976ec-118">participant</span></span>            | <span data-ttu-id="976ec-119">String</span><span class="sxs-lookup"><span data-stu-id="976ec-119">String</span></span>  | <span data-ttu-id="976ec-120">Die Teilnehmer Audiostream von Quelle.</span><span class="sxs-lookup"><span data-stu-id="976ec-120">The source participant audio stream.</span></span>                                                                |

## <a name="json-representation"></a><span data-ttu-id="976ec-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="976ec-121">JSON representation</span></span>

<span data-ttu-id="976ec-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="976ec-122">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "audioSourceLevel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
