# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="40845-101">mediaContentRatingAustralia-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="40845-101">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="40845-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="40845-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="40845-103">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="40845-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="40845-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="40845-104">Properties</span></span>
|<span data-ttu-id="40845-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="40845-105">Property</span></span>|<span data-ttu-id="40845-106">Typ</span><span class="sxs-lookup"><span data-stu-id="40845-106">Type</span></span>|<span data-ttu-id="40845-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="40845-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40845-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="40845-108">movieRating</span></span>|[<span data-ttu-id="40845-109">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="40845-109">ratingAustraliaMoviesType</span></span>](../resources/intune_deviceconfig_ratingaustraliamoviestype.md)|<span data-ttu-id="40845-110">Bewertung für Australien ausgewählter Filme.</span><span class="sxs-lookup"><span data-stu-id="40845-110">Movies rating selected for Australia Possible values are: , , , , , , .</span></span> <span data-ttu-id="40845-111">Mögliche Werte: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="40845-111">The possible values are `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`, , , , , or .</span></span>|
|<span data-ttu-id="40845-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="40845-112">tvRating</span></span>|[<span data-ttu-id="40845-113">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="40845-113">ratingAustraliaTelevisionType</span></span>](../resources/intune_deviceconfig_ratingaustraliatelevisiontype.md)|<span data-ttu-id="40845-114">Bewertung für Australien ausgewählter TV-Sendungen.</span><span class="sxs-lookup"><span data-stu-id="40845-114">TV rating selected for Australia Possible values are: , , , , , , , , .</span></span> <span data-ttu-id="40845-115">Mögliche Werte: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="40845-115">The possible values are `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`, , , or .</span></span>|

## <a name="relationships"></a><span data-ttu-id="40845-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="40845-116">Relationships</span></span>
<span data-ttu-id="40845-117">Keine</span><span class="sxs-lookup"><span data-stu-id="40845-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="40845-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="40845-118">JSON Representation</span></span>
<span data-ttu-id="40845-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="40845-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingAustralia"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingAustralia",
  "movieRating": "String",
  "tvRating": "String"
}
```



