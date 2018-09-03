# <a name="outlookitem-resource-type"></a><span data-ttu-id="a2f56-101">outlookItem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a2f56-101">outlookItem resource type</span></span>



## <a name="json-representation"></a><span data-ttu-id="a2f56-102">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a2f56-102">JSON representation</span></span>

<span data-ttu-id="a2f56-103">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a2f56-103">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "abstract": true,
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.outlookItem"
}-->

```json
{
  "categories": ["string"],
  "changeKey": "string",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}

```
## <a name="properties"></a><span data-ttu-id="a2f56-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a2f56-104">Properties</span></span>
| <span data-ttu-id="a2f56-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a2f56-105">Property</span></span>     | <span data-ttu-id="a2f56-106">Typ</span><span class="sxs-lookup"><span data-stu-id="a2f56-106">Type</span></span>   |<span data-ttu-id="a2f56-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a2f56-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a2f56-108">Kategorien</span><span class="sxs-lookup"><span data-stu-id="a2f56-108">categories</span></span>|<span data-ttu-id="a2f56-109">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="a2f56-109">String collection</span></span>|<span data-ttu-id="a2f56-110">Die Kategorien, die mit dem Element verknüpft sind</span><span class="sxs-lookup"><span data-stu-id="a2f56-110">The categories associated with the message.</span></span>|
|<span data-ttu-id="a2f56-111">changeKey</span><span class="sxs-lookup"><span data-stu-id="a2f56-111">changeKey</span></span>|<span data-ttu-id="a2f56-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a2f56-112">String</span></span>|<span data-ttu-id="a2f56-113">Identifiziert die Version des Elements.</span><span class="sxs-lookup"><span data-stu-id="a2f56-113">Identifies the version of the contact.</span></span> <span data-ttu-id="a2f56-114">Jedes Mal, wenn das Element geändert wird, ändert sich auch ChangeKey.</span><span class="sxs-lookup"><span data-stu-id="a2f56-114">Every time the contact is changed, ChangeKey  changes as well.</span></span> <span data-ttu-id="a2f56-115">Dies ermöglicht es Exchange, die Änderungen an der richtigen Version des Objekts vorzunehmen.</span><span class="sxs-lookup"><span data-stu-id="a2f56-115">Identifies the version of the reminder. Every time the reminder is changed, changeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span> <span data-ttu-id="a2f56-116">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a2f56-116">Read-only.</span></span>|
|<span data-ttu-id="a2f56-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a2f56-117">createdDateTime</span></span>|<span data-ttu-id="a2f56-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2f56-118">DateTimeOffset</span></span>|<span data-ttu-id="a2f56-p102">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="a2f56-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="a2f56-121">id</span><span class="sxs-lookup"><span data-stu-id="a2f56-121">id</span></span>|<span data-ttu-id="a2f56-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a2f56-122">String</span></span>| <span data-ttu-id="a2f56-123">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a2f56-123">Read-only.</span></span>|
|<span data-ttu-id="a2f56-124">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a2f56-124">lastModifiedDateTime</span></span>|<span data-ttu-id="a2f56-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2f56-125">DateTimeOffset</span></span>|<span data-ttu-id="a2f56-p103">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="a2f56-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="a2f56-128">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a2f56-128">Relationships</span></span>
<span data-ttu-id="a2f56-129">Keine</span><span class="sxs-lookup"><span data-stu-id="a2f56-129">None</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
