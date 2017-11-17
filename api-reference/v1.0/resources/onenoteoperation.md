# <a name="onenoteoperation-resource-type"></a><span data-ttu-id="d75b4-101">onenoteOperation-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d75b4-101">onenoteOperation resource type</span></span>

<span data-ttu-id="d75b4-102">Der Status bestimmter lange dauernder OneNote-Vorgänge.</span><span class="sxs-lookup"><span data-stu-id="d75b4-102">The status of certain long-running OneNote operations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d75b4-103">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d75b4-103">JSON representation</span></span>

<span data-ttu-id="d75b4-104">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d75b4-104">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteOperation"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "error": {"@odata.type": "microsoft.graph.onenoteOperationError"},
  "id": "string (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "resourceId": "string",
  "resourceLocation": "string",
  "status": "string",
  "percentComplete": "string"
}

```
## <a name="properties"></a><span data-ttu-id="d75b4-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d75b4-105">Properties</span></span>
| <span data-ttu-id="d75b4-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d75b4-106">Property</span></span>     | <span data-ttu-id="d75b4-107">Typ</span><span class="sxs-lookup"><span data-stu-id="d75b4-107">Type</span></span>   |<span data-ttu-id="d75b4-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d75b4-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d75b4-109">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d75b4-109">createdDateTime</span></span>| <span data-ttu-id="d75b4-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d75b4-110">DateTimeOffset</span></span> |<span data-ttu-id="d75b4-111">Die Startzeit des Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="d75b4-111">The start time of the operation.</span></span>|
|<span data-ttu-id="d75b4-112">error</span><span class="sxs-lookup"><span data-stu-id="d75b4-112">error</span></span>|[<span data-ttu-id="d75b4-113">onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="d75b4-113">onenoteOperationError</span></span>](onenoteoperationerror.md)|<span data-ttu-id="d75b4-114">Der Fehler, der vom Vorgang zurückgegeben wird.</span><span class="sxs-lookup"><span data-stu-id="d75b4-114">The error returned by the operation.</span></span>|
|<span data-ttu-id="d75b4-115">id</span><span class="sxs-lookup"><span data-stu-id="d75b4-115">id</span></span>|<span data-ttu-id="d75b4-116">string</span><span class="sxs-lookup"><span data-stu-id="d75b4-116">string</span></span>|<span data-ttu-id="d75b4-117">Die Vorgangs-ID. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d75b4-117">The operation id. Read-only.</span></span>|
|<span data-ttu-id="d75b4-118">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="d75b4-118">lastActionDateTime</span></span>| <span data-ttu-id="d75b4-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d75b4-119">DateTimeOffset</span></span> |<span data-ttu-id="d75b4-120">Der Zeitpunkt der letzten Aktion des Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="d75b4-120">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="d75b4-121">resourceId</span><span class="sxs-lookup"><span data-stu-id="d75b4-121">resourceId</span></span>|<span data-ttu-id="d75b4-122">string</span><span class="sxs-lookup"><span data-stu-id="d75b4-122">string</span></span>|<span data-ttu-id="d75b4-123">Die Ressourcen-ID.</span><span class="sxs-lookup"><span data-stu-id="d75b4-123">The resource id.</span></span>|
|<span data-ttu-id="d75b4-124">resourceLocation</span><span class="sxs-lookup"><span data-stu-id="d75b4-124">resourceLocation</span></span>|<span data-ttu-id="d75b4-125">string</span><span class="sxs-lookup"><span data-stu-id="d75b4-125">string</span></span>|<span data-ttu-id="d75b4-p101">Der Ressourcen-URI für das Objekt. Beispielsweise der Ressource-URI für eine kopierte Seite oder einen kopierten Abschnitt.</span><span class="sxs-lookup"><span data-stu-id="d75b4-p101">The resource URI for the object. For example, the resource URI for a copied page or section.</span></span> |
|<span data-ttu-id="d75b4-128">status</span><span class="sxs-lookup"><span data-stu-id="d75b4-128">status</span></span>|<span data-ttu-id="d75b4-129">string</span><span class="sxs-lookup"><span data-stu-id="d75b4-129">string</span></span>|<span data-ttu-id="d75b4-130">Der aktuellen Status des Vorgangs: `notstarted`, `running`, `completed`, `failed`</span><span class="sxs-lookup"><span data-stu-id="d75b4-130">The current status of the operation: `notstarted`, `running`, `completed`, `failed`</span></span> |
|<span data-ttu-id="d75b4-131">percentComplete</span><span class="sxs-lookup"><span data-stu-id="d75b4-131">percentComplete</span></span>|<span data-ttu-id="d75b4-132">string</span><span class="sxs-lookup"><span data-stu-id="d75b4-132">string</span></span>|<span data-ttu-id="d75b4-133">Der abgeschlossene Prozentsatz des Vorgangs, sofern der Vorgang noch den Status `running` hat.</span><span class="sxs-lookup"><span data-stu-id="d75b4-133">The operation percent complete if the operation is still in `running` status</span></span>

## <a name="relationships"></a><span data-ttu-id="d75b4-134">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d75b4-134">Relationships</span></span>
<span data-ttu-id="d75b4-135">Keine</span><span class="sxs-lookup"><span data-stu-id="d75b4-135">None</span></span>


## <a name="methods"></a><span data-ttu-id="d75b4-136">Methoden</span><span class="sxs-lookup"><span data-stu-id="d75b4-136">Methods</span></span>

| <span data-ttu-id="d75b4-137">Methode</span><span class="sxs-lookup"><span data-stu-id="d75b4-137">Method</span></span>           | <span data-ttu-id="d75b4-138">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="d75b4-138">Return Type</span></span>    |<span data-ttu-id="d75b4-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d75b4-139">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d75b4-140">Vorgang abrufen</span><span class="sxs-lookup"><span data-stu-id="d75b4-140">Get operation</span></span>](../api/onenoteoperation_get.md) | [<span data-ttu-id="d75b4-141">onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="d75b4-141">onenoteOperation</span></span>](onenoteoperation.md) |<span data-ttu-id="d75b4-142">Dient zum Abrufen des Status des Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="d75b4-142">Get the status of the operation.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
