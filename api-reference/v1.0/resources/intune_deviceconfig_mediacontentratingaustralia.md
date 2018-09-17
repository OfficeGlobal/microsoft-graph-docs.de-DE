# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="d8944-101">mediaContentRatingAustralia-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d8944-101">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="d8944-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d8944-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d8944-103">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="d8944-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="d8944-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d8944-104">Properties</span></span>
|<span data-ttu-id="d8944-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d8944-105">Property</span></span>|<span data-ttu-id="d8944-106">Typ</span><span class="sxs-lookup"><span data-stu-id="d8944-106">Type</span></span>|<span data-ttu-id="d8944-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d8944-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8944-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="d8944-108">movieRating</span></span>|[<span data-ttu-id="d8944-109">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="d8944-109">ratingAustraliaMoviesType</span></span>](../resources/intune_deviceconfig_ratingaustraliamoviestype.md)|<span data-ttu-id="d8944-p101">Filmbewertungen für Australien; mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="d8944-p101">Movies rating selected for Australia Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="d8944-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="d8944-112">tvRating</span></span>|[<span data-ttu-id="d8944-113">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="d8944-113">ratingAustraliaTelevisionType</span></span>](../resources/intune_deviceconfig_ratingaustraliatelevisiontype.md)|<span data-ttu-id="d8944-p102">TV-Bewertungen für Australien; mögliche Werte sind: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="d8944-p102">TV rating selected for Australia Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d8944-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d8944-116">Relationships</span></span>
<span data-ttu-id="d8944-117">Keine</span><span class="sxs-lookup"><span data-stu-id="d8944-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d8944-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d8944-118">JSON Representation</span></span>
<span data-ttu-id="d8944-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d8944-119">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingAustralia"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingAustralia",
  "movieRating": "String",
  "tvRating": "String"
}
```








