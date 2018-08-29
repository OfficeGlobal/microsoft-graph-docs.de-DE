# <a name="licensedetails-resource-type"></a><span data-ttu-id="174f5-101">licenseDetails-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="174f5-101">licenseDetails resource type</span></span>

<span data-ttu-id="174f5-102">Enthält Informationen über eine Lizenz, die einem Benutzer zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="174f5-102">Contains information about a license assigned to a user.</span></span>

## <a name="methods"></a><span data-ttu-id="174f5-103">Methoden</span><span class="sxs-lookup"><span data-stu-id="174f5-103">Methods</span></span>

| <span data-ttu-id="174f5-104">Methode</span><span class="sxs-lookup"><span data-stu-id="174f5-104">Method</span></span>           | <span data-ttu-id="174f5-105">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="174f5-105">Return Type</span></span>    |<span data-ttu-id="174f5-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="174f5-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="174f5-107">licenseDetails auflisten</span><span class="sxs-lookup"><span data-stu-id="174f5-107">List licenseDetails</span></span>](../api/user_list_licensedetails.md) | <span data-ttu-id="174f5-108">licenseDetails-Sammlung</span><span class="sxs-lookup"><span data-stu-id="174f5-108">licenseDetails collection</span></span> |<span data-ttu-id="174f5-109">Dient zum Abrufen einer Liste von licenseDetails-Objekten für einen Benutzer.</span><span class="sxs-lookup"><span data-stu-id="174f5-109">Retrieve a list of licenseDetails objects for a user.</span></span>|

<!--|[Get licenseDetails](../api/licensedetails_get.md) | licenseDetails |Read properties and relationships of a licenseDetails object.|-->

## <a name="properties"></a><span data-ttu-id="174f5-110">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="174f5-110">Properties</span></span>
| <span data-ttu-id="174f5-111">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="174f5-111">Property</span></span>     | <span data-ttu-id="174f5-112">Typ</span><span class="sxs-lookup"><span data-stu-id="174f5-112">Type</span></span>   |<span data-ttu-id="174f5-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="174f5-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="174f5-114">id</span><span class="sxs-lookup"><span data-stu-id="174f5-114">id</span></span>|<span data-ttu-id="174f5-115">String</span><span class="sxs-lookup"><span data-stu-id="174f5-115">String</span></span>| <span data-ttu-id="174f5-p101">Der eindeutige Bezeichner für das licenseDetails-Objekt. Schreibgeschützt, Schlüssel, lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="174f5-p101">The unique identifier for the license detail object. Read-only, Key, Not nullable</span></span> |
|<span data-ttu-id="174f5-118">servicePlans</span><span class="sxs-lookup"><span data-stu-id="174f5-118">servicePlans</span></span>|<span data-ttu-id="174f5-119">[servicePlanInfo](serviceplaninfo.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="174f5-119">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="174f5-p102">Informationen über die Servicepläne, die mit der Lizenz zugewiesen werden. Schreibgeschützt, lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="174f5-p102">Information about the service plans assigned with the license. Read-only, Not nullable</span></span> |
|<span data-ttu-id="174f5-122">skuId</span><span class="sxs-lookup"><span data-stu-id="174f5-122">skuId</span></span>|<span data-ttu-id="174f5-123">Guid</span><span class="sxs-lookup"><span data-stu-id="174f5-123">Guid</span></span>| <span data-ttu-id="174f5-p103">Der eindeutige Bezeichner (GUID) für die Dienst-SKU. Entspricht der skuId-Eigenschaft des zugehörigen [SubscribedSku](subscribedsku.md)-Objekts. Schreibgeschützt</span><span class="sxs-lookup"><span data-stu-id="174f5-p103">Unique identifier (GUID) for the service SKU. Equal to the skuId property on the related [SubscribedSku](subscribedsku.md) object. Read-only</span></span> |
|<span data-ttu-id="174f5-127">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="174f5-127">skuPartNumber</span></span>|<span data-ttu-id="174f5-128">String</span><span class="sxs-lookup"><span data-stu-id="174f5-128">String</span></span>| <span data-ttu-id="174f5-p104">Eindeutiger SKU-Anzeigename. Entspricht der skuPartNumber des zugehörigen [SubscribedSku](subscribedsku.md)-Objekts, z. B.: „AAD_Premium“. Schreibgeschützt</span><span class="sxs-lookup"><span data-stu-id="174f5-p104">Unique SKU display name. Equal to the skuPartNumber on the related [SubscribedSku](subscribedsku.md) object; for example: "AAD_Premium". Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="174f5-132">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="174f5-132">Relationships</span></span>
<span data-ttu-id="174f5-133">Keine</span><span class="sxs-lookup"><span data-stu-id="174f5-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="174f5-134">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="174f5-134">JSON representation</span></span>
<span data-ttu-id="174f5-135">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="174f5-135">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.licenseDetails"
}-->

```json
{
  "id": "String (identifier)",
  "servicePlans": [{"@odata.type": "microsoft.graph.servicePlanInfo"}],
  "skuId": "Guid",
  "skuPartNumber": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "licenseDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->