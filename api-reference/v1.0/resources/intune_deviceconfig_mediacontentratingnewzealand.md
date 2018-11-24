# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="ddb9b-101">mediaContentRatingNewZealand-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ddb9b-101">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="ddb9b-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ddb9b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ddb9b-103">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="ddb9b-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="ddb9b-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ddb9b-104">Properties</span></span>
|<span data-ttu-id="ddb9b-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ddb9b-105">Property</span></span>|<span data-ttu-id="ddb9b-106">Typ</span><span class="sxs-lookup"><span data-stu-id="ddb9b-106">Type</span></span>|<span data-ttu-id="ddb9b-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ddb9b-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ddb9b-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="ddb9b-108">movieRating</span></span>|[<span data-ttu-id="ddb9b-109">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="ddb9b-109">ratingNewZealandMoviesType</span></span>](../resources/intune_deviceconfig_ratingnewzealandmoviestype.md)|<span data-ttu-id="ddb9b-110">Bewertung für Neuseeland ausgewählten Filme.</span><span class="sxs-lookup"><span data-stu-id="ddb9b-110">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="ddb9b-111">Mögliche Werte: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span><span class="sxs-lookup"><span data-stu-id="ddb9b-111">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="ddb9b-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="ddb9b-112">tvRating</span></span>|[<span data-ttu-id="ddb9b-113">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="ddb9b-113">ratingNewZealandTelevisionType</span></span>](../resources/intune_deviceconfig_ratingnewzealandtelevisiontype.md)|<span data-ttu-id="ddb9b-114">TV-Bewertung für Neuseeland ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="ddb9b-114">TV rating selected for New Zealand.</span></span> <span data-ttu-id="ddb9b-115">Mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance` und `adults`.</span><span class="sxs-lookup"><span data-stu-id="ddb9b-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ddb9b-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ddb9b-116">Relationships</span></span>
<span data-ttu-id="ddb9b-117">Keine</span><span class="sxs-lookup"><span data-stu-id="ddb9b-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ddb9b-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ddb9b-118">JSON Representation</span></span>
<span data-ttu-id="ddb9b-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ddb9b-119">Here is a JSON representation of the resource.</span></span>
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



