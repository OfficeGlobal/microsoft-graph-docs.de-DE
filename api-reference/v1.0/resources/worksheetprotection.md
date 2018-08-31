# <a name="worksheetprotection-resource-type"></a><span data-ttu-id="15c16-101">WorksheetProtection-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="15c16-101">WorksheetProtection resource type</span></span>

<span data-ttu-id="15c16-102">Stellt den Schutz eines Arbeitsblattobjekts dar.</span><span class="sxs-lookup"><span data-stu-id="15c16-102">Represents the protection of a sheet object.</span></span>


## <a name="methods"></a><span data-ttu-id="15c16-103">Methoden</span><span class="sxs-lookup"><span data-stu-id="15c16-103">Methods</span></span>

| <span data-ttu-id="15c16-104">Methode</span><span class="sxs-lookup"><span data-stu-id="15c16-104">Method</span></span>           | <span data-ttu-id="15c16-105">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="15c16-105">Return Type</span></span>    |<span data-ttu-id="15c16-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="15c16-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="15c16-107">Get WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="15c16-107">Get WorksheetProtection</span></span>](../api/worksheetprotection_get.md) | [<span data-ttu-id="15c16-108">WorkbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="15c16-108">WorkbookWorksheetProtection</span></span>](worksheetprotection.md) |<span data-ttu-id="15c16-109">Dient zum Lesen der Eigenschaften und der Beziehungen des worksheetProtection-Objekts.</span><span class="sxs-lookup"><span data-stu-id="15c16-109">Read properties and relationships of worksheetProtection object.</span></span>|
|[<span data-ttu-id="15c16-110">Protect</span><span class="sxs-lookup"><span data-stu-id="15c16-110">Protect</span></span>](../api/worksheetprotection_protect.md)|<span data-ttu-id="15c16-111">Keine</span><span class="sxs-lookup"><span data-stu-id="15c16-111">None</span></span>|<span data-ttu-id="15c16-p101">Ein Arbeitsblatt schützen. Es wird ausgelöst, wenn das Arbeitsblatt geschützt ist.</span><span class="sxs-lookup"><span data-stu-id="15c16-p101">Protect a worksheet. It throws if the worksheet has been protected.</span></span>|
|[<span data-ttu-id="15c16-114">Schutz aufheben</span><span class="sxs-lookup"><span data-stu-id="15c16-114">Unprotect</span></span>](../api/worksheetprotection_unprotect.md)|<span data-ttu-id="15c16-115">Keine</span><span class="sxs-lookup"><span data-stu-id="15c16-115">None</span></span>|<span data-ttu-id="15c16-116">Schutz eines Arbeitsblatts aufheben.</span><span class="sxs-lookup"><span data-stu-id="15c16-116">Unprotect a worksheet</span></span>|

## <a name="properties"></a><span data-ttu-id="15c16-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="15c16-117">Properties</span></span>
| <span data-ttu-id="15c16-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="15c16-118">Property</span></span>     | <span data-ttu-id="15c16-119">Typ</span><span class="sxs-lookup"><span data-stu-id="15c16-119">Type</span></span>   |<span data-ttu-id="15c16-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="15c16-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="15c16-121">Optionen</span><span class="sxs-lookup"><span data-stu-id="15c16-121">options</span></span>|[<span data-ttu-id="15c16-122">WorkbookWorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="15c16-122">WorkbookWorksheetProtectionOptions</span></span>](worksheetprotectionoptions.md)|<span data-ttu-id="15c16-p102">Optionen für den Arbeitsblattschutz. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="15c16-p102">Sheet protection options. Read-only.</span></span>|
|<span data-ttu-id="15c16-125">geschützt</span><span class="sxs-lookup"><span data-stu-id="15c16-125">protected</span></span>|<span data-ttu-id="15c16-126">boolesch</span><span class="sxs-lookup"><span data-stu-id="15c16-126">boolean</span></span>|<span data-ttu-id="15c16-p103">Zeigt an, ob das Arbeitsblatt geschützt ist.  Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="15c16-p103">Indicates if the worksheet is protected.  Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="15c16-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="15c16-129">JSON representation</span></span>

<span data-ttu-id="15c16-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="15c16-130">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookWorksheetProtection"
}-->

```json
{
  "protected": true,
  "options": { "@odata.type": "microsoft.graph.workbookWorksheetProtectionOptions" }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->