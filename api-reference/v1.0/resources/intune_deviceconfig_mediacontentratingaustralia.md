# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="64e05-101">mediaContentRatingAustralia-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="64e05-101">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="64e05-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="64e05-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="64e05-103">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="64e05-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="64e05-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="64e05-104">Properties</span></span>
|<span data-ttu-id="64e05-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="64e05-105">Property</span></span>|<span data-ttu-id="64e05-106">Typ</span><span class="sxs-lookup"><span data-stu-id="64e05-106">Type</span></span>|<span data-ttu-id="64e05-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="64e05-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64e05-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="64e05-108">movieRating</span></span>|<span data-ttu-id="64e05-109">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="64e05-109">String</span></span>|<span data-ttu-id="64e05-110">Filmbewertungen für Australien; mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="64e05-110">Movies rating selected for Australia Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="64e05-111">tvRating</span><span class="sxs-lookup"><span data-stu-id="64e05-111">tvRating</span></span>|<span data-ttu-id="64e05-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="64e05-112">String</span></span>|<span data-ttu-id="64e05-113">TV-Bewertungen für Australien; mögliche Werte sind: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="64e05-113">TV rating selected for Australia Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="64e05-114">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="64e05-114">Relationships</span></span>
<span data-ttu-id="64e05-115">Keine</span><span class="sxs-lookup"><span data-stu-id="64e05-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="64e05-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="64e05-116">JSON Representation</span></span>
<span data-ttu-id="64e05-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="64e05-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mediaContentRatingAustralia"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingAustralia",
  "movieRating": "String",
  "tvRating": "String"
}
```



