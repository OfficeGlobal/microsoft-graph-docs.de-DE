---
title: Ressourcentyp „locationConstraint“
description: Die vom Client definierten Bedingungen für den Ort einer Besprechung
localization_priority: Normal
ms.openlocfilehash: b1ff078efd5608fa388587003cf904c2b995f12e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851527"
---
# <a name="locationconstraint-resource-type"></a><span data-ttu-id="4cd15-103">Ressourcentyp „locationConstraint“</span><span class="sxs-lookup"><span data-stu-id="4cd15-103">locationConstraint resource type</span></span>

> <span data-ttu-id="4cd15-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4cd15-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4cd15-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4cd15-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4cd15-106">Die vom Client definierten Bedingungen für den Ort einer Besprechung</span><span class="sxs-lookup"><span data-stu-id="4cd15-106">The conditions stated by a client for the location of a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4cd15-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4cd15-107">JSON representation</span></span>

<span data-ttu-id="4cd15-108">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4cd15-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="4cd15-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4cd15-109">Properties</span></span>
| <span data-ttu-id="4cd15-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4cd15-110">Property</span></span>     | <span data-ttu-id="4cd15-111">Typ</span><span class="sxs-lookup"><span data-stu-id="4cd15-111">Type</span></span>   |<span data-ttu-id="4cd15-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4cd15-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4cd15-113">isRequired</span><span class="sxs-lookup"><span data-stu-id="4cd15-113">isRequired</span></span>|<span data-ttu-id="4cd15-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="4cd15-114">Boolean</span></span>|<span data-ttu-id="4cd15-p102">Der Client fordert den Dienst auf, in der Antwort einen Besprechungsort für die Besprechung anzugeben. Ist diese Eigenschaft auf „true“ gesetzt und alle Ressourcen sind gebucht, gibt [findMeetingTimes](../api/user-findmeetingtimes.md) keine Besprechungsterminvorschläge zurück. Ist diese Eigenschaft auf „false“ gesetzt und alle Ressourcen sind gebucht, sucht **findMeetingTimes** trotzdem nach Besprechungsterminen, jedoch nicht nach Orten.</span><span class="sxs-lookup"><span data-stu-id="4cd15-p102">The client requests the service to include in the response a meeting location for the meeting. If this is true and all the resources are busy, [findMeetingTimes](../api/user-findmeetingtimes.md) will not return any meeting time suggestions. If this is false and all the resources are busy, **findMeetingTimes** would still look for meeting times without locations.</span></span> |
|<span data-ttu-id="4cd15-118">locations</span><span class="sxs-lookup"><span data-stu-id="4cd15-118">locations</span></span>|<span data-ttu-id="4cd15-119">[locationConstraintItem](locationconstraintitem.md) collection</span><span class="sxs-lookup"><span data-stu-id="4cd15-119">[locationConstraintItem](locationconstraintitem.md) collection</span></span>|<span data-ttu-id="4cd15-120">Einschränkungsinformationen für einen oder mehrere Orte, die der Kunde für die Besprechung anfordert</span><span class="sxs-lookup"><span data-stu-id="4cd15-120">Constraint information for one or more locations that the client requests for the meeting.</span></span>|
|<span data-ttu-id="4cd15-121">suggestLocation</span><span class="sxs-lookup"><span data-stu-id="4cd15-121">suggestLocation</span></span>|<span data-ttu-id="4cd15-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="4cd15-122">Boolean</span></span>|<span data-ttu-id="4cd15-123">Der Client fordert den Dienst auf, einen oder mehrere Besprechungsorte vorzuschlagen.</span><span class="sxs-lookup"><span data-stu-id="4cd15-123">The client requests the service to suggest one or more meeting locations.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "locationConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
