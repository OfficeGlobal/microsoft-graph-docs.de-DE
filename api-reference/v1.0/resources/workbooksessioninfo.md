# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="0fc6f-101">workbookSessionInfo-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0fc6f-101">workbookSessionInfo resource type</span></span>

<span data-ttu-id="0fc6f-102">Enthält Informationen zu Arbeitsmappensitzungen.</span><span class="sxs-lookup"><span data-stu-id="0fc6f-102">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="0fc6f-103">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0fc6f-103">JSON representation</span></span>

<span data-ttu-id="0fc6f-104">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0fc6f-104">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="0fc6f-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0fc6f-105">Properties</span></span>

| <span data-ttu-id="0fc6f-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0fc6f-106">Property</span></span> | <span data-ttu-id="0fc6f-107">Typ</span><span class="sxs-lookup"><span data-stu-id="0fc6f-107">Type</span></span>  | <span data-ttu-id="0fc6f-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0fc6f-108">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="0fc6f-109">id</span><span class="sxs-lookup"><span data-stu-id="0fc6f-109">id</span></span>  | <span data-ttu-id="0fc6f-110">string</span><span class="sxs-lookup"><span data-stu-id="0fc6f-110">string</span></span> | <span data-ttu-id="0fc6f-111">Die ID der Arbeitsmappensitzung.</span><span class="sxs-lookup"><span data-stu-id="0fc6f-111">Id of the workbook session.</span></span> |
| <span data-ttu-id="0fc6f-112">persistChanges</span><span class="sxs-lookup"><span data-stu-id="0fc6f-112">persistChanges</span></span> | <span data-ttu-id="0fc6f-113">string</span><span class="sxs-lookup"><span data-stu-id="0fc6f-113">string</span></span> |  <span data-ttu-id="0fc6f-114">`true` für eine beständige Sitzung</span><span class="sxs-lookup"><span data-stu-id="0fc6f-114">`true` for persistent session.</span></span> <span data-ttu-id="0fc6f-115">`false` für eine nicht-beständige Sitzung (Ansichtsmodus)</span><span class="sxs-lookup"><span data-stu-id="0fc6f-115">`false` for non-persistent session (view mode)</span></span> |

