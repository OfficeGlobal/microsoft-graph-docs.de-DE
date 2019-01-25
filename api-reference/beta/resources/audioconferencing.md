---
title: Ressourcentyp audioConferencing
description: Stellt Access Telefoninformationen für einen OnlineMeeting.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: cb822f2049d84f9a2460370f05d5dfc85c347f15
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522175"
---
# <a name="audioconferencing-resource-type"></a><span data-ttu-id="9babd-103">Ressourcentyp audioConferencing</span><span class="sxs-lookup"><span data-stu-id="9babd-103">audioConferencing resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9babd-104">Stellt Access Telefoninformationen für einen [OnlineMeeting](onlinemeeting.md).</span><span class="sxs-lookup"><span data-stu-id="9babd-104">Represents phone access information for an [onlineMeeting](onlinemeeting.md).</span></span>

## <a name="properties"></a><span data-ttu-id="9babd-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9babd-105">Properties</span></span>

| <span data-ttu-id="9babd-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9babd-106">Property</span></span>            | <span data-ttu-id="9babd-107">Typ</span><span class="sxs-lookup"><span data-stu-id="9babd-107">Type</span></span>    | <span data-ttu-id="9babd-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9babd-108">Description</span></span>                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="9babd-109">dialinUrl</span><span class="sxs-lookup"><span data-stu-id="9babd-109">dialinUrl</span></span>           | <span data-ttu-id="9babd-110">String</span><span class="sxs-lookup"><span data-stu-id="9babd-110">String</span></span>  | <span data-ttu-id="9babd-111">Eine URL, die extern zugängliche Webseite, die Einwahlinformationen enthält.</span><span class="sxs-lookup"><span data-stu-id="9babd-111">A URL to the externally-accessible web page that contains dial-in information.</span></span> |
| <span data-ttu-id="9babd-112">leaderPasscode</span><span class="sxs-lookup"><span data-stu-id="9babd-112">leaderPasscode</span></span>      | <span data-ttu-id="9babd-113">String</span><span class="sxs-lookup"><span data-stu-id="9babd-113">String</span></span>  | <span data-ttu-id="9babd-114">Der Leiter Kennwort zum Verbinden mit dem Audio Conference Provider erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9babd-114">The leader password required to connect to the Audio Conference Provider.</span></span>      |
| <span data-ttu-id="9babd-115">participantPasscode</span><span class="sxs-lookup"><span data-stu-id="9babd-115">participantPasscode</span></span> | <span data-ttu-id="9babd-116">String</span><span class="sxs-lookup"><span data-stu-id="9babd-116">String</span></span>  | <span data-ttu-id="9babd-117">Die Teilnehmer das Kennwort zum Verbinden mit dem Audio Conference Provider erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9babd-117">The participant password required to connect to the Audio Conference Provider.</span></span> |
| <span data-ttu-id="9babd-118">tollFreeNumber</span><span class="sxs-lookup"><span data-stu-id="9babd-118">tollFreeNumber</span></span>      | <span data-ttu-id="9babd-119">String</span><span class="sxs-lookup"><span data-stu-id="9babd-119">String</span></span>  | <span data-ttu-id="9babd-120">Die gebührenfreie Telefonnummer für die Audio Conference Provider die Verbindung.</span><span class="sxs-lookup"><span data-stu-id="9babd-120">The toll-free number to connect to the Audio Conference Provider.</span></span>              |
| <span data-ttu-id="9babd-121">tollNumber</span><span class="sxs-lookup"><span data-stu-id="9babd-121">tollNumber</span></span>          | <span data-ttu-id="9babd-122">String</span><span class="sxs-lookup"><span data-stu-id="9babd-122">String</span></span>  | <span data-ttu-id="9babd-123">Die gebührenpflichtige Telefonnummer für die Audio Conference Provider die Verbindung.</span><span class="sxs-lookup"><span data-stu-id="9babd-123">The toll number to connect to the Audio Conference Provider.</span></span>                   |

## <a name="json-representation"></a><span data-ttu-id="9babd-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9babd-124">JSON representation</span></span>

<span data-ttu-id="9babd-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9babd-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioConferencing"
}-->
```json
{
  "dialinUrl": "String",
  "leaderPasscode": "String",
  "participantPasscode": "String",
  "tollFreeNumber": "String",
  "tollNumber": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "audioConferencing resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/audioconferencing.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
