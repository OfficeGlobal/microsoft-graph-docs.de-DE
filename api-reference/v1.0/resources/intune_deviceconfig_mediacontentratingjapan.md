# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="ca0d8-101">mediaContentRatingJapan-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ca0d8-101">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="ca0d8-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ca0d8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ca0d8-103">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="ca0d8-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="ca0d8-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ca0d8-104">Properties</span></span>
|<span data-ttu-id="ca0d8-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ca0d8-105">Property</span></span>|<span data-ttu-id="ca0d8-106">Typ</span><span class="sxs-lookup"><span data-stu-id="ca0d8-106">Type</span></span>|<span data-ttu-id="ca0d8-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ca0d8-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca0d8-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="ca0d8-108">movieRating</span></span>|[<span data-ttu-id="ca0d8-109">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="ca0d8-109">ratingJapanMoviesType</span></span>](../resources/intune_deviceconfig_ratingjapanmoviestype.md)|<span data-ttu-id="ca0d8-110">Bewertung für Japan ausgewählter Filme.</span><span class="sxs-lookup"><span data-stu-id="ca0d8-110">Movies rating selected for Japan Possible values are: , , , , , .</span></span> <span data-ttu-id="ca0d8-111">Mögliche Werte: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="ca0d8-111">The possible values are `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`, , , , , , or .</span></span>|
|<span data-ttu-id="ca0d8-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="ca0d8-112">tvRating</span></span>|[<span data-ttu-id="ca0d8-113">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="ca0d8-113">ratingJapanTelevisionType</span></span>](../resources/intune_deviceconfig_ratingjapantelevisiontype.md)|<span data-ttu-id="ca0d8-114">Bewertung für Japan ausgewählter TV-Sendungen.</span><span class="sxs-lookup"><span data-stu-id="ca0d8-114">TV rating selected for Japan Possible values are: , , .</span></span> <span data-ttu-id="ca0d8-115">Mögliche Werte sind:`allAllowed`, `allBlocked`, `explicitAllowed`.</span><span class="sxs-lookup"><span data-stu-id="ca0d8-115">The possible values are `allAllowed`, `allBlocked`, `explicitAllowed`, , , , , , , , , or .</span></span>|

## <a name="relationships"></a><span data-ttu-id="ca0d8-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ca0d8-116">Relationships</span></span>
<span data-ttu-id="ca0d8-117">Keine</span><span class="sxs-lookup"><span data-stu-id="ca0d8-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ca0d8-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ca0d8-118">JSON Representation</span></span>
<span data-ttu-id="ca0d8-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ca0d8-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingJapan"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingJapan",
  "movieRating": "String",
  "tvRating": "String"
}
```



