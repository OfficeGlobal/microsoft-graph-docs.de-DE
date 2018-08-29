# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="476a0-101">mediaContentRatingUnitedStates-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="476a0-101">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="476a0-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="476a0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="476a0-103">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="476a0-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="476a0-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="476a0-104">Properties</span></span>
|<span data-ttu-id="476a0-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="476a0-105">Property</span></span>|<span data-ttu-id="476a0-106">Typ</span><span class="sxs-lookup"><span data-stu-id="476a0-106">Type</span></span>|<span data-ttu-id="476a0-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="476a0-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="476a0-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="476a0-108">movieRating</span></span>|[<span data-ttu-id="476a0-109">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="476a0-109">ratingUnitedStatesMoviesType</span></span>](../resources/intune_deviceconfig_ratingunitedstatesmoviestype.md)|<span data-ttu-id="476a0-110">Bewertung von Filmen ausgewählt für USA.</span><span class="sxs-lookup"><span data-stu-id="476a0-110">Movies rating selected for United States Possible values are: , , , , , , .</span></span> <span data-ttu-id="476a0-111">Mögliche Werte: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="476a0-111">The possible values are `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`, , , , , or .</span></span>|
|<span data-ttu-id="476a0-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="476a0-112">tvRating</span></span>|[<span data-ttu-id="476a0-113">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="476a0-113">ratingUnitedStatesTelevisionType</span></span>](../resources/intune_deviceconfig_ratingunitedstatestelevisiontype.md)|<span data-ttu-id="476a0-114">TV-Bewertung ausgewählt für USA.</span><span class="sxs-lookup"><span data-stu-id="476a0-114">TV rating selected for United States Possible values are: , , , , , , , .</span></span> <span data-ttu-id="476a0-115">Mögliche Werte: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="476a0-115">The possible values are `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`, , , , or .</span></span>|

## <a name="relationships"></a><span data-ttu-id="476a0-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="476a0-116">Relationships</span></span>
<span data-ttu-id="476a0-117">Keine</span><span class="sxs-lookup"><span data-stu-id="476a0-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="476a0-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="476a0-118">JSON Representation</span></span>
<span data-ttu-id="476a0-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="476a0-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedStates",
  "movieRating": "String",
  "tvRating": "String"
}
```



