# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="73fea-101">remoteLockActionResult-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="73fea-101">remoteLockActionResult resource type</span></span>

> <span data-ttu-id="73fea-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="73fea-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="73fea-103">Ergebnis einer Sperraktion mit einem Pin zum Entsperren</span><span class="sxs-lookup"><span data-stu-id="73fea-103">Lock action result with a pin to unlock</span></span>

<span data-ttu-id="73fea-104">Erbt von [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="73fea-104">Inherits from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="73fea-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="73fea-105">Properties</span></span>
|<span data-ttu-id="73fea-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="73fea-106">Property</span></span>|<span data-ttu-id="73fea-107">Typ</span><span class="sxs-lookup"><span data-stu-id="73fea-107">Type</span></span>|<span data-ttu-id="73fea-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="73fea-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73fea-109">actionName</span><span class="sxs-lookup"><span data-stu-id="73fea-109">ActionName</span></span>|<span data-ttu-id="73fea-110">String</span><span class="sxs-lookup"><span data-stu-id="73fea-110">String</span></span>|<span data-ttu-id="73fea-111">Aktionsname, geerbt von [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="73fea-111">Action name Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="73fea-112">actionState</span><span class="sxs-lookup"><span data-stu-id="73fea-112">actionState</span></span>|<span data-ttu-id="73fea-113">String</span><span class="sxs-lookup"><span data-stu-id="73fea-113">String</span></span>|<span data-ttu-id="73fea-114">Status der Aktion, geerbt von [deviceActionResult](../resources/intune_devices_deviceactionresult.md). Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="73fea-114">State of the action Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md) Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="73fea-115">startDateTime</span><span class="sxs-lookup"><span data-stu-id="73fea-115">startDateTime</span></span>|<span data-ttu-id="73fea-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73fea-116">DateTimeOffset</span></span>|<span data-ttu-id="73fea-117">Zeit, zu der die Aktion initiiert wurde. Geerbt von [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="73fea-117">Time the action was initiated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="73fea-118">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="73fea-118">lastUpdatedDateTime</span></span>|<span data-ttu-id="73fea-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73fea-119">DateTimeOffset</span></span>|<span data-ttu-id="73fea-120">Zeit, zu der der Aktionszustand zuletzt aktualisiert wurde. Geerbt von [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="73fea-120">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="73fea-121">unlockPin</span><span class="sxs-lookup"><span data-stu-id="73fea-121">unlockPin</span></span>|<span data-ttu-id="73fea-122">String</span><span class="sxs-lookup"><span data-stu-id="73fea-122">String</span></span>|<span data-ttu-id="73fea-123">Pin zum Entsperren des Clients</span><span class="sxs-lookup"><span data-stu-id="73fea-123">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="73fea-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="73fea-124">Relationships</span></span>
<span data-ttu-id="73fea-125">Keine</span><span class="sxs-lookup"><span data-stu-id="73fea-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="73fea-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="73fea-126">JSON Representation</span></span>
<span data-ttu-id="73fea-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="73fea-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.remoteLockActionResult"
}
-->
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



