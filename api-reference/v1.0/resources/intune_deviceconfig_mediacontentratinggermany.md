# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="54f15-101">mediaContentRatingGermany-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="54f15-101">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="54f15-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="54f15-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="54f15-103">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="54f15-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="54f15-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="54f15-104">Properties</span></span>
|<span data-ttu-id="54f15-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="54f15-105">Property</span></span>|<span data-ttu-id="54f15-106">Typ</span><span class="sxs-lookup"><span data-stu-id="54f15-106">Type</span></span>|<span data-ttu-id="54f15-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="54f15-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54f15-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="54f15-108">movieRating</span></span>|[<span data-ttu-id="54f15-109">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="54f15-109">ratingGermanyMoviesType</span></span>](../resources/intune_deviceconfig_ratinggermanymoviestype.md)|<span data-ttu-id="54f15-110">Film-Bewertung für Deutschland ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="54f15-110">Movies rating selected for Germany Possible values are: , , , , , , .</span></span> <span data-ttu-id="54f15-111">Die möglichen Werte sind: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="54f15-111">The possible values are `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`, , , , , or .</span></span>|
|<span data-ttu-id="54f15-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="54f15-112">tvRating</span></span>|[<span data-ttu-id="54f15-113">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="54f15-113">ratingGermanyTelevisionType</span></span>](../resources/intune_deviceconfig_ratinggermanytelevisiontype.md)|<span data-ttu-id="54f15-114">TV-Bewertung für Deutschland ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="54f15-114">TV rating selected for Germany Possible values are: , , , , , , .</span></span> <span data-ttu-id="54f15-115">Die möglichen Werte sind: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="54f15-115">The possible values are `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`, , , , , or .</span></span>|

## <a name="relationships"></a><span data-ttu-id="54f15-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="54f15-116">Relationships</span></span>
<span data-ttu-id="54f15-117">Keine</span><span class="sxs-lookup"><span data-stu-id="54f15-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="54f15-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="54f15-118">JSON Representation</span></span>
<span data-ttu-id="54f15-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="54f15-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingGermany"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingGermany",
  "movieRating": "String",
  "tvRating": "String"
}
```



