---
title: Ressourcentyp invitationParticipantInfo
description: Die **InvitationParticipant** wird verwendet, um die Darstellung eines Satzes von Identitäten zugeordnet einer unterhaltungseinladung zu einer und bietet zusätzliche Einladung-Parameter.
ms.openlocfilehash: 8b00625dad1c41121b0359586742301e16d163fc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060513"
---
# <a name="invitationparticipantinfo-resource-type"></a><span data-ttu-id="92198-103">Ressourcentyp invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="92198-103">invitationParticipantInfo resource type</span></span>

> <span data-ttu-id="92198-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="92198-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="92198-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="92198-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="92198-106">Die **InvitationParticipant** wird verwendet, um die Darstellung eines Satzes von Identitäten zugeordnet einer unterhaltungseinladung zu einer und bietet zusätzliche Einladung-Parameter.</span><span class="sxs-lookup"><span data-stu-id="92198-106">The **InvitationParticipant** is used to represent a set of identities associated with a conversation invitation, and provides additional invitation parameters.</span></span>

## <a name="properties"></a><span data-ttu-id="92198-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="92198-107">Properties</span></span>

| <span data-ttu-id="92198-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="92198-108">Property</span></span>                           | <span data-ttu-id="92198-109">Typ</span><span class="sxs-lookup"><span data-stu-id="92198-109">Type</span></span>                          | <span data-ttu-id="92198-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="92198-110">Description</span></span>                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| <span data-ttu-id="92198-111">endpointType</span><span class="sxs-lookup"><span data-stu-id="92198-111">endpointType</span></span>                       | <span data-ttu-id="92198-112">String</span><span class="sxs-lookup"><span data-stu-id="92198-112">String</span></span>                        | <span data-ttu-id="92198-113">Mögliche Werte: `default`, `voicemail`.</span><span class="sxs-lookup"><span data-stu-id="92198-113">Possible values are: `default`, `voicemail`.</span></span> |
| <span data-ttu-id="92198-114">identity</span><span class="sxs-lookup"><span data-stu-id="92198-114">identity</span></span>                           | [<span data-ttu-id="92198-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="92198-115">identitySet</span></span>](identityset.md) | <span data-ttu-id="92198-116">Die [IdentitySet](identityset.md) Einladung zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="92198-116">The [identitySet](identityset.md) associated with this invitation.</span></span>                   |
| <span data-ttu-id="92198-117">languageId</span><span class="sxs-lookup"><span data-stu-id="92198-117">languageId</span></span>                         | <span data-ttu-id="92198-118">String</span><span class="sxs-lookup"><span data-stu-id="92198-118">String</span></span>                        | <span data-ttu-id="92198-119">Die Sprache-Kultur-Zeichenfolge.</span><span class="sxs-lookup"><span data-stu-id="92198-119">The language culture string.</span></span>                                                                                     |
| <span data-ttu-id="92198-120">Region</span><span class="sxs-lookup"><span data-stu-id="92198-120">region</span></span>                             | <span data-ttu-id="92198-121">String</span><span class="sxs-lookup"><span data-stu-id="92198-121">String</span></span>                        | <span data-ttu-id="92198-122">Region des Teilnehmers.</span><span class="sxs-lookup"><span data-stu-id="92198-122">Region of the participant.</span></span>                                                           |
| <span data-ttu-id="92198-123">replacesCallId</span><span class="sxs-lookup"><span data-stu-id="92198-123">replacesCallId</span></span>                     | <span data-ttu-id="92198-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="92198-124">String</span></span>                        | <span data-ttu-id="92198-125">Optional.</span><span class="sxs-lookup"><span data-stu-id="92198-125">Optional.</span></span> <span data-ttu-id="92198-126">Der Aufruf der das Ziel Idenity derzeit gehört.</span><span class="sxs-lookup"><span data-stu-id="92198-126">The call which the target idenity is currently a part of.</span></span> <span data-ttu-id="92198-127">Sobald der Teilnehmer hinzugefügt wird, wird dieses Anrufs gelöscht werden.</span><span class="sxs-lookup"><span data-stu-id="92198-127">This call will be dropped once the participant is added.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="92198-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="92198-128">JSON representation</span></span>

<span data-ttu-id="92198-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="92198-129">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "invitationParticipantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
