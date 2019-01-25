---
title: Ressourcentyp meetingParticipantInfo
description: Informationen über einen Teilnehmer an einer Besprechung.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 1ba727344b1f653125a482b592e7d28c11d1d3d5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515027"
---
# <a name="meetingparticipantinfo-resource-type"></a><span data-ttu-id="c6ece-103">Ressourcentyp meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="c6ece-103">meetingParticipantInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6ece-104">Informationen über einen Teilnehmer an einer Besprechung.</span><span class="sxs-lookup"><span data-stu-id="c6ece-104">Information about a participant in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="c6ece-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c6ece-105">Properties</span></span>

| <span data-ttu-id="c6ece-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c6ece-106">Property</span></span>       | <span data-ttu-id="c6ece-107">Typ</span><span class="sxs-lookup"><span data-stu-id="c6ece-107">Type</span></span>                          | <span data-ttu-id="c6ece-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c6ece-108">Description</span></span>                              |
|:---------------|:------------------------------|:-----------------------------------------|
| <span data-ttu-id="c6ece-109">[-Identity]</span><span class="sxs-lookup"><span data-stu-id="c6ece-109">identity</span></span>       | [<span data-ttu-id="c6ece-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="c6ece-110">identitySet</span></span>](identityset.md) | <span data-ttu-id="c6ece-111">Identitätsinformationen des Teilnehmers.</span><span class="sxs-lookup"><span data-stu-id="c6ece-111">Identity information of the participant.</span></span> |
| <span data-ttu-id="c6ece-112">UPN</span><span class="sxs-lookup"><span data-stu-id="c6ece-112">upn</span></span>            | <span data-ttu-id="c6ece-113">String</span><span class="sxs-lookup"><span data-stu-id="c6ece-113">String</span></span>                        | <span data-ttu-id="c6ece-114">Benutzerprinzipalname des Teilnehmers.</span><span class="sxs-lookup"><span data-stu-id="c6ece-114">User principal name of the participant.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="c6ece-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c6ece-115">JSON representation</span></span>

<span data-ttu-id="c6ece-116">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c6ece-116">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "meetingParticipantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/meetingparticipantinfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
