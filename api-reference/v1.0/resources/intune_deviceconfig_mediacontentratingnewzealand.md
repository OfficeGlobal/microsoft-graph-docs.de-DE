# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="77300-101">mediaContentRatingNewZealand-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="77300-101">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="77300-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="77300-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="77300-103">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="77300-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="77300-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="77300-104">Properties</span></span>
|<span data-ttu-id="77300-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="77300-105">Property</span></span>|<span data-ttu-id="77300-106">Typ</span><span class="sxs-lookup"><span data-stu-id="77300-106">Type</span></span>|<span data-ttu-id="77300-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="77300-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77300-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="77300-108">movieRating</span></span>|[<span data-ttu-id="77300-109">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="77300-109">ratingNewZealandMoviesType</span></span>](../resources/intune_deviceconfig_ratingnewzealandmoviestype.md)|<span data-ttu-id="77300-110">Film-Bewertung für Neuseeland ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="77300-110">Movies rating selected for New Zealand Possible values are: , , , , , , , , , , .</span></span> <span data-ttu-id="77300-111">Die möglichen Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span><span class="sxs-lookup"><span data-stu-id="77300-111">The possible values are `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`, or .</span></span>|
|<span data-ttu-id="77300-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="77300-112">tvRating</span></span>|[<span data-ttu-id="77300-113">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="77300-113">ratingNewZealandTelevisionType</span></span>](../resources/intune_deviceconfig_ratingnewzealandtelevisiontype.md)|<span data-ttu-id="77300-114">TV-Bewertung für Neuseeland ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="77300-114">TV rating selected for New Zealand Possible values are: , , , , .</span></span> <span data-ttu-id="77300-115">Mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="77300-115">The possible values are `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`, , , , , , , or .</span></span>|

## <a name="relationships"></a><span data-ttu-id="77300-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="77300-116">Relationships</span></span>
<span data-ttu-id="77300-117">Keine</span><span class="sxs-lookup"><span data-stu-id="77300-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="77300-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="77300-118">JSON Representation</span></span>
<span data-ttu-id="77300-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="77300-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
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



