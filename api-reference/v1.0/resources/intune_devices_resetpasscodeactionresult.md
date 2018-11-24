# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="fc02f-101">resetPasscodeActionResult-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="fc02f-101">resetPasscodeActionResult resource type</span></span>

> <span data-ttu-id="fc02f-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="fc02f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fc02f-103">Kennung zurücksetzen – Aktionsergebnis</span><span class="sxs-lookup"><span data-stu-id="fc02f-103">Reset passcode action result</span></span>

<span data-ttu-id="fc02f-104">Erbt von [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="fc02f-104">Inherits from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fc02f-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="fc02f-105">Properties</span></span>
|<span data-ttu-id="fc02f-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fc02f-106">Property</span></span>|<span data-ttu-id="fc02f-107">Typ</span><span class="sxs-lookup"><span data-stu-id="fc02f-107">Type</span></span>|<span data-ttu-id="fc02f-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fc02f-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc02f-109">actionName</span><span class="sxs-lookup"><span data-stu-id="fc02f-109">actionName</span></span>|<span data-ttu-id="fc02f-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fc02f-110">String</span></span>|<span data-ttu-id="fc02f-111">Aktionsname, geerbt von [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="fc02f-111">Action name Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="fc02f-112">actionState</span><span class="sxs-lookup"><span data-stu-id="fc02f-112">actionState</span></span>|[<span data-ttu-id="fc02f-113">actionState</span><span class="sxs-lookup"><span data-stu-id="fc02f-113">actionState</span></span>](../resources/intune_devices_actionstate.md)|<span data-ttu-id="fc02f-114">Status der Aktion Inherited aus [DeviceActionResult](../resources/intune_devices_deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="fc02f-114">State of the action Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md).</span></span> <span data-ttu-id="fc02f-115">Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="fc02f-115">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="fc02f-116">startDateTime</span><span class="sxs-lookup"><span data-stu-id="fc02f-116">startDateTime</span></span>|<span data-ttu-id="fc02f-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc02f-117">DateTimeOffset</span></span>|<span data-ttu-id="fc02f-118">Zeit, zu der die Aktion initiiert wurde. Geerbt von [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="fc02f-118">Time the action was initiated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="fc02f-119">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="fc02f-119">lastUpdatedDateTime</span></span>|<span data-ttu-id="fc02f-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc02f-120">DateTimeOffset</span></span>|<span data-ttu-id="fc02f-121">Zeit, zu der der Aktionszustand zuletzt aktualisiert wurde. Geerbt von [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="fc02f-121">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="fc02f-122">Zugangscode</span><span class="sxs-lookup"><span data-stu-id="fc02f-122">passcode</span></span>|<span data-ttu-id="fc02f-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fc02f-123">String</span></span>|<span data-ttu-id="fc02f-124">Neu erstellter Zugangscode für das Gerät</span><span class="sxs-lookup"><span data-stu-id="fc02f-124">Newly generated passcode for the device</span></span> |

## <a name="relationships"></a><span data-ttu-id="fc02f-125">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="fc02f-125">Relationships</span></span>
<span data-ttu-id="fc02f-126">Keine</span><span class="sxs-lookup"><span data-stu-id="fc02f-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fc02f-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="fc02f-127">JSON Representation</span></span>
<span data-ttu-id="fc02f-128">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="fc02f-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.resetPasscodeActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resetPasscodeActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "passcode": "String"
}
```



