# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="66bdb-101">mediaContentRatingJapan-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="66bdb-101">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="66bdb-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="66bdb-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="66bdb-103">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="66bdb-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="66bdb-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="66bdb-104">Properties</span></span>
|<span data-ttu-id="66bdb-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="66bdb-105">Property</span></span>|<span data-ttu-id="66bdb-106">Typ</span><span class="sxs-lookup"><span data-stu-id="66bdb-106">Type</span></span>|<span data-ttu-id="66bdb-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="66bdb-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66bdb-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="66bdb-108">movieRating</span></span>|<span data-ttu-id="66bdb-109">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="66bdb-109">String</span></span>|<span data-ttu-id="66bdb-110">Filmbewertungen für Japan; mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="66bdb-110">Movies rating selected for Japan Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="66bdb-111">tvRating</span><span class="sxs-lookup"><span data-stu-id="66bdb-111">tvRating</span></span>|<span data-ttu-id="66bdb-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="66bdb-112">String</span></span>|<span data-ttu-id="66bdb-113">TV-Bewertungen für Japan; mögliche Werte sind: `allAllowed`, `allBlocked`, `explicitAllowed`.</span><span class="sxs-lookup"><span data-stu-id="66bdb-113">TV rating selected for Japan Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="66bdb-114">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="66bdb-114">Relationships</span></span>
<span data-ttu-id="66bdb-115">Keine</span><span class="sxs-lookup"><span data-stu-id="66bdb-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="66bdb-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="66bdb-116">JSON Representation</span></span>
<span data-ttu-id="66bdb-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="66bdb-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mediaContentRatingJapan"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingJapan",
  "movieRating": "String",
  "tvRating": "String"
}
```



