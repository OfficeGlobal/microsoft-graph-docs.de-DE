---
title: Ressourcentyp „locationConstraint“
description: Die vom Client definierten Bedingungen für den Ort einer Besprechung
localization_priority: Normal
ms.openlocfilehash: f311ceae1718333ba6ffca55f046317d6da53705
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522742"
---
# <a name="locationconstraint-resource-type"></a><span data-ttu-id="c0e01-103">Ressourcentyp „locationConstraint“</span><span class="sxs-lookup"><span data-stu-id="c0e01-103">locationConstraint resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0e01-104">Die vom Client definierten Bedingungen für den Ort einer Besprechung</span><span class="sxs-lookup"><span data-stu-id="c0e01-104">The conditions stated by a client for the location of a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c0e01-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c0e01-105">JSON representation</span></span>

<span data-ttu-id="c0e01-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c0e01-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.locationconstraint"
}-->

```json
{
  "isRequired": true,
  "locations": [{"@odata.type": "microsoft.graph.locationConstraintItem"}],
  "suggestLocation": true
}

```
## <a name="properties"></a><span data-ttu-id="c0e01-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c0e01-107">Properties</span></span>
| <span data-ttu-id="c0e01-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c0e01-108">Property</span></span>     | <span data-ttu-id="c0e01-109">Typ</span><span class="sxs-lookup"><span data-stu-id="c0e01-109">Type</span></span>   |<span data-ttu-id="c0e01-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c0e01-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c0e01-111">isRequired</span><span class="sxs-lookup"><span data-stu-id="c0e01-111">isRequired</span></span>|<span data-ttu-id="c0e01-112">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c0e01-112">Boolean</span></span>|<span data-ttu-id="c0e01-p101">Der Client fordert den Dienst auf, in der Antwort einen Besprechungsort für die Besprechung anzugeben. Ist diese Eigenschaft auf „true“ gesetzt und alle Ressourcen sind gebucht, gibt [findMeetingTimes](../api/user-findmeetingtimes.md) keine Besprechungsterminvorschläge zurück. Ist diese Eigenschaft auf „false“ gesetzt und alle Ressourcen sind gebucht, sucht **findMeetingTimes** trotzdem nach Besprechungsterminen, jedoch nicht nach Orten.</span><span class="sxs-lookup"><span data-stu-id="c0e01-p101">The client requests the service to include in the response a meeting location for the meeting. If this is true and all the resources are busy, [findMeetingTimes](../api/user-findmeetingtimes.md) will not return any meeting time suggestions. If this is false and all the resources are busy, **findMeetingTimes** would still look for meeting times without locations.</span></span> |
|<span data-ttu-id="c0e01-116">locations</span><span class="sxs-lookup"><span data-stu-id="c0e01-116">locations</span></span>|<span data-ttu-id="c0e01-117">[locationConstraintItem](locationconstraintitem.md) collection</span><span class="sxs-lookup"><span data-stu-id="c0e01-117">[locationConstraintItem](locationconstraintitem.md) collection</span></span>|<span data-ttu-id="c0e01-118">Einschränkungsinformationen für einen oder mehrere Orte, die der Kunde für die Besprechung anfordert</span><span class="sxs-lookup"><span data-stu-id="c0e01-118">Constraint information for one or more locations that the client requests for the meeting.</span></span>|
|<span data-ttu-id="c0e01-119">suggestLocation</span><span class="sxs-lookup"><span data-stu-id="c0e01-119">suggestLocation</span></span>|<span data-ttu-id="c0e01-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0e01-120">Boolean</span></span>|<span data-ttu-id="c0e01-121">Der Client fordert den Dienst auf, einen oder mehrere Besprechungsorte vorzuschlagen.</span><span class="sxs-lookup"><span data-stu-id="c0e01-121">The client requests the service to suggest one or more meeting locations.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "locationConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/locationconstraint.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
