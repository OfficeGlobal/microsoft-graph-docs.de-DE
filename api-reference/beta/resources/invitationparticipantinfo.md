---
title: Ressourcentyp invitationParticipantInfo
description: Die **InvitationParticipant** wird verwendet, um die Darstellung eines Satzes von Identitäten zugeordnet einer unterhaltungseinladung zu einer und bietet zusätzliche Einladung-Parameter.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 666de597d40570a567ea88a375ab15d1e5f09038
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573599"
---
# <a name="invitationparticipantinfo-resource-type"></a><span data-ttu-id="c5a18-103">Ressourcentyp invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="c5a18-103">invitationParticipantInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5a18-104">Die **InvitationParticipant** wird verwendet, um die Darstellung eines Satzes von Identitäten zugeordnet einer unterhaltungseinladung zu einer und bietet zusätzliche Einladung-Parameter.</span><span class="sxs-lookup"><span data-stu-id="c5a18-104">The **InvitationParticipant** is used to represent a set of identities associated with a conversation invitation, and provides additional invitation parameters.</span></span>

## <a name="properties"></a><span data-ttu-id="c5a18-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c5a18-105">Properties</span></span>

| <span data-ttu-id="c5a18-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c5a18-106">Property</span></span>                           | <span data-ttu-id="c5a18-107">Typ</span><span class="sxs-lookup"><span data-stu-id="c5a18-107">Type</span></span>                          | <span data-ttu-id="c5a18-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c5a18-108">Description</span></span>                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| <span data-ttu-id="c5a18-109">endpointType</span><span class="sxs-lookup"><span data-stu-id="c5a18-109">endpointType</span></span>                       | <span data-ttu-id="c5a18-110">operationStatus</span><span class="sxs-lookup"><span data-stu-id="c5a18-110">operationStatus</span></span>               | <span data-ttu-id="c5a18-111">Mögliche Werte sind: `default` und `voicemail`.</span><span class="sxs-lookup"><span data-stu-id="c5a18-111">Possible values are: `default`, `voicemail`.</span></span> |
| <span data-ttu-id="c5a18-112">identity</span><span class="sxs-lookup"><span data-stu-id="c5a18-112">identity</span></span>                           | [<span data-ttu-id="c5a18-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="c5a18-113">identitySet</span></span>](identityset.md) | <span data-ttu-id="c5a18-114">Die [IdentitySet](identityset.md) Einladung zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="c5a18-114">The [identitySet](identityset.md) associated with this invitation.</span></span>                   |
| <span data-ttu-id="c5a18-115">languageId</span><span class="sxs-lookup"><span data-stu-id="c5a18-115">languageId</span></span>                         | <span data-ttu-id="c5a18-116">String</span><span class="sxs-lookup"><span data-stu-id="c5a18-116">String</span></span>                        | <span data-ttu-id="c5a18-117">Die Sprache-Kultur-Zeichenfolge.</span><span class="sxs-lookup"><span data-stu-id="c5a18-117">The language culture string.</span></span>                                                                                     |
| <span data-ttu-id="c5a18-118">Region</span><span class="sxs-lookup"><span data-stu-id="c5a18-118">region</span></span>                             | <span data-ttu-id="c5a18-119">String</span><span class="sxs-lookup"><span data-stu-id="c5a18-119">String</span></span>                        | <span data-ttu-id="c5a18-120">Region des Teilnehmers.</span><span class="sxs-lookup"><span data-stu-id="c5a18-120">Region of the participant.</span></span>                                                           |
| <span data-ttu-id="c5a18-121">replacesCallId</span><span class="sxs-lookup"><span data-stu-id="c5a18-121">replacesCallId</span></span>                     | <span data-ttu-id="c5a18-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c5a18-122">String</span></span>                        | <span data-ttu-id="c5a18-123">Optional.</span><span class="sxs-lookup"><span data-stu-id="c5a18-123">Optional.</span></span> <span data-ttu-id="c5a18-124">Der Aufruf der das Ziel Idenity derzeit gehört.</span><span class="sxs-lookup"><span data-stu-id="c5a18-124">The call which the target idenity is currently a part of.</span></span> <span data-ttu-id="c5a18-125">Sobald der Teilnehmer hinzugefügt wird, wird dieses Anrufs gelöscht werden.</span><span class="sxs-lookup"><span data-stu-id="c5a18-125">This call will be dropped once the participant is added.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c5a18-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c5a18-126">JSON representation</span></span>

<span data-ttu-id="c5a18-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c5a18-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.invitationParticipantInfo"
}-->
```json
{
  "endpointType": "operationStatus",
  "identity": {"@odata.type": "#microsoft.graph.identitySet"},
  "languageId": "String",
  "region": "String",
  "replacesCallId": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "invitationParticipantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/invitationparticipantinfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
