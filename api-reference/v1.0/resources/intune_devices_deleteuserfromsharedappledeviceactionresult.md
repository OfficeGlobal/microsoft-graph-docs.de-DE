# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="bc7e7-101">deleteUserFromSharedAppleDeviceActionResult-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="bc7e7-101">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

> <span data-ttu-id="bc7e7-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="bc7e7-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bc7e7-103">Benutzer von freigegebenem Apple-Gerät löschen – Aktionsergebnis</span><span class="sxs-lookup"><span data-stu-id="bc7e7-103">Delete user from shared apple device action result</span></span>

<span data-ttu-id="bc7e7-104">Erbt von [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="bc7e7-104">Inherits from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bc7e7-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bc7e7-105">Properties</span></span>
|<span data-ttu-id="bc7e7-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bc7e7-106">Property</span></span>|<span data-ttu-id="bc7e7-107">Typ</span><span class="sxs-lookup"><span data-stu-id="bc7e7-107">Type</span></span>|<span data-ttu-id="bc7e7-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bc7e7-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc7e7-109">actionName</span><span class="sxs-lookup"><span data-stu-id="bc7e7-109">actionName</span></span>|<span data-ttu-id="bc7e7-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bc7e7-110">String</span></span>|<span data-ttu-id="bc7e7-111">Aktionsname, geerbt von [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="bc7e7-111">Action name Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="bc7e7-112">actionState</span><span class="sxs-lookup"><span data-stu-id="bc7e7-112">actionState</span></span>|[<span data-ttu-id="bc7e7-113">actionState</span><span class="sxs-lookup"><span data-stu-id="bc7e7-113">actionState</span></span>](../resources/intune_devices_actionstate.md)|<span data-ttu-id="bc7e7-p101">Status der Aktion. Geerbt von [DeviceActionResult](../resources/intune_devices_deviceactionresult.md). Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="bc7e7-p101">State of the action Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md) Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="bc7e7-116">startDateTime</span><span class="sxs-lookup"><span data-stu-id="bc7e7-116">startDateTime</span></span>|<span data-ttu-id="bc7e7-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc7e7-117">DateTimeOffset</span></span>|<span data-ttu-id="bc7e7-118">Zeit, zu der die Aktion initiiert wurde. Geerbt von [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="bc7e7-118">Time the action was initiated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="bc7e7-119">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="bc7e7-119">lastUpdatedDateTime</span></span>|<span data-ttu-id="bc7e7-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc7e7-120">DateTimeOffset</span></span>|<span data-ttu-id="bc7e7-121">Zeit, zu der der Aktionszustand zuletzt aktualisiert wurde. Geerbt von [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="bc7e7-121">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="bc7e7-122">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="bc7e7-122">userPrincipalName</span></span>|<span data-ttu-id="bc7e7-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bc7e7-123">String</span></span>|<span data-ttu-id="bc7e7-124">Benutzerprinzipalnamen für den Benutzer, der gelöscht werden soll</span><span class="sxs-lookup"><span data-stu-id="bc7e7-124">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc7e7-125">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="bc7e7-125">Relationships</span></span>
<span data-ttu-id="bc7e7-126">Keine</span><span class="sxs-lookup"><span data-stu-id="bc7e7-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bc7e7-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bc7e7-127">JSON Representation</span></span>
<span data-ttu-id="bc7e7-128">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="bc7e7-128">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deleteUserFromSharedAppleDeviceActionResult"
}-->
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








