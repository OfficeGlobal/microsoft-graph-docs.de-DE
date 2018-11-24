# <a name="iosnetworkusagerule-resource-type"></a><span data-ttu-id="6f477-101">iosNetworkUsageRule-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6f477-101">iosNetworkUsageRule resource type</span></span>

> <span data-ttu-id="6f477-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6f477-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6f477-103">In Netzwerknutzungsregeln können Unternehmen angeben, wie verwaltete Apps Netzwerke, beispielsweise Mobilfunknetze, verwenden.</span><span class="sxs-lookup"><span data-stu-id="6f477-103">Network Usage Rules allow enterprises to specify how managed apps use networks, such as cellular data networks.</span></span>
## <a name="properties"></a><span data-ttu-id="6f477-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6f477-104">Properties</span></span>
|<span data-ttu-id="6f477-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6f477-105">Property</span></span>|<span data-ttu-id="6f477-106">Typ</span><span class="sxs-lookup"><span data-stu-id="6f477-106">Type</span></span>|<span data-ttu-id="6f477-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6f477-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f477-108">managedApps</span><span class="sxs-lookup"><span data-stu-id="6f477-108">managedApps</span></span>|<span data-ttu-id="6f477-109">[appListItem](../resources/intune_deviceconfig_applistitem.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6f477-109">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="6f477-110">Informationen zu den verwalteten Apps, auf die diese Regel angewendet werden wird.</span><span class="sxs-lookup"><span data-stu-id="6f477-110">Information about the managed apps that this rule is going to apply to.</span></span> <span data-ttu-id="6f477-111">Diese Sammlung kann bis zu 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="6f477-111">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="6f477-112">cellularDataBlockWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="6f477-112">cellularDataBlockWhenRoaming</span></span>|<span data-ttu-id="6f477-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f477-113">Boolean</span></span>|<span data-ttu-id="6f477-114">Wenn dies auf „true“ festgelegt wird, können die entsprechenden verwalteten Apps beim Roaming keine mobilen Daten verwenden.</span><span class="sxs-lookup"><span data-stu-id="6f477-114">If set to true, corresponding managed apps will not be allowed to use cellular data when roaming.</span></span>|
|<span data-ttu-id="6f477-115">cellularDataBlocked</span><span class="sxs-lookup"><span data-stu-id="6f477-115">cellularDataBlocked</span></span>|<span data-ttu-id="6f477-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f477-116">Boolean</span></span>|<span data-ttu-id="6f477-117">Wenn dies auf „true“ festgelegt wird, können die entsprechenden verwalteten Apps zu keiner Zeit mobile Daten verwenden.</span><span class="sxs-lookup"><span data-stu-id="6f477-117">If set to true, corresponding managed apps will not be allowed to use cellular data at any time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6f477-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6f477-118">Relationships</span></span>
<span data-ttu-id="6f477-119">Keine</span><span class="sxs-lookup"><span data-stu-id="6f477-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6f477-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6f477-120">JSON Representation</span></span>
<span data-ttu-id="6f477-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6f477-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosNetworkUsageRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosNetworkUsageRule",
  "managedApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "cellularDataBlockWhenRoaming": true,
  "cellularDataBlocked": true
}
```



