# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="11df4-101">mediaContentRatingGermany-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="11df4-101">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="11df4-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="11df4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="11df4-103">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="11df4-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="11df4-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="11df4-104">Properties</span></span>
|<span data-ttu-id="11df4-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="11df4-105">Property</span></span>|<span data-ttu-id="11df4-106">Typ</span><span class="sxs-lookup"><span data-stu-id="11df4-106">Type</span></span>|<span data-ttu-id="11df4-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="11df4-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11df4-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="11df4-108">movieRating</span></span>|<span data-ttu-id="11df4-109">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="11df4-109">String</span></span>|<span data-ttu-id="11df4-110">Filmbewertungen für Deutschland; mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="11df4-110">Movies rating selected for Germany Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="11df4-111">tvRating</span><span class="sxs-lookup"><span data-stu-id="11df4-111">tvRating</span></span>|<span data-ttu-id="11df4-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="11df4-112">String</span></span>|<span data-ttu-id="11df4-113">TV-Bewertungen für Deutschland; mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="11df4-113">TV rating selected for Germany Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="11df4-114">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="11df4-114">Relationships</span></span>
<span data-ttu-id="11df4-115">Keine</span><span class="sxs-lookup"><span data-stu-id="11df4-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="11df4-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="11df4-116">JSON Representation</span></span>
<span data-ttu-id="11df4-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="11df4-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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



