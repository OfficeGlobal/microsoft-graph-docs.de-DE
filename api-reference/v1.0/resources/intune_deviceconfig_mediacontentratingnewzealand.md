# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="86a85-101">mediaContentRatingNewZealand-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="86a85-101">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="86a85-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="86a85-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="86a85-103">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="86a85-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="86a85-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="86a85-104">Properties</span></span>
|<span data-ttu-id="86a85-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="86a85-105">Property</span></span>|<span data-ttu-id="86a85-106">Typ</span><span class="sxs-lookup"><span data-stu-id="86a85-106">Type</span></span>|<span data-ttu-id="86a85-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="86a85-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86a85-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="86a85-108">movieRating</span></span>|<span data-ttu-id="86a85-109">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="86a85-109">String</span></span>|<span data-ttu-id="86a85-110">Filmbewertungen für Neuseeland; mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span><span class="sxs-lookup"><span data-stu-id="86a85-110">Movies rating selected for New Zealand Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="86a85-111">tvRating</span><span class="sxs-lookup"><span data-stu-id="86a85-111">tvRating</span></span>|<span data-ttu-id="86a85-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="86a85-112">String</span></span>|<span data-ttu-id="86a85-113">TV-Bewertungen für Neuseeland; mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="86a85-113">TV rating selected for New Zealand Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="86a85-114">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="86a85-114">Relationships</span></span>
<span data-ttu-id="86a85-115">Keine</span><span class="sxs-lookup"><span data-stu-id="86a85-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="86a85-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="86a85-116">JSON Representation</span></span>
<span data-ttu-id="86a85-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="86a85-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mediaContentRatingNewZealand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingNewZealand",
  "movieRating": "String",
  "tvRating": "String"
}
```



