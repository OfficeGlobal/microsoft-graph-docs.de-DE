# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="31375-101">mediaContentRatingGermany-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="31375-101">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="31375-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="31375-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="31375-103">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="31375-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="31375-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="31375-104">Properties</span></span>
|<span data-ttu-id="31375-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="31375-105">Property</span></span>|<span data-ttu-id="31375-106">Typ</span><span class="sxs-lookup"><span data-stu-id="31375-106">Type</span></span>|<span data-ttu-id="31375-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="31375-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31375-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="31375-108">movieRating</span></span>|[<span data-ttu-id="31375-109">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="31375-109">ratingGermanyMoviesType</span></span>](../resources/intune_deviceconfig_ratinggermanymoviestype.md)|<span data-ttu-id="31375-110">Bewertung für Deutschland ausgewählten Filme.</span><span class="sxs-lookup"><span data-stu-id="31375-110">Movies rating selected for Germany.</span></span> <span data-ttu-id="31375-111">Mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16` und `adults`.</span><span class="sxs-lookup"><span data-stu-id="31375-111">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="31375-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="31375-112">tvRating</span></span>|[<span data-ttu-id="31375-113">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="31375-113">ratingGermanyTelevisionType</span></span>](../resources/intune_deviceconfig_ratinggermanytelevisiontype.md)|<span data-ttu-id="31375-114">TV-Bewertung für Deutschland ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="31375-114">TV rating selected for Germany.</span></span> <span data-ttu-id="31375-115">Mögliche Werte: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="31375-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="31375-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="31375-116">Relationships</span></span>
<span data-ttu-id="31375-117">Keine</span><span class="sxs-lookup"><span data-stu-id="31375-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="31375-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="31375-118">JSON Representation</span></span>
<span data-ttu-id="31375-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="31375-119">Here is a JSON representation of the resource.</span></span>
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



