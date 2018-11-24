# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="b8660-101">iosStoreAppAssignmentSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b8660-101">iosStoreAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="b8660-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b8660-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b8660-103">Enthält Eigenschaften zum Zuweisen einer mobilen iOS-Store-App zu einer Gruppe.</span><span class="sxs-lookup"><span data-stu-id="b8660-103">Contains properties used to assign an iOS Store mobile app to a group.</span></span>

<span data-ttu-id="b8660-104">Erbt von [mobileAppAssignmentSettings](../resources/intune_apps_mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="b8660-104">Inherits from [mobileAppAssignmentSettings](../resources/intune_apps_mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b8660-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b8660-105">Properties</span></span>
|<span data-ttu-id="b8660-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b8660-106">Property</span></span>|<span data-ttu-id="b8660-107">Typ</span><span class="sxs-lookup"><span data-stu-id="b8660-107">Type</span></span>|<span data-ttu-id="b8660-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b8660-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8660-109">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="b8660-109">vpnConfigurationId</span></span>|<span data-ttu-id="b8660-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b8660-110">String</span></span>|<span data-ttu-id="b8660-111">Die VPN-Konfigurations-ID, die für diese App verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="b8660-111">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8660-112">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b8660-112">Relationships</span></span>
<span data-ttu-id="b8660-113">Keine</span><span class="sxs-lookup"><span data-stu-id="b8660-113">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b8660-114">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b8660-114">JSON Representation</span></span>
<span data-ttu-id="b8660-115">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b8660-115">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosStoreAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosStoreAppAssignmentSettings",
  "vpnConfigurationId": "String"
}
```



