# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="eb8ea-101">windowsDefenderScanActionResult-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="eb8ea-101">windowsDefenderScanActionResult resource type</span></span>

> <span data-ttu-id="eb8ea-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="eb8ea-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eb8ea-103">Letzte Analyseergebnisse von Windows Defender</span><span class="sxs-lookup"><span data-stu-id="eb8ea-103">Windows Defender last scan result</span></span>

<span data-ttu-id="eb8ea-104">Erbt von [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="eb8ea-104">Inherits from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="eb8ea-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="eb8ea-105">Properties</span></span>
|<span data-ttu-id="eb8ea-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="eb8ea-106">Property</span></span>|<span data-ttu-id="eb8ea-107">Typ</span><span class="sxs-lookup"><span data-stu-id="eb8ea-107">Type</span></span>|<span data-ttu-id="eb8ea-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="eb8ea-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb8ea-109">actionName</span><span class="sxs-lookup"><span data-stu-id="eb8ea-109">actionName</span></span>|<span data-ttu-id="eb8ea-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="eb8ea-110">String</span></span>|<span data-ttu-id="eb8ea-111">Aktionsname, geerbt von [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="eb8ea-111">Action name Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="eb8ea-112">actionState</span><span class="sxs-lookup"><span data-stu-id="eb8ea-112">actionState</span></span>|[<span data-ttu-id="eb8ea-113">actionState</span><span class="sxs-lookup"><span data-stu-id="eb8ea-113">actionState</span></span>](../resources/intune_devices_actionstate.md)|<span data-ttu-id="eb8ea-p101">Status der Aktion. Geerbt von [DeviceActionResult](../resources/intune_devices_deviceactionresult.md). Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="eb8ea-p101">State of the action Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md) Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="eb8ea-116">startDateTime</span><span class="sxs-lookup"><span data-stu-id="eb8ea-116">startDateTime</span></span>|<span data-ttu-id="eb8ea-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb8ea-117">DateTimeOffset</span></span>|<span data-ttu-id="eb8ea-118">Zeit, zu der die Aktion initiiert wurde. Geerbt von [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="eb8ea-118">Time the action was initiated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="eb8ea-119">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="eb8ea-119">lastUpdatedDateTime</span></span>|<span data-ttu-id="eb8ea-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb8ea-120">DateTimeOffset</span></span>|<span data-ttu-id="eb8ea-121">Zeit, zu der der Aktionszustand zuletzt aktualisiert wurde. Geerbt von [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="eb8ea-121">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="eb8ea-122">scanType</span><span class="sxs-lookup"><span data-stu-id="eb8ea-122">scanType</span></span>|<span data-ttu-id="eb8ea-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="eb8ea-123">String</span></span>|<span data-ttu-id="eb8ea-124">Überprüfungstyp, entweder vollständige oder schnelle Überprüfung</span><span class="sxs-lookup"><span data-stu-id="eb8ea-124">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="eb8ea-125">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="eb8ea-125">Relationships</span></span>
<span data-ttu-id="eb8ea-126">Keine</span><span class="sxs-lookup"><span data-stu-id="eb8ea-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="eb8ea-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="eb8ea-127">JSON Representation</span></span>
<span data-ttu-id="eb8ea-128">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="eb8ea-128">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
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








