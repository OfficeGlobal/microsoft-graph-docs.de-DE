# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="5eb28-101">remoteLockActionResult-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="5eb28-101">remoteLockActionResult resource type</span></span>

> <span data-ttu-id="5eb28-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5eb28-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5eb28-103">Ergebnis einer Sperraktion mit einem Pin zum Entsperren</span><span class="sxs-lookup"><span data-stu-id="5eb28-103">Lock action result with a pin to unlock</span></span>

<span data-ttu-id="5eb28-104">Erbt von [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="5eb28-104">Inherits from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5eb28-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5eb28-105">Properties</span></span>
|<span data-ttu-id="5eb28-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5eb28-106">Property</span></span>|<span data-ttu-id="5eb28-107">Typ</span><span class="sxs-lookup"><span data-stu-id="5eb28-107">Type</span></span>|<span data-ttu-id="5eb28-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5eb28-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5eb28-109">actionName</span><span class="sxs-lookup"><span data-stu-id="5eb28-109">actionName</span></span>|<span data-ttu-id="5eb28-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5eb28-110">String</span></span>|<span data-ttu-id="5eb28-111">Aktionsname, geerbt von [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="5eb28-111">Action name Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="5eb28-112">actionState</span><span class="sxs-lookup"><span data-stu-id="5eb28-112">actionState</span></span>|[<span data-ttu-id="5eb28-113">actionState</span><span class="sxs-lookup"><span data-stu-id="5eb28-113">actionState</span></span>](../resources/intune_devices_actionstate.md)|<span data-ttu-id="5eb28-114">Zustand der aus [DeviceActionResult](../resources/intune_devices_deviceactionresult.md) geerbten Aktion.</span><span class="sxs-lookup"><span data-stu-id="5eb28-114">State of the action Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md) Possible values are: , , , , , , .</span></span> <span data-ttu-id="5eb28-115">Mögliche Werte: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="5eb28-115">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="5eb28-116">startDateTime</span><span class="sxs-lookup"><span data-stu-id="5eb28-116">startDateTime</span></span>|<span data-ttu-id="5eb28-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5eb28-117">DateTimeOffset</span></span>|<span data-ttu-id="5eb28-118">Zeit, zu der die Aktion initiiert wurde. Geerbt von [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="5eb28-118">Time the action was initiated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="5eb28-119">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="5eb28-119">lastUpdatedDateTime</span></span>|<span data-ttu-id="5eb28-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5eb28-120">DateTimeOffset</span></span>|<span data-ttu-id="5eb28-121">Zeit, zu der der Aktionszustand zuletzt aktualisiert wurde. Geerbt von [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="5eb28-121">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="5eb28-122">unlockPin</span><span class="sxs-lookup"><span data-stu-id="5eb28-122">unlockPin</span></span>|<span data-ttu-id="5eb28-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5eb28-123">String</span></span>|<span data-ttu-id="5eb28-124">Pin zum Entsperren des Clients</span><span class="sxs-lookup"><span data-stu-id="5eb28-124">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="5eb28-125">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="5eb28-125">Relationships</span></span>
<span data-ttu-id="5eb28-126">Keine</span><span class="sxs-lookup"><span data-stu-id="5eb28-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5eb28-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5eb28-127">JSON Representation</span></span>
<span data-ttu-id="5eb28-128">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5eb28-128">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.remoteLockActionResult"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.remoteLockActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "unlockPin": "String"
}
```








