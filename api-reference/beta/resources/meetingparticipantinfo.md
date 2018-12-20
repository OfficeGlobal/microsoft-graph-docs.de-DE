---
title: Ressourcentyp meetingParticipantInfo
description: Informationen über einen Teilnehmer an einer Besprechung.
author: VinodRavichandran
ms.openlocfilehash: 2bbb410ea26640ec05d66b5beb0c4b4ea24a42bd
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380198"
---
# <a name="meetingparticipantinfo-resource-type"></a><span data-ttu-id="4000f-103">Ressourcentyp meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="4000f-103">meetingParticipantInfo resource type</span></span>

> <span data-ttu-id="4000f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4000f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4000f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4000f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4000f-106">Informationen über einen Teilnehmer an einer Besprechung.</span><span class="sxs-lookup"><span data-stu-id="4000f-106">Information about a participant in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="4000f-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4000f-107">Properties</span></span>

| <span data-ttu-id="4000f-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4000f-108">Property</span></span>       | <span data-ttu-id="4000f-109">Typ</span><span class="sxs-lookup"><span data-stu-id="4000f-109">Type</span></span>                          | <span data-ttu-id="4000f-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4000f-110">Description</span></span>                              |
|:---------------|:------------------------------|:-----------------------------------------|
| <span data-ttu-id="4000f-111">Identität</span><span class="sxs-lookup"><span data-stu-id="4000f-111">identity</span></span>       | [<span data-ttu-id="4000f-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="4000f-112">identitySet</span></span>](identityset.md) | <span data-ttu-id="4000f-113">Identitätsinformationen des Teilnehmers.</span><span class="sxs-lookup"><span data-stu-id="4000f-113">Identity information of the participant.</span></span> |
| <span data-ttu-id="4000f-114">UPN</span><span class="sxs-lookup"><span data-stu-id="4000f-114">upn</span></span>            | <span data-ttu-id="4000f-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4000f-115">String</span></span>                        | <span data-ttu-id="4000f-116">Benutzerprinzipalname des Teilnehmers.</span><span class="sxs-lookup"><span data-stu-id="4000f-116">User principal name of the participant.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="4000f-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4000f-117">JSON representation</span></span>

<span data-ttu-id="4000f-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4000f-118">The following is a JSON representation of the resource.</span></span>

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
