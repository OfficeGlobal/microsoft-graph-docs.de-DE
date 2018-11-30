---
title: Ressourcentyp meetingParticipantInfo
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: 1d9c22924f8f05255b5e01bad4bbcd6ae5957ffe
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061808"
---
# <a name="meetingparticipantinfo-resource-type"></a><span data-ttu-id="56a3b-103">Ressourcentyp meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="56a3b-103">meetingParticipantInfo resource type</span></span>

> <span data-ttu-id="56a3b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="56a3b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="56a3b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="56a3b-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="properties"></a><span data-ttu-id="56a3b-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="56a3b-106">Properties</span></span>

| <span data-ttu-id="56a3b-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="56a3b-107">Property</span></span>       | <span data-ttu-id="56a3b-108">Typ</span><span class="sxs-lookup"><span data-stu-id="56a3b-108">Type</span></span>                          | <span data-ttu-id="56a3b-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="56a3b-109">Description</span></span>                              |
|:---------------|:------------------------------|:-----------------------------------------|
| <span data-ttu-id="56a3b-110">Identität</span><span class="sxs-lookup"><span data-stu-id="56a3b-110">identity</span></span>       | [<span data-ttu-id="56a3b-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="56a3b-111">identitySet</span></span>](identityset.md) | <span data-ttu-id="56a3b-112">Identitätsinformationen des Teilnehmers.</span><span class="sxs-lookup"><span data-stu-id="56a3b-112">Identity information of the participant.</span></span> |
| <span data-ttu-id="56a3b-113">UPN</span><span class="sxs-lookup"><span data-stu-id="56a3b-113">upn</span></span>            | <span data-ttu-id="56a3b-114">String</span><span class="sxs-lookup"><span data-stu-id="56a3b-114">String</span></span>                        | <span data-ttu-id="56a3b-115">Benutzerprinzipalname des Teilnehmers.</span><span class="sxs-lookup"><span data-stu-id="56a3b-115">User principal name of the participant.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="56a3b-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="56a3b-116">JSON representation</span></span>

<span data-ttu-id="56a3b-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="56a3b-117">The following is a JSON representation of the resource.</span></span>

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
