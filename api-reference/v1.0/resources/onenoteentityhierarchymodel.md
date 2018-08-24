# <a name="onenoteentityhierarchymodel-resource"></a><span data-ttu-id="06337-101">Ressource onenoteEntityHierarchyModel</span><span class="sxs-lookup"><span data-stu-id="06337-101">onenoteEntityHierarchyModel resource</span></span>

<span data-ttu-id="06337-102">Dies ist ein Basistyp für OneNote-Entitäten.</span><span class="sxs-lookup"><span data-stu-id="06337-102">This is a base type for OneNote entities.</span></span>

## <a name="json-representation"></a><span data-ttu-id="06337-103">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="06337-103">JSON representation</span></span>

<span data-ttu-id="06337-104">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="06337-104">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.onenoteEntitySchemaObjectModel",
  "optionalProperties": [
    "self"
  ],
  "@odata.type": "microsoft.graph.onenoteEntityHierarchyModel"
}-->

```json
{
  "displayName": "string",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)"
}

```
## <a name="properties"></a><span data-ttu-id="06337-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="06337-105">Properties</span></span>
## <a name="properties"></a><span data-ttu-id="06337-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="06337-106">Properties</span></span>
| <span data-ttu-id="06337-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="06337-107">Property</span></span>     | <span data-ttu-id="06337-108">Typ</span><span class="sxs-lookup"><span data-stu-id="06337-108">Type</span></span>   |<span data-ttu-id="06337-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="06337-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="06337-110">displayName</span><span class="sxs-lookup"><span data-stu-id="06337-110">displayName</span></span>|<span data-ttu-id="06337-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="06337-111">String</span></span>|<span data-ttu-id="06337-112">Der Name des Notizbuchs.</span><span class="sxs-lookup"><span data-stu-id="06337-112">The name of the notebook.</span></span>|
|<span data-ttu-id="06337-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="06337-113">createdBy</span></span>|[<span data-ttu-id="06337-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="06337-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="06337-p101">Die Identität des Benutzers, des Geräts und der Anwendung, von der das Element erstellt wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="06337-p101">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="06337-117">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="06337-117">lastModifiedBy</span></span>|[<span data-ttu-id="06337-118">identitySet</span><span class="sxs-lookup"><span data-stu-id="06337-118">identitySet</span></span>](identityset.md)|<span data-ttu-id="06337-p102">Die Identität des Benutzers, des Geräts und der Anwendung, von der das Element erstellt wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="06337-p102">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="06337-121">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="06337-121">lastModifiedDateTime</span></span>|<span data-ttu-id="06337-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06337-122">DateTimeOffset</span></span>|<span data-ttu-id="06337-p103">Das Datum und die Uhrzeit der letzten Änderung des Notizbuchs. Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="06337-p103">The date and time when the notebook was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|

<!-- uuid: 8b1af557-1a7c-4432-86eb-94989c2d4b54
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->