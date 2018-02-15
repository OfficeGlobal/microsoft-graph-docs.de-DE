# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="bd16b-101">mediaContentRatingCanada-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="bd16b-101">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="bd16b-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="bd16b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bd16b-103">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="bd16b-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="bd16b-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bd16b-104">Properties</span></span>
|<span data-ttu-id="bd16b-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bd16b-105">Property</span></span>|<span data-ttu-id="bd16b-106">Typ</span><span class="sxs-lookup"><span data-stu-id="bd16b-106">Type</span></span>|<span data-ttu-id="bd16b-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bd16b-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd16b-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="bd16b-108">movieRating</span></span>|<span data-ttu-id="bd16b-109">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bd16b-109">String</span></span>|<span data-ttu-id="bd16b-110">Filmbewertungen für Kanada; mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span><span class="sxs-lookup"><span data-stu-id="bd16b-110">Movies rating selected for Canada Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="bd16b-111">tvRating</span><span class="sxs-lookup"><span data-stu-id="bd16b-111">tvRating</span></span>|<span data-ttu-id="bd16b-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bd16b-112">String</span></span>|<span data-ttu-id="bd16b-113">TV-Bewertungen für Kanada; mögliche Werte sind: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="bd16b-113">TV rating selected for Canada Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bd16b-114">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="bd16b-114">Relationships</span></span>
<span data-ttu-id="bd16b-115">Keine</span><span class="sxs-lookup"><span data-stu-id="bd16b-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bd16b-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bd16b-116">JSON Representation</span></span>
<span data-ttu-id="bd16b-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="bd16b-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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



