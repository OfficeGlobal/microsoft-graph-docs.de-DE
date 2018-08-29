# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="e654c-101">iosVppAppAssignmentSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e654c-101">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="e654c-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e654c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e654c-103">Enthält Eigenschaften zum Zuweisen einer mobilen iOS-VPP-App zu einer Gruppe.</span><span class="sxs-lookup"><span data-stu-id="e654c-103">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>

<span data-ttu-id="e654c-104">Erbt von [mobileAppAssignmentSettings](../resources/intune_apps_mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="e654c-104">Inherits from [mobileAppAssignmentSettings](../resources/intune_apps_mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e654c-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e654c-105">Properties</span></span>
|<span data-ttu-id="e654c-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e654c-106">Property</span></span>|<span data-ttu-id="e654c-107">Typ</span><span class="sxs-lookup"><span data-stu-id="e654c-107">Type</span></span>|<span data-ttu-id="e654c-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e654c-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e654c-109">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="e654c-109">useDeviceLicensing</span></span>|<span data-ttu-id="e654c-110">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e654c-110">Boolean</span></span>|<span data-ttu-id="e654c-111">Gibt an, ob die Gerätelizenzierung verwendet werden soll oder nicht.</span><span class="sxs-lookup"><span data-stu-id="e654c-111">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="e654c-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="e654c-112">vpnConfigurationId</span></span>|<span data-ttu-id="e654c-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e654c-113">String</span></span>|<span data-ttu-id="e654c-114">Die VPN-Konfigurations-ID, die für diese App verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="e654c-114">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e654c-115">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e654c-115">Relationships</span></span>
<span data-ttu-id="e654c-116">Keine</span><span class="sxs-lookup"><span data-stu-id="e654c-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e654c-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e654c-117">JSON Representation</span></span>
<span data-ttu-id="e654c-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e654c-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.mobileAppAssignmentSettings",
  "@odata.type": "microsoft.graph.iosVppAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppAppAssignmentSettings",
  "useDeviceLicensing": true,
  "vpnConfigurationId": "String"
}
```



