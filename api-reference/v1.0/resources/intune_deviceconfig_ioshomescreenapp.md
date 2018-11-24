# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="241a1-101">iosHomeScreenApp-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="241a1-101">iosHomeScreenApp resource type</span></span>

> <span data-ttu-id="241a1-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="241a1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="241a1-103">Gibt das Symbol einer App auf der Startseite an.</span><span class="sxs-lookup"><span data-stu-id="241a1-103">Represents an icon for an app on the Home Screen</span></span>

<span data-ttu-id="241a1-104">Erbt von [iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="241a1-104">Inherits from [iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="241a1-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="241a1-105">Properties</span></span>
|<span data-ttu-id="241a1-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="241a1-106">Property</span></span>|<span data-ttu-id="241a1-107">Typ</span><span class="sxs-lookup"><span data-stu-id="241a1-107">Type</span></span>|<span data-ttu-id="241a1-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="241a1-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="241a1-109">displayName</span><span class="sxs-lookup"><span data-stu-id="241a1-109">displayName</span></span>|<span data-ttu-id="241a1-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="241a1-110">String</span></span>|<span data-ttu-id="241a1-111">Name der von [iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md) geerbten App</span><span class="sxs-lookup"><span data-stu-id="241a1-111">Name of the app Inherited from [iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="241a1-112">bundleID</span><span class="sxs-lookup"><span data-stu-id="241a1-112">bundleID</span></span>|<span data-ttu-id="241a1-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="241a1-113">String</span></span>|<span data-ttu-id="241a1-114">Paket-ID der App</span><span class="sxs-lookup"><span data-stu-id="241a1-114">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="241a1-115">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="241a1-115">Relationships</span></span>
<span data-ttu-id="241a1-116">Keine</span><span class="sxs-lookup"><span data-stu-id="241a1-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="241a1-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="241a1-117">JSON Representation</span></span>
<span data-ttu-id="241a1-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="241a1-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenApp",
  "displayName": "String",
  "bundleID": "String"
}
```



