---
title: recipient-Ressourcentyp
description: 'Stellt Informationen zu einem Benutzer am sendenden oder empfangenden Ende eines Ereignisses, einer Nachricht oder einer Gruppenveröffentlichung dar. '
ms.openlocfilehash: 7ae272d239f44c3d2f709a03438facb2f0247e49
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016583"
---
# <a name="recipient-resource-type"></a><span data-ttu-id="ecacf-103">recipient-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ecacf-103">recipient resource type</span></span>

<span data-ttu-id="ecacf-104">Stellt Informationen zu einem Benutzer am sendenden oder empfangenden Ende eines Ereignisses, einer Nachricht oder einer Gruppenveröffentlichung dar.</span><span class="sxs-lookup"><span data-stu-id="ecacf-104">Represents information about a user in the sending or receiving end of an event, message or group post.</span></span> 

## <a name="properties"></a><span data-ttu-id="ecacf-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ecacf-105">Properties</span></span>
| <span data-ttu-id="ecacf-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ecacf-106">Property</span></span>     | <span data-ttu-id="ecacf-107">Typ</span><span class="sxs-lookup"><span data-stu-id="ecacf-107">Type</span></span>   |<span data-ttu-id="ecacf-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ecacf-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ecacf-109">emailAddress</span><span class="sxs-lookup"><span data-stu-id="ecacf-109">emailAddress</span></span>|[<span data-ttu-id="ecacf-110">EmailAddress</span><span class="sxs-lookup"><span data-stu-id="ecacf-110">EmailAddress</span></span>](emailaddress.md)|<span data-ttu-id="ecacf-111">Die E-Mail-Adresse des Empfängers.</span><span class="sxs-lookup"><span data-stu-id="ecacf-111">The recipient's email address.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ecacf-112">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ecacf-112">JSON representation</span></span>

<span data-ttu-id="ecacf-113">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ecacf-113">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recipient"
}-->

```json
{
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recipient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->