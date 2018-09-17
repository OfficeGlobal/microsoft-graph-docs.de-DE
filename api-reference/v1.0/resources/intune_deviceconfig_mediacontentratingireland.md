# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="4de77-101">mediaContentRatingIreland-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="4de77-101">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="4de77-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4de77-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4de77-103">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="4de77-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="4de77-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4de77-104">Properties</span></span>
|<span data-ttu-id="4de77-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4de77-105">Property</span></span>|<span data-ttu-id="4de77-106">Typ</span><span class="sxs-lookup"><span data-stu-id="4de77-106">Type</span></span>|<span data-ttu-id="4de77-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4de77-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4de77-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="4de77-108">movieRating</span></span>|[<span data-ttu-id="4de77-109">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="4de77-109">ratingIrelandMoviesType</span></span>](../resources/intune_deviceconfig_ratingirelandmoviestype.md)|<span data-ttu-id="4de77-110">Filmbewertung für Irland.</span><span class="sxs-lookup"><span data-stu-id="4de77-110">Movies rating selected for Ireland Possible values are: , , , , , , , .</span></span> <span data-ttu-id="4de77-111">Mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16` und `adults`.</span><span class="sxs-lookup"><span data-stu-id="4de77-111">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="4de77-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="4de77-112">tvRating</span></span>|[<span data-ttu-id="4de77-113">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="4de77-113">ratingIrelandTelevisionType</span></span>](../resources/intune_deviceconfig_ratingirelandtelevisiontype.md)|<span data-ttu-id="4de77-114">TV-Bewertung für Irland.</span><span class="sxs-lookup"><span data-stu-id="4de77-114">TV rating selected for Ireland Possible values are: , , , , , , .</span></span> <span data-ttu-id="4de77-115">Mögliche Werte: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span><span class="sxs-lookup"><span data-stu-id="4de77-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4de77-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="4de77-116">Relationships</span></span>
<span data-ttu-id="4de77-117">Keine</span><span class="sxs-lookup"><span data-stu-id="4de77-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4de77-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4de77-118">JSON Representation</span></span>
<span data-ttu-id="4de77-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4de77-119">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingIreland"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingIreland",
  "movieRating": "String",
  "tvRating": "String"
}
```








