# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="b89f3-101">deleteUserFromSharedAppleDeviceActionResult-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b89f3-101">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

> <span data-ttu-id="b89f3-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b89f3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b89f3-103">Benutzer von freigegebenem Apple-Gerät löschen – Aktionsergebnis</span><span class="sxs-lookup"><span data-stu-id="b89f3-103">Delete user from shared apple device action result</span></span>

<span data-ttu-id="b89f3-104">Erbt von [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b89f3-104">Inherits from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b89f3-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b89f3-105">Properties</span></span>
|<span data-ttu-id="b89f3-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b89f3-106">Property</span></span>|<span data-ttu-id="b89f3-107">Typ</span><span class="sxs-lookup"><span data-stu-id="b89f3-107">Type</span></span>|<span data-ttu-id="b89f3-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b89f3-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b89f3-109">actionName</span><span class="sxs-lookup"><span data-stu-id="b89f3-109">actionName</span></span>|<span data-ttu-id="b89f3-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b89f3-110">String</span></span>|<span data-ttu-id="b89f3-111">Aktionsname, geerbt von [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b89f3-111">Action name Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="b89f3-112">actionState</span><span class="sxs-lookup"><span data-stu-id="b89f3-112">actionState</span></span>|[<span data-ttu-id="b89f3-113">actionState</span><span class="sxs-lookup"><span data-stu-id="b89f3-113">actionState</span></span>](../resources/intune_devices_actionstate.md)|<span data-ttu-id="b89f3-114">Status der Aktion, geerbt aus [DeviceActionResult](../resources/intune_devices_deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="b89f3-114">State of the action Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md) Possible values are: , , , , , , .</span></span> <span data-ttu-id="b89f3-115">Mögliche Werte: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="b89f3-115">The possible values are `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`, , , , , or .</span></span>|
|<span data-ttu-id="b89f3-116">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b89f3-116">startDateTime</span></span>|<span data-ttu-id="b89f3-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b89f3-117">DateTimeOffset</span></span>|<span data-ttu-id="b89f3-118">Zeit, zu der die Aktion initiiert wurde. Geerbt von [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b89f3-118">Time the action was initiated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="b89f3-119">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="b89f3-119">lastUpdatedDateTime</span></span>|<span data-ttu-id="b89f3-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b89f3-120">DateTimeOffset</span></span>|<span data-ttu-id="b89f3-121">Zeit, zu der der Aktionszustand zuletzt aktualisiert wurde. Geerbt von [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b89f3-121">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="b89f3-122">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b89f3-122">userPrincipalName</span></span>|<span data-ttu-id="b89f3-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b89f3-123">String</span></span>|<span data-ttu-id="b89f3-124">Benutzerprinzipalnamen für den Benutzer, der gelöscht werden soll</span><span class="sxs-lookup"><span data-stu-id="b89f3-124">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="b89f3-125">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b89f3-125">Relationships</span></span>
<span data-ttu-id="b89f3-126">Keine</span><span class="sxs-lookup"><span data-stu-id="b89f3-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b89f3-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b89f3-127">JSON Representation</span></span>
<span data-ttu-id="b89f3-128">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b89f3-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.deviceActionResult",
  "@odata.type": "microsoft.graph.deleteUserFromSharedAppleDeviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deleteUserFromSharedAppleDeviceActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```



