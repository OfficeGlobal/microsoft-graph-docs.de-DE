# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="c5581-101">mediaContentRatingFrance-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c5581-101">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="c5581-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c5581-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c5581-103">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="c5581-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="c5581-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c5581-104">Properties</span></span>
|<span data-ttu-id="c5581-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c5581-105">Property</span></span>|<span data-ttu-id="c5581-106">Typ</span><span class="sxs-lookup"><span data-stu-id="c5581-106">Type</span></span>|<span data-ttu-id="c5581-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c5581-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5581-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="c5581-108">movieRating</span></span>|<span data-ttu-id="c5581-109">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c5581-109">String</span></span>|<span data-ttu-id="c5581-110">Filmbewertungen für Frankreich; mögliche Werte sind: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="c5581-110">Movies rating selected for France Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="c5581-111">tvRating</span><span class="sxs-lookup"><span data-stu-id="c5581-111">tvRating</span></span>|<span data-ttu-id="c5581-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c5581-112">String</span></span>|<span data-ttu-id="c5581-113">TV-Bewertungen für Frankreich; mögliche Werte sind: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="c5581-113">TV rating selected for France Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c5581-114">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c5581-114">Relationships</span></span>
<span data-ttu-id="c5581-115">Keine</span><span class="sxs-lookup"><span data-stu-id="c5581-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c5581-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c5581-116">JSON Representation</span></span>
<span data-ttu-id="c5581-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c5581-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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



