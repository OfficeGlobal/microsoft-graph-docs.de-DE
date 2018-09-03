# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="27ef1-101">windowsDefenderScanActionResult-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="27ef1-101">windowsDefenderScanActionResult resource type</span></span>

> <span data-ttu-id="27ef1-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="27ef1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="27ef1-103">Letzte Analyseergebnisse von Windows Defender</span><span class="sxs-lookup"><span data-stu-id="27ef1-103">Windows Defender last scan result</span></span>

<span data-ttu-id="27ef1-104">Erbt von [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="27ef1-104">Inherits from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="27ef1-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="27ef1-105">Properties</span></span>
|<span data-ttu-id="27ef1-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="27ef1-106">Property</span></span>|<span data-ttu-id="27ef1-107">Typ</span><span class="sxs-lookup"><span data-stu-id="27ef1-107">Type</span></span>|<span data-ttu-id="27ef1-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="27ef1-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27ef1-109">actionName</span><span class="sxs-lookup"><span data-stu-id="27ef1-109">actionName</span></span>|<span data-ttu-id="27ef1-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="27ef1-110">String</span></span>|<span data-ttu-id="27ef1-111">Aktionsname, geerbt von [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="27ef1-111">Action name Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="27ef1-112">actionState</span><span class="sxs-lookup"><span data-stu-id="27ef1-112">actionState</span></span>|[<span data-ttu-id="27ef1-113">actionState</span><span class="sxs-lookup"><span data-stu-id="27ef1-113">actionState</span></span>](../resources/intune_devices_actionstate.md)|<span data-ttu-id="27ef1-114">Status der Aktion, geerbt aus [ DeviceActionResult.](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="27ef1-114">State of the action Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md) Possible values are: , , , , , , .</span></span> <span data-ttu-id="27ef1-115">Die möglichen Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="27ef1-115">The possible values are `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`, , , , , or .</span></span>|
|<span data-ttu-id="27ef1-116">startDateTime</span><span class="sxs-lookup"><span data-stu-id="27ef1-116">startDateTime</span></span>|<span data-ttu-id="27ef1-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27ef1-117">DateTimeOffset</span></span>|<span data-ttu-id="27ef1-118">Zeit, zu der die Aktion initiiert wurde. Geerbt von [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="27ef1-118">Time the action was initiated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="27ef1-119">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="27ef1-119">lastUpdatedDateTime</span></span>|<span data-ttu-id="27ef1-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27ef1-120">DateTimeOffset</span></span>|<span data-ttu-id="27ef1-121">Zeit, zu der der Aktionszustand zuletzt aktualisiert wurde. Geerbt von [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="27ef1-121">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="27ef1-122">scanType</span><span class="sxs-lookup"><span data-stu-id="27ef1-122">scanType</span></span>|<span data-ttu-id="27ef1-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="27ef1-123">String</span></span>|<span data-ttu-id="27ef1-124">Überprüfungstyp, entweder vollständige oder schnelle Überprüfung</span><span class="sxs-lookup"><span data-stu-id="27ef1-124">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="27ef1-125">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="27ef1-125">Relationships</span></span>
<span data-ttu-id="27ef1-126">Keine</span><span class="sxs-lookup"><span data-stu-id="27ef1-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="27ef1-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="27ef1-127">JSON Representation</span></span>
<span data-ttu-id="27ef1-128">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="27ef1-128">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.deviceActionResult",
  "@odata.type": "microsoft.graph.windowsDefenderScanActionResult"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDefenderScanActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "scanType": "String"
}
```



