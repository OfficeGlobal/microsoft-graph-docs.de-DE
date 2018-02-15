# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="d7799-101">iosDeviceType-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d7799-101">iosDeviceType resource type</span></span>

> <span data-ttu-id="d7799-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d7799-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d7799-103">Enthält die Eigenschaften der möglichen iOS-Gerätetypen, auf denen die mobile App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="d7799-103">Contains properties of the possible iOS device types the mobile app can run on.</span></span>
## <a name="properties"></a><span data-ttu-id="d7799-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d7799-104">Properties</span></span>
|<span data-ttu-id="d7799-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d7799-105">Property</span></span>|<span data-ttu-id="d7799-106">Typ</span><span class="sxs-lookup"><span data-stu-id="d7799-106">Type</span></span>|<span data-ttu-id="d7799-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d7799-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7799-108">iPad</span><span class="sxs-lookup"><span data-stu-id="d7799-108">iPad</span></span>|<span data-ttu-id="d7799-109">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d7799-109">Boolean</span></span>|<span data-ttu-id="d7799-110">Gibt an, ob die App auf iPads ausgeführt werden soll.</span><span class="sxs-lookup"><span data-stu-id="d7799-110">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="d7799-111">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="d7799-111">iPhoneAndIPod</span></span>|<span data-ttu-id="d7799-112">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d7799-112">Boolean</span></span>|<span data-ttu-id="d7799-113">Gibt an, ob die App auf iPhones und iPads ausgeführt werden soll.</span><span class="sxs-lookup"><span data-stu-id="d7799-113">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d7799-114">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d7799-114">Relationships</span></span>
<span data-ttu-id="d7799-115">Keine</span><span class="sxs-lookup"><span data-stu-id="d7799-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d7799-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d7799-116">JSON Representation</span></span>
<span data-ttu-id="d7799-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d7799-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosDeviceType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosDeviceType",
  "iPad": true,
  "iPhoneAndIPod": true
}
```



