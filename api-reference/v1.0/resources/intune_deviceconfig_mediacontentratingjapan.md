# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="23f60-101">mediaContentRatingJapan-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="23f60-101">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="23f60-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="23f60-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="23f60-103">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="23f60-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="23f60-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="23f60-104">Properties</span></span>
|<span data-ttu-id="23f60-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="23f60-105">Property</span></span>|<span data-ttu-id="23f60-106">Typ</span><span class="sxs-lookup"><span data-stu-id="23f60-106">Type</span></span>|<span data-ttu-id="23f60-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="23f60-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23f60-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="23f60-108">movieRating</span></span>|[<span data-ttu-id="23f60-109">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="23f60-109">ratingJapanMoviesType</span></span>](../resources/intune_deviceconfig_ratingjapanmoviestype.md)|<span data-ttu-id="23f60-p101">Filmbewertungen für Japan; mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="23f60-p101">Movies rating selected for Japan Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="23f60-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="23f60-112">tvRating</span></span>|[<span data-ttu-id="23f60-113">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="23f60-113">ratingJapanTelevisionType</span></span>](../resources/intune_deviceconfig_ratingjapantelevisiontype.md)|<span data-ttu-id="23f60-p102">TV-Bewertungen für Japan; mögliche Werte sind: `allAllowed`, `allBlocked`, `explicitAllowed`.</span><span class="sxs-lookup"><span data-stu-id="23f60-p102">TV rating selected for Japan Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="23f60-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="23f60-116">Relationships</span></span>
<span data-ttu-id="23f60-117">Keine</span><span class="sxs-lookup"><span data-stu-id="23f60-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="23f60-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="23f60-118">JSON Representation</span></span>
<span data-ttu-id="23f60-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="23f60-119">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingJapan"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingJapan",
  "movieRating": "String",
  "tvRating": "String"
}
```








