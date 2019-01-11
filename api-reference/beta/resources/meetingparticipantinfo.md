---
title: Ressourcentyp meetingParticipantInfo
description: Informationen über einen Teilnehmer an einer Besprechung.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: d7b5ae17bd3bfb566bce0da9814b86aab98173da
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834258"
---
# <a name="meetingparticipantinfo-resource-type"></a><span data-ttu-id="bfb10-103">Ressourcentyp meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="bfb10-103">meetingParticipantInfo resource type</span></span>

> <span data-ttu-id="bfb10-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="bfb10-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bfb10-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bfb10-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bfb10-106">Informationen über einen Teilnehmer an einer Besprechung.</span><span class="sxs-lookup"><span data-stu-id="bfb10-106">Information about a participant in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="bfb10-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bfb10-107">Properties</span></span>

| <span data-ttu-id="bfb10-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bfb10-108">Property</span></span>       | <span data-ttu-id="bfb10-109">Typ</span><span class="sxs-lookup"><span data-stu-id="bfb10-109">Type</span></span>                          | <span data-ttu-id="bfb10-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bfb10-110">Description</span></span>                              |
|:---------------|:------------------------------|:-----------------------------------------|
| <span data-ttu-id="bfb10-111">Identität</span><span class="sxs-lookup"><span data-stu-id="bfb10-111">identity</span></span>       | [<span data-ttu-id="bfb10-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="bfb10-112">identitySet</span></span>](identityset.md) | <span data-ttu-id="bfb10-113">Identitätsinformationen des Teilnehmers.</span><span class="sxs-lookup"><span data-stu-id="bfb10-113">Identity information of the participant.</span></span> |
| <span data-ttu-id="bfb10-114">UPN</span><span class="sxs-lookup"><span data-stu-id="bfb10-114">upn</span></span>            | <span data-ttu-id="bfb10-115">String</span><span class="sxs-lookup"><span data-stu-id="bfb10-115">String</span></span>                        | <span data-ttu-id="bfb10-116">Benutzerprinzipalname des Teilnehmers.</span><span class="sxs-lookup"><span data-stu-id="bfb10-116">User principal name of the participant.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="bfb10-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bfb10-117">JSON representation</span></span>

<span data-ttu-id="bfb10-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="bfb10-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingParticipantInfo"
}-->
```json
{
  "identity": {"@odata.type": "#microsoft.graph.identitySet"},
  "upn": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingParticipantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
