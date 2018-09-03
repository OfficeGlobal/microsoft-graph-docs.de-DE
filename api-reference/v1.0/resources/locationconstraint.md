# <a name="locationconstraint-resource-type"></a><span data-ttu-id="adeab-101">Ressourcentyp „locationConstraint“</span><span class="sxs-lookup"><span data-stu-id="adeab-101">locationConstraint resource type</span></span>

<span data-ttu-id="adeab-102">Die vom Client definierten Bedingungen für den Ort einer Besprechung</span><span class="sxs-lookup"><span data-stu-id="adeab-102">The conditions stated by a client for the location of a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="adeab-103">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="adeab-103">JSON representation</span></span>

<span data-ttu-id="adeab-104">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="adeab-104">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.locationConstraint"
}-->

```json
{
  "isRequired": true,
  "locations": [{"@odata.type": "microsoft.graph.locationConstraintItem"}],
  "suggestLocation": true
}

```
## <a name="properties"></a><span data-ttu-id="adeab-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="adeab-105">Properties</span></span>
| <span data-ttu-id="adeab-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="adeab-106">Property</span></span>     | <span data-ttu-id="adeab-107">Typ</span><span class="sxs-lookup"><span data-stu-id="adeab-107">Type</span></span>   |<span data-ttu-id="adeab-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="adeab-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="adeab-109">isRequired</span><span class="sxs-lookup"><span data-stu-id="adeab-109">isRequired</span></span>|<span data-ttu-id="adeab-110">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="adeab-110">Boolean</span></span>|<span data-ttu-id="adeab-p101">Der Client fordert den Dienst auf, in der Antwort einen Besprechungsort für die Besprechung anzugeben. Ist diese Eigenschaft auf „true“ gesetzt und alle Ressourcen sind gebucht, gibt [findMeetingTimes](../api/user_findmeetingtimes.md) keine Besprechungsterminvorschläge zurück. Ist diese Eigenschaft auf „false“ gesetzt und alle Ressourcen sind gebucht, sucht **findMeetingTimes** trotzdem nach Besprechungsterminen, jedoch nicht nach Orten.</span><span class="sxs-lookup"><span data-stu-id="adeab-p101">The client requests the service to include in the response a meeting location for the meeting. If this is true and all the resources are busy, [findMeetingTimes](../api/user_findmeetingtimes.md) will not return any meeting time suggestions. If this is false and all the resources are busy, **findMeetingTimes** would still look for meeting times without locations.</span></span> |
|<span data-ttu-id="adeab-114">locations</span><span class="sxs-lookup"><span data-stu-id="adeab-114">locations</span></span>|<span data-ttu-id="adeab-115">[locationConstraintItem](locationconstraintitem.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="adeab-115">[locationConstraintItem](locationconstraintitem.md) collection</span></span>|<span data-ttu-id="adeab-116">Einschränkungsinformationen für einen oder mehrere Orte, die der Kunde für die Besprechung anfordert</span><span class="sxs-lookup"><span data-stu-id="adeab-116">Constraint information for one or more locations that the client requests for the meeting.</span></span>|
|<span data-ttu-id="adeab-117">suggestLocation</span><span class="sxs-lookup"><span data-stu-id="adeab-117">suggestLocation</span></span>|<span data-ttu-id="adeab-118">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="adeab-118">Boolean</span></span>|<span data-ttu-id="adeab-119">Der Client fordert den Dienst auf, einen oder mehrere Besprechungsorte vorzuschlagen.</span><span class="sxs-lookup"><span data-stu-id="adeab-119">The client requests the service to suggest one or more meeting locations.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "locationConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->