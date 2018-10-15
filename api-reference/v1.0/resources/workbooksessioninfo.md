# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="c4979-101">workbookSessionInfo-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c4979-101">workbookSessionInfo resource type</span></span>

<span data-ttu-id="c4979-102">Enthält Informationen zu Arbeitsmappensitzungen.</span><span class="sxs-lookup"><span data-stu-id="c4979-102">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="c4979-103">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c4979-103">JSON representation</span></span>

<span data-ttu-id="c4979-104">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c4979-104">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.workbookSessionInfo"
}-->

```json
{
  "id": "string",
  "persistChanges": true
}
```

## <a name="properties"></a><span data-ttu-id="c4979-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c4979-105">Properties</span></span>

| <span data-ttu-id="c4979-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c4979-106">Property</span></span> | <span data-ttu-id="c4979-107">Typ</span><span class="sxs-lookup"><span data-stu-id="c4979-107">Type</span></span>  | <span data-ttu-id="c4979-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c4979-108">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="c4979-109">id</span><span class="sxs-lookup"><span data-stu-id="c4979-109">id</span></span>  | <span data-ttu-id="c4979-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c4979-110">string</span></span> | <span data-ttu-id="c4979-111">Die ID der Arbeitsmappensitzung.</span><span class="sxs-lookup"><span data-stu-id="c4979-111">Id of the workbook session.</span></span> |
| <span data-ttu-id="c4979-112">persistChanges</span><span class="sxs-lookup"><span data-stu-id="c4979-112">persistChanges</span></span> | <span data-ttu-id="c4979-113">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c4979-113">boolean</span></span> |  <span data-ttu-id="c4979-114">`true` für eine beständige Sitzung.</span><span class="sxs-lookup"><span data-stu-id="c4979-114">`true` for persistent session.</span></span> <span data-ttu-id="c4979-115">`false` für eine nicht-beständige Sitzung (Ansichtsmodus)</span><span class="sxs-lookup"><span data-stu-id="c4979-115">`false` for non-persistent session (view mode)</span></span> |

