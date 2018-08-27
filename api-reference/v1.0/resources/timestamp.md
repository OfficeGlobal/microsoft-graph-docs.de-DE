# <a name="timestamp-resource-type"></a><span data-ttu-id="31995-101">Zeitstempel Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="31995-101">timeStamp resource type</span></span>

<span data-ttu-id="31995-102">Datums- und Zeitangaben für einen bestimmten Zeitpunkt</span><span class="sxs-lookup"><span data-stu-id="31995-102">Date and time information for a point in time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="31995-103">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="31995-103">JSON representation</span></span>

<span data-ttu-id="31995-104">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="31995-104">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeStamp"
}-->

```json
{
  "date": "String (timestamp)",
  "time": "String (timestamp)",
  "timeZone": "string"
}

```
## <a name="properties"></a><span data-ttu-id="31995-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="31995-105">Properties</span></span>
| <span data-ttu-id="31995-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="31995-106">Property</span></span>       | <span data-ttu-id="31995-107">Typ</span><span class="sxs-lookup"><span data-stu-id="31995-107">Type</span></span>    |<span data-ttu-id="31995-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="31995-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="31995-109">date</span><span class="sxs-lookup"><span data-stu-id="31995-109">date</span></span>|<span data-ttu-id="31995-110">Datum</span><span class="sxs-lookup"><span data-stu-id="31995-110">Date</span></span>|<span data-ttu-id="31995-111">Der Datumsteil des Zeitstempels.</span><span class="sxs-lookup"><span data-stu-id="31995-111">The date portion of the timestamp.</span></span>|
|<span data-ttu-id="31995-112">time</span><span class="sxs-lookup"><span data-stu-id="31995-112">time</span></span>|<span data-ttu-id="31995-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="31995-113">TimeOfDay</span></span>|<span data-ttu-id="31995-114">Der Uhrzeitteil des Zeitstempels.</span><span class="sxs-lookup"><span data-stu-id="31995-114">The time portion of the timestamp.</span></span>|
|<span data-ttu-id="31995-115">timeZone</span><span class="sxs-lookup"><span data-stu-id="31995-115">timeZone</span></span>|<span data-ttu-id="31995-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="31995-116">String</span></span>|<span data-ttu-id="31995-117">Der Zeitzonenteil des Zeitstempels, der eine der 24 Zeitzonen der Welt bezeichnet.</span><span class="sxs-lookup"><span data-stu-id="31995-117">The timezone portion of the timestamp, which is one of the 24 longitudinal areas in the world.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeStamp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->