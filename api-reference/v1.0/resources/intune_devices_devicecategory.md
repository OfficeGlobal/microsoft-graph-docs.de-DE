# <a name="devicecategory-resource-type"></a><span data-ttu-id="8a724-101">deviceCategory-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8a724-101">deviceCategory resource type</span></span>

> <span data-ttu-id="8a724-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8a724-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8a724-103">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="8a724-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="8a724-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="8a724-104">Methods</span></span>
|<span data-ttu-id="8a724-105">Methode</span><span class="sxs-lookup"><span data-stu-id="8a724-105">Method</span></span>|<span data-ttu-id="8a724-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="8a724-106">Return Type</span></span>|<span data-ttu-id="8a724-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8a724-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8a724-108">deviceCategory abrufen</span><span class="sxs-lookup"><span data-stu-id="8a724-108">Get deviceCategory</span></span>](../api/intune_devices_devicecategory_get.md)|[<span data-ttu-id="8a724-109">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="8a724-109">deviceCategory</span></span>](../resources/intune_devices_devicecategory.md)|<span data-ttu-id="8a724-110">Lesen von Eigenschaften und Beziehungen des [deviceCategory](../resources/intune_devices_devicecategory.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="8a724-110">Read properties and relationships of [plannerPlanDetails](../resources/intune_devices_devicecategory.md) object.</span></span>|
|[<span data-ttu-id="8a724-111">deviceCategory aktualisieren</span><span class="sxs-lookup"><span data-stu-id="8a724-111">Update deviceCategory</span></span>](../api/intune_devices_devicecategory_update.md)|[<span data-ttu-id="8a724-112">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="8a724-112">deviceCategory</span></span>](../resources/intune_devices_devicecategory.md)|<span data-ttu-id="8a724-113">Aktualisieren der Eigenschaften eines [deviceCategory](../resources/intune_devices_devicecategory.md)-Objekts</span><span class="sxs-lookup"><span data-stu-id="8a724-113">Update the properties of a [calendar](../resources/intune_devices_devicecategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8a724-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8a724-114">Properties</span></span>
|<span data-ttu-id="8a724-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8a724-115">Property</span></span>|<span data-ttu-id="8a724-116">Typ</span><span class="sxs-lookup"><span data-stu-id="8a724-116">Type</span></span>|<span data-ttu-id="8a724-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8a724-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a724-118">id</span><span class="sxs-lookup"><span data-stu-id="8a724-118">id</span></span>|<span data-ttu-id="8a724-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8a724-119">String</span></span>|<span data-ttu-id="8a724-120">Der eindeutige Bezeichner für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="8a724-120">Unique identifier for the device category.</span></span> <span data-ttu-id="8a724-121">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8a724-121">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8a724-122">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8a724-122">Relationships</span></span>
<span data-ttu-id="8a724-123">Keine</span><span class="sxs-lookup"><span data-stu-id="8a724-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8a724-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8a724-124">JSON Representation</span></span>
<span data-ttu-id="8a724-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8a724-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "String (identifier)"
}
```



