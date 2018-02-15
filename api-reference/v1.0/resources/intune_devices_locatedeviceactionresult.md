# <a name="locatedeviceactionresult-resource-type"></a><span data-ttu-id="72c5e-101">locateDeviceActionResult-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="72c5e-101">locateDeviceActionResult resource type</span></span>

> <span data-ttu-id="72c5e-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="72c5e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="72c5e-103">Gerät suchen – Aktionsergebnis</span><span class="sxs-lookup"><span data-stu-id="72c5e-103">Locate device action result</span></span>

<span data-ttu-id="72c5e-104">Erbt von [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="72c5e-104">Inherits from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="72c5e-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="72c5e-105">Properties</span></span>
|<span data-ttu-id="72c5e-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="72c5e-106">Property</span></span>|<span data-ttu-id="72c5e-107">Typ</span><span class="sxs-lookup"><span data-stu-id="72c5e-107">Type</span></span>|<span data-ttu-id="72c5e-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="72c5e-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72c5e-109">actionName</span><span class="sxs-lookup"><span data-stu-id="72c5e-109">ActionName</span></span>|<span data-ttu-id="72c5e-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="72c5e-110">String</span></span>|<span data-ttu-id="72c5e-111">Aktionsname, geerbt von [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="72c5e-111">Action name Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="72c5e-112">actionState</span><span class="sxs-lookup"><span data-stu-id="72c5e-112">actionState</span></span>|<span data-ttu-id="72c5e-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="72c5e-113">String</span></span>|<span data-ttu-id="72c5e-114">Status der Aktion, geerbt von [deviceActionResult](../resources/intune_devices_deviceactionresult.md). Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="72c5e-114">State of the action Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md) Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="72c5e-115">startDateTime</span><span class="sxs-lookup"><span data-stu-id="72c5e-115">startDateTime</span></span>|<span data-ttu-id="72c5e-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72c5e-116">DateTimeOffset</span></span>|<span data-ttu-id="72c5e-117">Zeit, zu der die Aktion initiiert wurde. Geerbt von [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="72c5e-117">Time the action was initiated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="72c5e-118">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="72c5e-118">lastUpdatedDateTime</span></span>|<span data-ttu-id="72c5e-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72c5e-119">DateTimeOffset</span></span>|<span data-ttu-id="72c5e-120">Zeit, zu der der Aktionszustand zuletzt aktualisiert wurde. Geerbt von [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="72c5e-120">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="72c5e-121">deviceLocation</span><span class="sxs-lookup"><span data-stu-id="72c5e-121">deviceLocation</span></span>|[<span data-ttu-id="72c5e-122">deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="72c5e-122">deviceGeoLocation</span></span>](../resources/intune_devices_devicegeolocation.md)|<span data-ttu-id="72c5e-123">Standort des Geräts</span><span class="sxs-lookup"><span data-stu-id="72c5e-123">device location</span></span>|

## <a name="relationships"></a><span data-ttu-id="72c5e-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="72c5e-124">Relationships</span></span>
<span data-ttu-id="72c5e-125">Keine</span><span class="sxs-lookup"><span data-stu-id="72c5e-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="72c5e-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="72c5e-126">JSON Representation</span></span>
<span data-ttu-id="72c5e-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="72c5e-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.locateDeviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.locateDeviceActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "deviceLocation": {
    "@odata.type": "microsoft.graph.deviceGeoLocation",
    "lastCollectedDateTime": "String (timestamp)",
    "longitude": "<Unknown Primitive Type Edm.Double>",
    "latitude": "<Unknown Primitive Type Edm.Double>",
    "altitude": "<Unknown Primitive Type Edm.Double>",
    "horizontalAccuracy": "<Unknown Primitive Type Edm.Double>",
    "verticalAccuracy": "<Unknown Primitive Type Edm.Double>",
    "heading": "<Unknown Primitive Type Edm.Double>",
    "speed": "<Unknown Primitive Type Edm.Double>"
  }
}
```



