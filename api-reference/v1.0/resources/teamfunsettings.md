# <a name="teamfunsettings-resource-type"></a><span data-ttu-id="e05cf-101">Ressourcentyp teamFunSettings</span><span class="sxs-lookup"><span data-stu-id="e05cf-101">teamFunSettings resource type</span></span>



<span data-ttu-id="e05cf-102">Einstellungen zum Konfigurieren der Verwendung von Giphy, Memes und Aufkleber in das [Team](team.md).</span><span class="sxs-lookup"><span data-stu-id="e05cf-102">Settings to configure use of Giphy, memes, and stickers in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e05cf-103">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e05cf-103">Properties</span></span>
| <span data-ttu-id="e05cf-104">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e05cf-104">Property</span></span>     | <span data-ttu-id="e05cf-105">Typ</span><span class="sxs-lookup"><span data-stu-id="e05cf-105">Type</span></span>   |<span data-ttu-id="e05cf-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e05cf-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e05cf-107">allowGiphy</span><span class="sxs-lookup"><span data-stu-id="e05cf-107">allowGiphy</span></span>|<span data-ttu-id="e05cf-108">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e05cf-108">Boolean</span></span>|<span data-ttu-id="e05cf-109">Wenn auf "true" ermöglicht Giphy Verwendung festgelegt.</span><span class="sxs-lookup"><span data-stu-id="e05cf-109">If set to true, enables Giphy use.</span></span>|
|<span data-ttu-id="e05cf-110">giphyContentRating</span><span class="sxs-lookup"><span data-stu-id="e05cf-110">giphyContentRating</span></span>|<span data-ttu-id="e05cf-111">Zeichenfolge (Aufzählung)</span><span class="sxs-lookup"><span data-stu-id="e05cf-111">String (enum)</span></span>|<span data-ttu-id="e05cf-112">Giphy bewerten.</span><span class="sxs-lookup"><span data-stu-id="e05cf-112">Giphy content rating.</span></span> <span data-ttu-id="e05cf-113">Mögliche Werte sind: `moderate` und `strict`.</span><span class="sxs-lookup"><span data-stu-id="e05cf-113">Possible values are: `moderate`, `strict`.</span></span>|
|<span data-ttu-id="e05cf-114">allowStickersAndMemes</span><span class="sxs-lookup"><span data-stu-id="e05cf-114">allowStickersAndMemes</span></span>|<span data-ttu-id="e05cf-115">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e05cf-115">Boolean</span></span>|<span data-ttu-id="e05cf-116">Wenn Festlegung auf "true" ermöglicht Benutzern das Aufkleber und Memes enthalten.</span><span class="sxs-lookup"><span data-stu-id="e05cf-116">If set to true, enables users to include stickers and memes.</span></span>|
|<span data-ttu-id="e05cf-117">allowCustomMemes</span><span class="sxs-lookup"><span data-stu-id="e05cf-117">allowCustomMemes</span></span>|<span data-ttu-id="e05cf-118">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e05cf-118">Boolean</span></span>|<span data-ttu-id="e05cf-119">Wenn auf "true" ermöglicht Benutzern das Einschließen von benutzerdefinierten Memes festgelegt.</span><span class="sxs-lookup"><span data-stu-id="e05cf-119">If set to true, enables users to include custom memes.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e05cf-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e05cf-120">JSON representation</span></span>

<span data-ttu-id="e05cf-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e05cf-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamFunSettings"
}-->

```json
{
  "allowGiphy": true,
  "giphyContentRating": "strict",
  "allowStickersAndMemes": true,
  "allowCustomMemes": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's funSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
