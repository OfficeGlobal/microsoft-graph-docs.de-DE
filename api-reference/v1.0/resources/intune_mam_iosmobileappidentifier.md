# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="c6ce2-101">iosMobileAppIdentifier-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c6ce2-101">iosMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="c6ce2-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c6ce2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c6ce2-103">Der Bezeichner für eine iOS-App.</span><span class="sxs-lookup"><span data-stu-id="c6ce2-103">The identifier for an iOS app.</span></span>

<span data-ttu-id="c6ce2-104">Erbt von [MobileAppIdentifier](../resources/intune_mam_mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="c6ce2-104">Inherits from [mobileAppIdentifier](../resources/intune_mam_mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c6ce2-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c6ce2-105">Properties</span></span>
|<span data-ttu-id="c6ce2-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c6ce2-106">Property</span></span>|<span data-ttu-id="c6ce2-107">Typ</span><span class="sxs-lookup"><span data-stu-id="c6ce2-107">Type</span></span>|<span data-ttu-id="c6ce2-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c6ce2-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6ce2-109">bundleId</span><span class="sxs-lookup"><span data-stu-id="c6ce2-109">bundleId</span></span>|<span data-ttu-id="c6ce2-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c6ce2-110">String</span></span>|<span data-ttu-id="c6ce2-111">Der Bezeichner für eine App wie im App-Store definiert.</span><span class="sxs-lookup"><span data-stu-id="c6ce2-111">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c6ce2-112">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c6ce2-112">Relationships</span></span>
<span data-ttu-id="c6ce2-113">Keine</span><span class="sxs-lookup"><span data-stu-id="c6ce2-113">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c6ce2-114">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c6ce2-114">JSON Representation</span></span>
<span data-ttu-id="c6ce2-115">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c6ce2-115">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosMobileAppIdentifier"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosMobileAppIdentifier",
  "bundleId": "String"
}
```



