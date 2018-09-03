# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="8a2ea-101">mediaContentRatingCanada-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8a2ea-101">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="8a2ea-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8a2ea-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8a2ea-103">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="8a2ea-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="8a2ea-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8a2ea-104">Properties</span></span>
|<span data-ttu-id="8a2ea-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8a2ea-105">Property</span></span>|<span data-ttu-id="8a2ea-106">Typ</span><span class="sxs-lookup"><span data-stu-id="8a2ea-106">Type</span></span>|<span data-ttu-id="8a2ea-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8a2ea-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a2ea-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="8a2ea-108">movieRating</span></span>|[<span data-ttu-id="8a2ea-109">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="8a2ea-109">ratingCanadaMoviesType</span></span>](../resources/intune_deviceconfig_ratingcanadamoviestype.md)|<span data-ttu-id="8a2ea-110">Für Kanada ausgewählte Filmbewertung.</span><span class="sxs-lookup"><span data-stu-id="8a2ea-110">Movies rating selected for Canada Possible values are: , , , , , , .</span></span> <span data-ttu-id="8a2ea-111">Die möglichen Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span><span class="sxs-lookup"><span data-stu-id="8a2ea-111">The possible values are `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`, , , , , or .</span></span>|
|<span data-ttu-id="8a2ea-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="8a2ea-112">tvRating</span></span>|[<span data-ttu-id="8a2ea-113">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="8a2ea-113">ratingCanadaTelevisionType</span></span>](../resources/intune_deviceconfig_ratingcanadatelevisiontype.md)|<span data-ttu-id="8a2ea-114">Für Kanada ausgewählte TV-Bewertung.</span><span class="sxs-lookup"><span data-stu-id="8a2ea-114">TV rating selected for Canada Possible values are: , , , , , , , .</span></span> <span data-ttu-id="8a2ea-115">Mögliche Werte: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="8a2ea-115">The possible values are `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, , , , or .</span></span>|

## <a name="relationships"></a><span data-ttu-id="8a2ea-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8a2ea-116">Relationships</span></span>
<span data-ttu-id="8a2ea-117">Keine</span><span class="sxs-lookup"><span data-stu-id="8a2ea-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8a2ea-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8a2ea-118">JSON Representation</span></span>
<span data-ttu-id="8a2ea-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8a2ea-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingCanada"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingCanada",
  "movieRating": "String",
  "tvRating": "String"
}
```



