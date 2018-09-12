# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="6d593-101">mediaContentRatingNewZealand-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6d593-101">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="6d593-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6d593-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6d593-103">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="6d593-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="6d593-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6d593-104">Properties</span></span>
|<span data-ttu-id="6d593-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6d593-105">Property</span></span>|<span data-ttu-id="6d593-106">Typ</span><span class="sxs-lookup"><span data-stu-id="6d593-106">Type</span></span>|<span data-ttu-id="6d593-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6d593-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d593-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="6d593-108">movieRating</span></span>|[<span data-ttu-id="6d593-109">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="6d593-109">ratingNewZealandMoviesType</span></span>](../resources/intune_deviceconfig_ratingnewzealandmoviestype.md)|<span data-ttu-id="6d593-p101">Filmbewertungen für Neuseeeland. Mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span><span class="sxs-lookup"><span data-stu-id="6d593-p101">Movies rating selected for New Zealand Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="6d593-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="6d593-112">tvRating</span></span>|[<span data-ttu-id="6d593-113">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="6d593-113">ratingNewZealandTelevisionType</span></span>](../resources/intune_deviceconfig_ratingnewzealandtelevisiontype.md)|<span data-ttu-id="6d593-p102">TV-Bewertungen für Neuseeland. Mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="6d593-p102">TV rating selected for New Zealand Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6d593-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6d593-116">Relationships</span></span>
<span data-ttu-id="6d593-117">Keine</span><span class="sxs-lookup"><span data-stu-id="6d593-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6d593-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6d593-118">JSON Representation</span></span>
<span data-ttu-id="6d593-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6d593-119">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingNewZealand"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingNewZealand",
  "movieRating": "String",
  "tvRating": "String"
}
```








