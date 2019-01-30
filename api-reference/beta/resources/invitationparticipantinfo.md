---
title: Ressourcentyp invitationParticipantInfo
description: Die **InvitationParticipant** wird verwendet, um die Darstellung eines Satzes von Identitäten zugeordnet einer unterhaltungseinladung zu einer und bietet zusätzliche Einladung-Parameter.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: cb20dde1a74472695755e65dc404a6709f79c8b0
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641918"
---
# <a name="invitationparticipantinfo-resource-type"></a><span data-ttu-id="4cf8c-103">Ressourcentyp invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="4cf8c-103">invitationParticipantInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4cf8c-104">Die **InvitationParticipant** wird verwendet, um die Darstellung eines Satzes von Identitäten zugeordnet einer unterhaltungseinladung zu einer und bietet zusätzliche Einladung-Parameter.</span><span class="sxs-lookup"><span data-stu-id="4cf8c-104">The **InvitationParticipant** is used to represent a set of identities associated with a conversation invitation, and provides additional invitation parameters.</span></span>

## <a name="properties"></a><span data-ttu-id="4cf8c-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4cf8c-105">Properties</span></span>

| <span data-ttu-id="4cf8c-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4cf8c-106">Property</span></span>                           | <span data-ttu-id="4cf8c-107">Typ</span><span class="sxs-lookup"><span data-stu-id="4cf8c-107">Type</span></span>                          | <span data-ttu-id="4cf8c-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4cf8c-108">Description</span></span>                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| <span data-ttu-id="4cf8c-109">endpointType</span><span class="sxs-lookup"><span data-stu-id="4cf8c-109">endpointType</span></span>                       | <span data-ttu-id="4cf8c-110">String</span><span class="sxs-lookup"><span data-stu-id="4cf8c-110">String</span></span>                        | <span data-ttu-id="4cf8c-111">Mögliche Werte: `default`, `voicemail`.</span><span class="sxs-lookup"><span data-stu-id="4cf8c-111">Possible values are: `default`, `voicemail`.</span></span> |
| <span data-ttu-id="4cf8c-112">identity</span><span class="sxs-lookup"><span data-stu-id="4cf8c-112">identity</span></span>                           | [<span data-ttu-id="4cf8c-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="4cf8c-113">identitySet</span></span>](identityset.md) | <span data-ttu-id="4cf8c-114">Die [IdentitySet](identityset.md) Einladung zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="4cf8c-114">The [identitySet](identityset.md) associated with this invitation.</span></span>                   |
| <span data-ttu-id="4cf8c-115">languageId</span><span class="sxs-lookup"><span data-stu-id="4cf8c-115">languageId</span></span>                         | <span data-ttu-id="4cf8c-116">String</span><span class="sxs-lookup"><span data-stu-id="4cf8c-116">String</span></span>                        | <span data-ttu-id="4cf8c-117">Die Sprache-Kultur-Zeichenfolge.</span><span class="sxs-lookup"><span data-stu-id="4cf8c-117">The language culture string.</span></span>                                                                                     |
| <span data-ttu-id="4cf8c-118">Region</span><span class="sxs-lookup"><span data-stu-id="4cf8c-118">region</span></span>                             | <span data-ttu-id="4cf8c-119">String</span><span class="sxs-lookup"><span data-stu-id="4cf8c-119">String</span></span>                        | <span data-ttu-id="4cf8c-120">Region des Teilnehmers.</span><span class="sxs-lookup"><span data-stu-id="4cf8c-120">Region of the participant.</span></span>                                                           |
| <span data-ttu-id="4cf8c-121">replacesCallId</span><span class="sxs-lookup"><span data-stu-id="4cf8c-121">replacesCallId</span></span>                     | <span data-ttu-id="4cf8c-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4cf8c-122">String</span></span>                        | <span data-ttu-id="4cf8c-123">Optional.</span><span class="sxs-lookup"><span data-stu-id="4cf8c-123">Optional.</span></span> <span data-ttu-id="4cf8c-124">Der Aufruf der das Ziel Idenity derzeit gehört.</span><span class="sxs-lookup"><span data-stu-id="4cf8c-124">The call which the target idenity is currently a part of.</span></span> <span data-ttu-id="4cf8c-125">Sobald der Teilnehmer hinzugefügt wird, wird dieses Anrufs gelöscht werden.</span><span class="sxs-lookup"><span data-stu-id="4cf8c-125">This call will be dropped once the participant is added.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4cf8c-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4cf8c-126">JSON representation</span></span>

<span data-ttu-id="4cf8c-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4cf8c-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.invitationParticipantInfo"
}-->
```json
{
  "endpointType": "default | voicemail",
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
