# <a name="subscribedsku-resource-type"></a><span data-ttu-id="50510-101">subscribedSku-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="50510-101">subscribedSku resource type</span></span>

<span data-ttu-id="50510-102">Enthält Informationen zu einer Dienst-SKU, die ein Unternehmen abonniert hat.</span><span class="sxs-lookup"><span data-stu-id="50510-102">Contains information about a service SKU that a company is subscribed to.</span></span>

<span data-ttu-id="50510-p101">Für abonnierte SKUs wird nur der Lesevorgang unterstützt. Erstellen, Aktualisieren und Löschen werden nicht unterstützt. Abfragefilterausdrücke werden nicht unterstützt. Erbt von [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="50510-p101">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported. Query filter expressions are not supported. Inherits from [directoryObject](directoryobject.md).</span></span>

## <a name="methods"></a><span data-ttu-id="50510-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="50510-106">Methods</span></span>
| <span data-ttu-id="50510-107">Methode</span><span class="sxs-lookup"><span data-stu-id="50510-107">Method</span></span>           | <span data-ttu-id="50510-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="50510-108">Return Type</span></span>    |<span data-ttu-id="50510-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="50510-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="50510-110">subscribedSku abrufen</span><span class="sxs-lookup"><span data-stu-id="50510-110">Get subscribedSku</span></span>](../api/subscribedsku_get.md) | [<span data-ttu-id="50510-111">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="50510-111">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="50510-112">Dient zum Lesen der Eigenschaften und Beziehungen des subscribedSku-Objekts.</span><span class="sxs-lookup"><span data-stu-id="50510-112">Read properties and relationships of subscribedSku object.</span></span>|
|[<span data-ttu-id="50510-113">subscribedSku auflisten</span><span class="sxs-lookup"><span data-stu-id="50510-113">List subscribedSku</span></span>](../api/subscribedsku_list.md) | <span data-ttu-id="50510-114">|||UNTRANSLATED_CONTENT_START|||[subscribedSku](subscribedsku.md) collection|||UNTRANSLATED_CONTENT_END|||</span><span class="sxs-lookup"><span data-stu-id="50510-114">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="50510-115">Dienst zum Abrufen der Liste aller kommerziellen Abonnements, die eine Organisation erworben hat.</span><span class="sxs-lookup"><span data-stu-id="50510-115">Retrieve the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="50510-116">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="50510-116">Properties</span></span>
| <span data-ttu-id="50510-117">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="50510-117">Property</span></span>     | <span data-ttu-id="50510-118">Typ</span><span class="sxs-lookup"><span data-stu-id="50510-118">Type</span></span>   |<span data-ttu-id="50510-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="50510-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="50510-120">appliesTo</span><span class="sxs-lookup"><span data-stu-id="50510-120">appliesTo</span></span>|<span data-ttu-id="50510-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="50510-121">String</span></span>| <span data-ttu-id="50510-122">Beispiel: „Benutzer“ oder „Community“.</span><span class="sxs-lookup"><span data-stu-id="50510-122">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="50510-123">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="50510-123">capabilityStatus</span></span>|<span data-ttu-id="50510-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="50510-124">String</span></span>| <span data-ttu-id="50510-125">Beispiel: „Aktiviert“.</span><span class="sxs-lookup"><span data-stu-id="50510-125">For example, "Enabled".</span></span> |
|<span data-ttu-id="50510-126">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="50510-126">consumedUnits</span></span>|<span data-ttu-id="50510-127">Int32</span><span class="sxs-lookup"><span data-stu-id="50510-127">Int32</span></span>| <span data-ttu-id="50510-128">Die Anzahl der Lizenzen, die zugewiesen wurden.</span><span class="sxs-lookup"><span data-stu-id="50510-128">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="50510-129">ID</span><span class="sxs-lookup"><span data-stu-id="50510-129">id</span></span>|<span data-ttu-id="50510-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="50510-130">String</span></span>| <span data-ttu-id="50510-p102">Der eindeutige Bezeichner für das subscribedSku-Objekt. Schlüssel, lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="50510-p102">The unique identifier for the subscribed sku object. Key, not nullable.</span></span> |
|<span data-ttu-id="50510-133">prepaidUnits</span><span class="sxs-lookup"><span data-stu-id="50510-133">prepaidUnits</span></span>|[<span data-ttu-id="50510-134">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="50510-134">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="50510-135">Informationen über die Anzahl und den Status der Prepaidlizenzen.</span><span class="sxs-lookup"><span data-stu-id="50510-135">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="50510-136">servicePlans</span><span class="sxs-lookup"><span data-stu-id="50510-136">servicePlans</span></span>|<span data-ttu-id="50510-137">[servicePlanInfo](serviceplaninfo.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="50510-137">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="50510-p103">Informationen über die Servicepläne, die mit der SKU verfügbar sind. Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="50510-p103">Information about the service plans that are available with the SKU. Not nullable</span></span> |
|<span data-ttu-id="50510-140">skuId</span><span class="sxs-lookup"><span data-stu-id="50510-140">skuId</span></span>|<span data-ttu-id="50510-141">Guid</span><span class="sxs-lookup"><span data-stu-id="50510-141">Guid</span></span>| <span data-ttu-id="50510-142">Der eindeutige Bezeichner (GUID) für die Dienst-SKU.</span><span class="sxs-lookup"><span data-stu-id="50510-142">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="50510-143">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="50510-143">skuPartNumber</span></span>|<span data-ttu-id="50510-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="50510-144">String</span></span>| <span data-ttu-id="50510-145">Die SKU-Teilenummer, z. B.: „AAD_PREMIUM“ oder „RMSBASIC“.</span><span class="sxs-lookup"><span data-stu-id="50510-145">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> |

## <a name="relationships"></a><span data-ttu-id="50510-146">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="50510-146">Relationships</span></span>
<span data-ttu-id="50510-147">Keine</span><span class="sxs-lookup"><span data-stu-id="50510-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="50510-148">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="50510-148">JSON representation</span></span>

<span data-ttu-id="50510-149">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="50510-149">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.subscribedSku",
  "@odata.annotations": [
    {
      "capabilities": {
        "skippable": false,
        "toppable": false,
        "countable": false,
        "expandable": false,
        "filterable": false,
        "referenceable": false,
        "selectable": false
      }
    }
  ]
}-->

```json
{
  "appliesTo": "string",
  "capabilityStatus": "string",
  "consumedUnits": 1024,
  "id": "string (identifier)",
  "prepaidUnits": {"@odata.type": "microsoft.graph.licenseUnitsDetail"},
  "servicePlans": [{"@odata.type": "microsoft.graph.servicePlanInfo"}],
  "skuId": "guid",
  "skuPartNumber": "string"
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscribedSku resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
