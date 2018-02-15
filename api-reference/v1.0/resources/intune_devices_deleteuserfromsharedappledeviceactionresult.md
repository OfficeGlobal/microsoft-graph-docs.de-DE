# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="f7d35-101">deleteUserFromSharedAppleDeviceActionResult-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f7d35-101">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

> <span data-ttu-id="f7d35-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f7d35-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f7d35-103">Benutzer von freigegebenem Apple-Gerät löschen – Aktionsergebnis</span><span class="sxs-lookup"><span data-stu-id="f7d35-103">Delete user from shared apple device action result</span></span>

<span data-ttu-id="f7d35-104">Erbt von [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="f7d35-104">Inherits from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f7d35-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f7d35-105">Properties</span></span>
|<span data-ttu-id="f7d35-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f7d35-106">Property</span></span>|<span data-ttu-id="f7d35-107">Typ</span><span class="sxs-lookup"><span data-stu-id="f7d35-107">Type</span></span>|<span data-ttu-id="f7d35-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f7d35-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7d35-109">actionName</span><span class="sxs-lookup"><span data-stu-id="f7d35-109">ActionName</span></span>|<span data-ttu-id="f7d35-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f7d35-110">String</span></span>|<span data-ttu-id="f7d35-111">Aktionsname, geerbt von [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="f7d35-111">Action name Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="f7d35-112">actionState</span><span class="sxs-lookup"><span data-stu-id="f7d35-112">actionState</span></span>|<span data-ttu-id="f7d35-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f7d35-113">String</span></span>|<span data-ttu-id="f7d35-114">Status der Aktion, geerbt von [deviceActionResult](../resources/intune_devices_deviceactionresult.md). Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="f7d35-114">State of the action Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md) Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="f7d35-115">startDateTime</span><span class="sxs-lookup"><span data-stu-id="f7d35-115">startDateTime</span></span>|<span data-ttu-id="f7d35-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7d35-116">DateTimeOffset</span></span>|<span data-ttu-id="f7d35-117">Zeit, zu der die Aktion initiiert wurde. Geerbt von [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="f7d35-117">Time the action was initiated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="f7d35-118">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="f7d35-118">lastUpdatedDateTime</span></span>|<span data-ttu-id="f7d35-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7d35-119">DateTimeOffset</span></span>|<span data-ttu-id="f7d35-120">Zeit, zu der der Aktionszustand zuletzt aktualisiert wurde. Geerbt von [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="f7d35-120">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="f7d35-121">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f7d35-121">userPrincipalName</span></span>|<span data-ttu-id="f7d35-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f7d35-122">String</span></span>|<span data-ttu-id="f7d35-123">Benutzerprinzipalnamen für den Benutzer, der gelöscht werden soll</span><span class="sxs-lookup"><span data-stu-id="f7d35-123">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="f7d35-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f7d35-124">Relationships</span></span>
<span data-ttu-id="f7d35-125">Keine</span><span class="sxs-lookup"><span data-stu-id="f7d35-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f7d35-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f7d35-126">JSON Representation</span></span>
<span data-ttu-id="f7d35-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f7d35-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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



