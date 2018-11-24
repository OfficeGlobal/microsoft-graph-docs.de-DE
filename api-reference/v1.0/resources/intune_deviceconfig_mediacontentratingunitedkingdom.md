# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="aa84b-101">mediaContentRatingUnitedKingdom-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="aa84b-101">mediaContentRatingUnitedKingdom resource type</span></span>

> <span data-ttu-id="aa84b-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="aa84b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aa84b-103">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="aa84b-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="aa84b-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="aa84b-104">Properties</span></span>
|<span data-ttu-id="aa84b-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="aa84b-105">Property</span></span>|<span data-ttu-id="aa84b-106">Typ</span><span class="sxs-lookup"><span data-stu-id="aa84b-106">Type</span></span>|<span data-ttu-id="aa84b-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aa84b-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa84b-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="aa84b-108">movieRating</span></span>|[<span data-ttu-id="aa84b-109">ratingUnitedKingdomMoviesType</span><span class="sxs-lookup"><span data-stu-id="aa84b-109">ratingUnitedKingdomMoviesType</span></span>](../resources/intune_deviceconfig_ratingunitedkingdommoviestype.md)|<span data-ttu-id="aa84b-110">Bewertung für Großbritannien ausgewählten Filme.</span><span class="sxs-lookup"><span data-stu-id="aa84b-110">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="aa84b-111">Mögliche Werte: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="aa84b-111">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="aa84b-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="aa84b-112">tvRating</span></span>|[<span data-ttu-id="aa84b-113">ratingUnitedKingdomTelevisionType</span><span class="sxs-lookup"><span data-stu-id="aa84b-113">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune_deviceconfig_ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="aa84b-114">TV-Bewertung für Großbritannien ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="aa84b-114">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="aa84b-115">Mögliche Werte sind: `allAllowed`, `allBlocked` und `caution`.</span><span class="sxs-lookup"><span data-stu-id="aa84b-115">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aa84b-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="aa84b-116">Relationships</span></span>
<span data-ttu-id="aa84b-117">Keine</span><span class="sxs-lookup"><span data-stu-id="aa84b-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="aa84b-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="aa84b-118">JSON Representation</span></span>
<span data-ttu-id="aa84b-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="aa84b-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedKingdom",
  "movieRating": "String",
  "tvRating": "String"
}
```



