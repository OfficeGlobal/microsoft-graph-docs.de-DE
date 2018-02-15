# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="acce2-101">mediaContentRatingUnitedStates-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="acce2-101">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="acce2-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="acce2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="acce2-103">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="acce2-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="acce2-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="acce2-104">Properties</span></span>
|<span data-ttu-id="acce2-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="acce2-105">Property</span></span>|<span data-ttu-id="acce2-106">Typ</span><span class="sxs-lookup"><span data-stu-id="acce2-106">Type</span></span>|<span data-ttu-id="acce2-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="acce2-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="acce2-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="acce2-108">movieRating</span></span>|<span data-ttu-id="acce2-109">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="acce2-109">String</span></span>|<span data-ttu-id="acce2-110">Filmbewertungen für die Vereinigten Staaten; mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="acce2-110">Movies rating selected for United States Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="acce2-111">tvRating</span><span class="sxs-lookup"><span data-stu-id="acce2-111">tvRating</span></span>|<span data-ttu-id="acce2-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="acce2-112">String</span></span>|<span data-ttu-id="acce2-113">TV-Bewertungen für die Vereinigten Staaten; mögliche Werte sind: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="acce2-113">TV rating selected for United States Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="acce2-114">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="acce2-114">Relationships</span></span>
<span data-ttu-id="acce2-115">Keine</span><span class="sxs-lookup"><span data-stu-id="acce2-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="acce2-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="acce2-116">JSON Representation</span></span>
<span data-ttu-id="acce2-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="acce2-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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



