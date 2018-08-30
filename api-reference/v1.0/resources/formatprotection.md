# <a name="formatprotection-resource-type"></a><span data-ttu-id="0cd9c-101">FormatProtection-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0cd9c-101">FormatProtection resource type</span></span>

<span data-ttu-id="0cd9c-102">Stellt den Formatschutz eines Bereichsobjekts dar.</span><span class="sxs-lookup"><span data-stu-id="0cd9c-102">Represents the format protection of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="0cd9c-103">Methoden</span><span class="sxs-lookup"><span data-stu-id="0cd9c-103">Methods</span></span>

| <span data-ttu-id="0cd9c-104">Methode</span><span class="sxs-lookup"><span data-stu-id="0cd9c-104">Method</span></span>           | <span data-ttu-id="0cd9c-105">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="0cd9c-105">Return Type</span></span>    |<span data-ttu-id="0cd9c-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0cd9c-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0cd9c-107">FormatProtection abrufen</span><span class="sxs-lookup"><span data-stu-id="0cd9c-107">Get FormatProtection</span></span>](../api/formatprotection_get.md) | [<span data-ttu-id="0cd9c-108">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="0cd9c-108">FormatProtection</span></span>](formatprotection.md) |<span data-ttu-id="0cd9c-109">Dient zum Lesen der Eigenschaften und der Beziehungen des formatProtection-Objekts.</span><span class="sxs-lookup"><span data-stu-id="0cd9c-109">Read properties and relationships of formatProtection object.</span></span>|
|[<span data-ttu-id="0cd9c-110">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="0cd9c-110">Update</span></span>](../api/formatprotection_update.md) | [<span data-ttu-id="0cd9c-111">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="0cd9c-111">FormatProtection</span></span>](formatprotection.md)  |<span data-ttu-id="0cd9c-112">Dient zum Aktualisieren des FormatProtection-Objekts.</span><span class="sxs-lookup"><span data-stu-id="0cd9c-112">Update FormatProtection object.</span></span> |

## <a name="properties"></a><span data-ttu-id="0cd9c-113">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0cd9c-113">Properties</span></span>
| <span data-ttu-id="0cd9c-114">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0cd9c-114">Property</span></span>     | <span data-ttu-id="0cd9c-115">Typ</span><span class="sxs-lookup"><span data-stu-id="0cd9c-115">Type</span></span>   |<span data-ttu-id="0cd9c-116">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0cd9c-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0cd9c-117">formulaHidden</span><span class="sxs-lookup"><span data-stu-id="0cd9c-117">formulaHidden</span></span>|<span data-ttu-id="0cd9c-118">boolesch</span><span class="sxs-lookup"><span data-stu-id="0cd9c-118">boolean</span></span>|<span data-ttu-id="0cd9c-p101">Zeigt an, ob Excel die Formel für die Zellen im Bereich ausblendet. Ein Nullwert gibt an, dass der gesamte Bereich keine einheitliche Einstellung zur Formelausblendung hat.</span><span class="sxs-lookup"><span data-stu-id="0cd9c-p101">Indicates if Excel hides the formula for the cells in the range. A null value indicates that the entire range doesn't have uniform formula hidden setting.</span></span>|
|<span data-ttu-id="0cd9c-121">locked</span><span class="sxs-lookup"><span data-stu-id="0cd9c-121">locked</span></span>|<span data-ttu-id="0cd9c-122">boolesch</span><span class="sxs-lookup"><span data-stu-id="0cd9c-122">boolean</span></span>|<span data-ttu-id="0cd9c-p102">Gibt an, ob Excel die Zellen im Objekt sperrt. Ein Nullwert gibt an, dass der gesamte Bereich keine einheitliche Einstellung zum Sperren hat.</span><span class="sxs-lookup"><span data-stu-id="0cd9c-p102">Indicates if Excel locks the cells in the object. A null value indicates that the entire range doesn't have uniform lock setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0cd9c-125">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0cd9c-125">Relationships</span></span>
<span data-ttu-id="0cd9c-126">Keine</span><span class="sxs-lookup"><span data-stu-id="0cd9c-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="0cd9c-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0cd9c-127">JSON representation</span></span>

<span data-ttu-id="0cd9c-128">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0cd9c-128">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookFormatProtection"
}-->

```json
{
  "formulaHidden": true,
  "locked": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "FormatProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->