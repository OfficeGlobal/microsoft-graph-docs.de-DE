# <a name="alternativesecurityid-resource-type"></a><span data-ttu-id="f1346-101">alternativeSecurityId-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f1346-101">alternativeSecurityId resource type</span></span>

<span data-ttu-id="f1346-p101">Enthält eine alternative Sicherheits-ID, die mit einem Gerät verknüpft ist. Die **alternativeSecurityIds**-Eigenschaft der [Device](device.md)-Entität ist eine Sammlung von **alternativeSecurityId**.</span><span class="sxs-lookup"><span data-stu-id="f1346-p101">Contains an alternative security ID associated with a device. The **alternativeSecurityIds** property of the [Device](device.md) entity is a collection of **alternativeSecurityId**.</span></span>

## <a name="properties"></a><span data-ttu-id="f1346-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f1346-104">Properties</span></span>
| <span data-ttu-id="f1346-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f1346-105">Property</span></span>     | <span data-ttu-id="f1346-106">Typ</span><span class="sxs-lookup"><span data-stu-id="f1346-106">Type</span></span>   |<span data-ttu-id="f1346-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f1346-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f1346-108">identityProvider</span><span class="sxs-lookup"><span data-stu-id="f1346-108">identityProvider</span></span>|<span data-ttu-id="f1346-109">String</span><span class="sxs-lookup"><span data-stu-id="f1346-109">String</span></span>|            |
|<span data-ttu-id="f1346-110">Key</span><span class="sxs-lookup"><span data-stu-id="f1346-110">key</span></span>|<span data-ttu-id="f1346-111">Binär</span><span class="sxs-lookup"><span data-stu-id="f1346-111">Binary</span></span>|            |
|<span data-ttu-id="f1346-112">Typ</span><span class="sxs-lookup"><span data-stu-id="f1346-112">type</span></span>|<span data-ttu-id="f1346-113">Int32</span><span class="sxs-lookup"><span data-stu-id="f1346-113">Int32</span></span>|            |

## <a name="json-representation"></a><span data-ttu-id="f1346-114">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f1346-114">JSON representation</span></span>

<span data-ttu-id="f1346-115">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f1346-115">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.alternativeSecurityId"
}-->

```json
{
  "identityProvider": "string",
  "key": "binary",
  "type": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alternativeSecurityId resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
