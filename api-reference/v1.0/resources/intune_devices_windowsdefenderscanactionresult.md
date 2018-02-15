# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="31dff-101">windowsDefenderScanActionResult-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="31dff-101">windowsDefenderScanActionResult resource type</span></span>

> <span data-ttu-id="31dff-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="31dff-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="31dff-103">Letzte Analyseergebnisse von Windows Defender</span><span class="sxs-lookup"><span data-stu-id="31dff-103">Windows Defender last scan result</span></span>

<span data-ttu-id="31dff-104">Erbt von [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="31dff-104">Inherits from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="31dff-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="31dff-105">Properties</span></span>
|<span data-ttu-id="31dff-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="31dff-106">Property</span></span>|<span data-ttu-id="31dff-107">Typ</span><span class="sxs-lookup"><span data-stu-id="31dff-107">Type</span></span>|<span data-ttu-id="31dff-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="31dff-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31dff-109">actionName</span><span class="sxs-lookup"><span data-stu-id="31dff-109">ActionName</span></span>|<span data-ttu-id="31dff-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="31dff-110">String</span></span>|<span data-ttu-id="31dff-111">Aktionsname, geerbt von [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="31dff-111">Action name Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="31dff-112">actionState</span><span class="sxs-lookup"><span data-stu-id="31dff-112">actionState</span></span>|<span data-ttu-id="31dff-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="31dff-113">String</span></span>|<span data-ttu-id="31dff-114">Status der Aktion, geerbt von [deviceActionResult](../resources/intune_devices_deviceactionresult.md). Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="31dff-114">State of the action Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md) Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="31dff-115">startDateTime</span><span class="sxs-lookup"><span data-stu-id="31dff-115">startDateTime</span></span>|<span data-ttu-id="31dff-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31dff-116">DateTimeOffset</span></span>|<span data-ttu-id="31dff-117">Zeit, zu der die Aktion initiiert wurde. Geerbt von [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="31dff-117">Time the action was initiated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="31dff-118">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="31dff-118">lastUpdatedDateTime</span></span>|<span data-ttu-id="31dff-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31dff-119">DateTimeOffset</span></span>|<span data-ttu-id="31dff-120">Zeit, zu der der Aktionszustand zuletzt aktualisiert wurde. Geerbt von [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="31dff-120">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="31dff-121">scanType</span><span class="sxs-lookup"><span data-stu-id="31dff-121">scanType</span></span>|<span data-ttu-id="31dff-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="31dff-122">String</span></span>|<span data-ttu-id="31dff-123">Überprüfungstyp, entweder vollständige oder schnelle Überprüfung</span><span class="sxs-lookup"><span data-stu-id="31dff-123">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="31dff-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="31dff-124">Relationships</span></span>
<span data-ttu-id="31dff-125">Keine</span><span class="sxs-lookup"><span data-stu-id="31dff-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="31dff-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="31dff-126">JSON Representation</span></span>
<span data-ttu-id="31dff-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="31dff-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsDefenderScanActionResult"
}
-->
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



