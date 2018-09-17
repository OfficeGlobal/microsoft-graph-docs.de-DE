# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="20fa3-101">mediaContentRatingUnitedStates-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="20fa3-101">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="20fa3-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="20fa3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="20fa3-103">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="20fa3-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="20fa3-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="20fa3-104">Properties</span></span>
|<span data-ttu-id="20fa3-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="20fa3-105">Property</span></span>|<span data-ttu-id="20fa3-106">Typ</span><span class="sxs-lookup"><span data-stu-id="20fa3-106">Type</span></span>|<span data-ttu-id="20fa3-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="20fa3-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20fa3-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="20fa3-108">movieRating</span></span>|[<span data-ttu-id="20fa3-109">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="20fa3-109">ratingUnitedStatesMoviesType</span></span>](../resources/intune_deviceconfig_ratingunitedstatesmoviestype.md)|<span data-ttu-id="20fa3-p101">Ausgewählte Filmbewertung für die Vereinigten Staaten. Mögliche Werte: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="20fa3-p101">Movies rating selected for United States Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="20fa3-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="20fa3-112">tvRating</span></span>|[<span data-ttu-id="20fa3-113">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="20fa3-113">ratingUnitedStatesTelevisionType</span></span>](../resources/intune_deviceconfig_ratingunitedstatestelevisiontype.md)|<span data-ttu-id="20fa3-p102">Ausgewählte TV-Bewertung für die Vereinigten Staaten. Mögliche Werte: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="20fa3-p102">TV rating selected for United States Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="20fa3-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="20fa3-116">Relationships</span></span>
<span data-ttu-id="20fa3-117">Keine</span><span class="sxs-lookup"><span data-stu-id="20fa3-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="20fa3-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="20fa3-118">JSON Representation</span></span>
<span data-ttu-id="20fa3-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="20fa3-119">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedStates",
  "movieRating": "String",
  "tvRating": "String"
}
```








