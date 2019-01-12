---
title: Ressourcentyp audioConferencing
description: Stellt Access Telefoninformationen für einen OnlineMeeting.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: cd65b094a17ad3fa470471c3ed6dd3908367e578
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977507"
---
# <a name="audioconferencing-resource-type"></a><span data-ttu-id="ef0ab-103">Ressourcentyp audioConferencing</span><span class="sxs-lookup"><span data-stu-id="ef0ab-103">audioConferencing resource type</span></span>

> <span data-ttu-id="ef0ab-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ef0ab-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ef0ab-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ef0ab-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ef0ab-106">Stellt Access Telefoninformationen für einen [OnlineMeeting](onlinemeeting.md).</span><span class="sxs-lookup"><span data-stu-id="ef0ab-106">Represents phone access information for an [onlineMeeting](onlinemeeting.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ef0ab-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ef0ab-107">Properties</span></span>

| <span data-ttu-id="ef0ab-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ef0ab-108">Property</span></span>            | <span data-ttu-id="ef0ab-109">Typ</span><span class="sxs-lookup"><span data-stu-id="ef0ab-109">Type</span></span>    | <span data-ttu-id="ef0ab-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ef0ab-110">Description</span></span>                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="ef0ab-111">dialinUrl</span><span class="sxs-lookup"><span data-stu-id="ef0ab-111">dialinUrl</span></span>           | <span data-ttu-id="ef0ab-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ef0ab-112">String</span></span>  | <span data-ttu-id="ef0ab-113">Eine URL, die extern zugängliche Webseite, die Einwahlinformationen enthält.</span><span class="sxs-lookup"><span data-stu-id="ef0ab-113">A URL to the externally-accessible web page that contains dial-in information.</span></span> |
| <span data-ttu-id="ef0ab-114">leaderPasscode</span><span class="sxs-lookup"><span data-stu-id="ef0ab-114">leaderPasscode</span></span>      | <span data-ttu-id="ef0ab-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ef0ab-115">String</span></span>  | <span data-ttu-id="ef0ab-116">Der Leiter Kennwort zum Verbinden mit dem Audio Conference Provider erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ef0ab-116">The leader password required to connect to the Audio Conference Provider.</span></span>      |
| <span data-ttu-id="ef0ab-117">participantPasscode</span><span class="sxs-lookup"><span data-stu-id="ef0ab-117">participantPasscode</span></span> | <span data-ttu-id="ef0ab-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ef0ab-118">String</span></span>  | <span data-ttu-id="ef0ab-119">Die Teilnehmer das Kennwort zum Verbinden mit dem Audio Conference Provider erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ef0ab-119">The participant password required to connect to the Audio Conference Provider.</span></span> |
| <span data-ttu-id="ef0ab-120">tollFreeNumber</span><span class="sxs-lookup"><span data-stu-id="ef0ab-120">tollFreeNumber</span></span>      | <span data-ttu-id="ef0ab-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ef0ab-121">String</span></span>  | <span data-ttu-id="ef0ab-122">Die gebührenfreie Telefonnummer für die Audio Conference Provider die Verbindung.</span><span class="sxs-lookup"><span data-stu-id="ef0ab-122">The toll-free number to connect to the Audio Conference Provider.</span></span>              |
| <span data-ttu-id="ef0ab-123">tollNumber</span><span class="sxs-lookup"><span data-stu-id="ef0ab-123">tollNumber</span></span>          | <span data-ttu-id="ef0ab-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ef0ab-124">String</span></span>  | <span data-ttu-id="ef0ab-125">Die gebührenpflichtige Telefonnummer für die Audio Conference Provider die Verbindung.</span><span class="sxs-lookup"><span data-stu-id="ef0ab-125">The toll number to connect to the Audio Conference Provider.</span></span>                   |

## <a name="json-representation"></a><span data-ttu-id="ef0ab-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ef0ab-126">JSON representation</span></span>

<span data-ttu-id="ef0ab-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ef0ab-127">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "audioConferencing resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
