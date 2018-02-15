# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="6aff3-101">iosLobAppAssignmentSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6aff3-101">iosLobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="6aff3-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6aff3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6aff3-103">Enthält Eigenschaften zum Zuweisen einer mobilen iOS-Branchen-App zu einer Gruppe.</span><span class="sxs-lookup"><span data-stu-id="6aff3-103">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>

<span data-ttu-id="6aff3-104">Erbt von [mobileAppAssignmentSettings](../resources/intune_apps_mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="6aff3-104">Inherits from [mobileAppAssignmentSettings](../resources/intune_apps_mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6aff3-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6aff3-105">Properties</span></span>
|<span data-ttu-id="6aff3-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6aff3-106">Property</span></span>|<span data-ttu-id="6aff3-107">Typ</span><span class="sxs-lookup"><span data-stu-id="6aff3-107">Type</span></span>|<span data-ttu-id="6aff3-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6aff3-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6aff3-109">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="6aff3-109">vpnConfigurationId</span></span>|<span data-ttu-id="6aff3-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6aff3-110">String</span></span>|<span data-ttu-id="6aff3-111">Die VPN-Konfigurations-ID, die für diese App verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="6aff3-111">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6aff3-112">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6aff3-112">Relationships</span></span>
<span data-ttu-id="6aff3-113">Keine</span><span class="sxs-lookup"><span data-stu-id="6aff3-113">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6aff3-114">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6aff3-114">JSON Representation</span></span>
<span data-ttu-id="6aff3-115">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6aff3-115">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosLobAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosLobAppAssignmentSettings",
  "vpnConfigurationId": "String"
}
```



