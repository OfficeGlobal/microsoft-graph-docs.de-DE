# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="ae808-101">mediaContentRatingFrance-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ae808-101">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="ae808-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ae808-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ae808-103">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="ae808-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="ae808-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ae808-104">Properties</span></span>
|<span data-ttu-id="ae808-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ae808-105">Property</span></span>|<span data-ttu-id="ae808-106">Typ</span><span class="sxs-lookup"><span data-stu-id="ae808-106">Type</span></span>|<span data-ttu-id="ae808-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ae808-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae808-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="ae808-108">movieRating</span></span>|[<span data-ttu-id="ae808-109">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="ae808-109">ratingFranceMoviesType</span></span>](../resources/intune_deviceconfig_ratingfrancemoviestype.md)|<span data-ttu-id="ae808-110">Bewertung für Frankreich ausgewählten Filme.</span><span class="sxs-lookup"><span data-stu-id="ae808-110">Movies rating selected for France.</span></span> <span data-ttu-id="ae808-111">Mögliche Werte sind: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16` und `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="ae808-111">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="ae808-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="ae808-112">tvRating</span></span>|[<span data-ttu-id="ae808-113">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="ae808-113">ratingFranceTelevisionType</span></span>](../resources/intune_deviceconfig_ratingfrancetelevisiontype.md)|<span data-ttu-id="ae808-114">TV-Bewertung für Frankreich ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="ae808-114">TV rating selected for France.</span></span> <span data-ttu-id="ae808-115">Mögliche Werte sind: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16` und `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="ae808-115">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ae808-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ae808-116">Relationships</span></span>
<span data-ttu-id="ae808-117">Keine</span><span class="sxs-lookup"><span data-stu-id="ae808-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ae808-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ae808-118">JSON Representation</span></span>
<span data-ttu-id="ae808-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ae808-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingFrance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingFrance",
  "movieRating": "String",
  "tvRating": "String"
}
```



