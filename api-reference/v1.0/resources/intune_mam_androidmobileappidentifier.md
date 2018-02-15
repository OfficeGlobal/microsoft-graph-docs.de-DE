# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="60370-101">androidMobileAppIdentifier-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="60370-101">androidMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="60370-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="60370-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="60370-103">Der Bezeichner für eine Android-App.</span><span class="sxs-lookup"><span data-stu-id="60370-103">The identifier for an Android app.</span></span>

<span data-ttu-id="60370-104">Erbt von [mobileAppIdentifier](../resources/intune_mam_mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="60370-104">Inherits from [mobileAppIdentifier](../resources/intune_mam_mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="60370-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="60370-105">Properties</span></span>
|<span data-ttu-id="60370-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="60370-106">Property</span></span>|<span data-ttu-id="60370-107">Typ</span><span class="sxs-lookup"><span data-stu-id="60370-107">Type</span></span>|<span data-ttu-id="60370-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="60370-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60370-109">packageId</span><span class="sxs-lookup"><span data-stu-id="60370-109">packageId</span></span>|<span data-ttu-id="60370-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="60370-110">String</span></span>|<span data-ttu-id="60370-111">Der Bezeichner für eine App wie im Play Store definiert.</span><span class="sxs-lookup"><span data-stu-id="60370-111">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="60370-112">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="60370-112">Relationships</span></span>
<span data-ttu-id="60370-113">Keine</span><span class="sxs-lookup"><span data-stu-id="60370-113">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="60370-114">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="60370-114">JSON Representation</span></span>
<span data-ttu-id="60370-115">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="60370-115">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidMobileAppIdentifier"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidMobileAppIdentifier",
  "packageId": "String"
}
```



