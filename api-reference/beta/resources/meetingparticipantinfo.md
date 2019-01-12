---
title: Ressourcentyp meetingParticipantInfo
description: Informationen über einen Teilnehmer an einer Besprechung.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 409cf7eff4b1151a0ded11674fcde36a519f0e7f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924482"
---
# <a name="meetingparticipantinfo-resource-type"></a><span data-ttu-id="f7ac0-103">Ressourcentyp meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="f7ac0-103">meetingParticipantInfo resource type</span></span>

> <span data-ttu-id="f7ac0-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f7ac0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f7ac0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f7ac0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f7ac0-106">Informationen über einen Teilnehmer an einer Besprechung.</span><span class="sxs-lookup"><span data-stu-id="f7ac0-106">Information about a participant in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="f7ac0-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f7ac0-107">Properties</span></span>

| <span data-ttu-id="f7ac0-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f7ac0-108">Property</span></span>       | <span data-ttu-id="f7ac0-109">Typ</span><span class="sxs-lookup"><span data-stu-id="f7ac0-109">Type</span></span>                          | <span data-ttu-id="f7ac0-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f7ac0-110">Description</span></span>                              |
|:---------------|:------------------------------|:-----------------------------------------|
| <span data-ttu-id="f7ac0-111">Identität</span><span class="sxs-lookup"><span data-stu-id="f7ac0-111">identity</span></span>       | [<span data-ttu-id="f7ac0-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="f7ac0-112">identitySet</span></span>](identityset.md) | <span data-ttu-id="f7ac0-113">Identitätsinformationen des Teilnehmers.</span><span class="sxs-lookup"><span data-stu-id="f7ac0-113">Identity information of the participant.</span></span> |
| <span data-ttu-id="f7ac0-114">UPN</span><span class="sxs-lookup"><span data-stu-id="f7ac0-114">upn</span></span>            | <span data-ttu-id="f7ac0-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f7ac0-115">String</span></span>                        | <span data-ttu-id="f7ac0-116">Benutzerprinzipalname des Teilnehmers.</span><span class="sxs-lookup"><span data-stu-id="f7ac0-116">User principal name of the participant.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="f7ac0-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f7ac0-117">JSON representation</span></span>

<span data-ttu-id="f7ac0-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f7ac0-118">The following is a JSON representation of the resource.</span></span>

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
