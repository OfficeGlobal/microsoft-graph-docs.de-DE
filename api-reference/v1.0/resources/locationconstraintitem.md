# <a name="locationconstraintitem-resource-type"></a><span data-ttu-id="890de-101">Ressourcentyp „locationConstraintItem“</span><span class="sxs-lookup"><span data-stu-id="890de-101">locationConstraintItem resource type</span></span>

<span data-ttu-id="890de-102">Die vom Client definierten Bedingungen für den Ort einer Besprechung.</span><span class="sxs-lookup"><span data-stu-id="890de-102">The conditions stated by a client for the location of a meeting.</span></span>

<span data-ttu-id="890de-103">Abgeleitet von [location](location.md).</span><span class="sxs-lookup"><span data-stu-id="890de-103">Derived from [location](location.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="890de-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="890de-104">JSON representation</span></span>

<span data-ttu-id="890de-105">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="890de-105">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.location",
  "@odata.type": "microsoft.graph.locationConstraintItem"
}-->

```json
{
  "resolveAvailability": true,
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "displayName": "string",
  "locationEmailAddress": "string"
}

```
## <a name="properties"></a><span data-ttu-id="890de-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="890de-106">Properties</span></span>
| <span data-ttu-id="890de-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="890de-107">Property</span></span>     | <span data-ttu-id="890de-108">Typ</span><span class="sxs-lookup"><span data-stu-id="890de-108">Type</span></span>   |<span data-ttu-id="890de-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="890de-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="890de-110">address</span><span class="sxs-lookup"><span data-stu-id="890de-110">address</span></span> | [<span data-ttu-id="890de-111">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="890de-111">physicalAddress</span></span>](physicalAddress.md) |<span data-ttu-id="890de-112">Die Adresse des Orts.</span><span class="sxs-lookup"><span data-stu-id="890de-112">The street address of the location.</span></span> |
| <span data-ttu-id="890de-113">displayName</span><span class="sxs-lookup"><span data-stu-id="890de-113">displayName</span></span>  | <span data-ttu-id="890de-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="890de-114">String</span></span> | <span data-ttu-id="890de-115">Der Name, der mit dem Ort verknüpft ist</span><span class="sxs-lookup"><span data-stu-id="890de-115">The name associated with the location.</span></span>                       |
| <span data-ttu-id="890de-116">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="890de-116">locationEmailAddress</span></span> | <span data-ttu-id="890de-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="890de-117">String</span></span> | <span data-ttu-id="890de-118">Optionale E-Mail-Adresse des Orts</span><span class="sxs-lookup"><span data-stu-id="890de-118">Optional email address of the location.</span></span> |
| <span data-ttu-id="890de-119">resolveAvailability</span><span class="sxs-lookup"><span data-stu-id="890de-119">resolveAvailability</span></span> | <span data-ttu-id="890de-120">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="890de-120">Boolean</span></span> | <span data-ttu-id="890de-p101">Wenn „true“ gesetzt ist und die angegebene Ressource gebucht ist, sucht [findMeetingTimes](../api/user_findmeetingtimes.md) nach einer anderen, freien Ressource. Wenn „false“ gesetzt ist und die angegebene Ressource gebucht ist, gibt **findMeetingTimes** die Ressource mit dem höchsten Wert aus dem Cache des Benutzers zurück, ohne zu prüfen, ob diese Ressource frei ist. Der Standardwert ist „true“.</span><span class="sxs-lookup"><span data-stu-id="890de-p101">If set to true and the specified resource is busy, [findMeetingTimes](../api/user_findmeetingtimes.md) looks for another resource that is free. If set to false and the specified resource is busy, **findMeetingTimes** returns the resource best ranked in the user's cache without checking if it's free. Default is true.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "locationConstraintItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->