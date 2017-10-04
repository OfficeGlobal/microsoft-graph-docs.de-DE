# <a name="recentnotebooklinks-resource-type"></a><span data-ttu-id="fd73c-101">recentNotebookLinks-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="fd73c-101">recentNotebookLinks resource type</span></span>

<span data-ttu-id="fd73c-102">Links zum Öffnen eines OneNote-Notizbuchs.</span><span class="sxs-lookup"><span data-stu-id="fd73c-102">Links for opening a OneNote notebook.</span></span> <span data-ttu-id="fd73c-103">Dieser Ressourcentyp ist als Eigenschaft für eine [recentNotebook](recentnotebook.md)-Ressource vorhanden.</span><span class="sxs-lookup"><span data-stu-id="fd73c-103">This resource type exists as a property on a [recentNotebook](recentnotebook.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="fd73c-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="fd73c-104">Properties</span></span>
| <span data-ttu-id="fd73c-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fd73c-105">Property</span></span>     | <span data-ttu-id="fd73c-106">Typ</span><span class="sxs-lookup"><span data-stu-id="fd73c-106">Type</span></span>   |<span data-ttu-id="fd73c-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fd73c-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fd73c-108">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="fd73c-108">oneNoteClientUrl</span></span>|[<span data-ttu-id="fd73c-109">externalLink</span><span class="sxs-lookup"><span data-stu-id="fd73c-109">externalLink</span></span>](externallink.md)|<span data-ttu-id="fd73c-110">Öffnet das Notizbuch im systemeigenen OneNote-Client, sofern er installiert ist.</span><span class="sxs-lookup"><span data-stu-id="fd73c-110">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="fd73c-111">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="fd73c-111">oneNoteWebUrl</span></span>|[<span data-ttu-id="fd73c-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="fd73c-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="fd73c-113">Öffnet das Notizbuch in OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="fd73c-113">Opens the notebook in OneNote Online.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fd73c-114">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="fd73c-114">JSON representation</span></span>

<span data-ttu-id="fd73c-115">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="fd73c-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recentNotebookLinks"
}-->

```json
{
  "oneNoteClientUrl": {"@odata.type": "microsoft.graph.externalLink"},
  "oneNoteWebUrl": {"@odata.type": "microsoft.graph.externalLink"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recentNotebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
