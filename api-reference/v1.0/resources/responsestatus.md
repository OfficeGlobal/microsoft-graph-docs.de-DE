# <a name="responsestatus-resource-type"></a><span data-ttu-id="7acc0-101">responseStatus-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="7acc0-101">responseStatus resource type</span></span>

<span data-ttu-id="7acc0-102">Der Antwortstatus einer Besprechungsanfrage.</span><span class="sxs-lookup"><span data-stu-id="7acc0-102">The response status of a meeting request.</span></span>

## <a name="properties"></a><span data-ttu-id="7acc0-103">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7acc0-103">Properties</span></span>

| <span data-ttu-id="7acc0-104">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7acc0-104">Property</span></span> | <span data-ttu-id="7acc0-105">Typ</span><span class="sxs-lookup"><span data-stu-id="7acc0-105">Type</span></span>           | <span data-ttu-id="7acc0-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7acc0-106">Description</span></span> |
|:---------|:---------------|:------------|
| <span data-ttu-id="7acc0-107">Antwort</span><span class="sxs-lookup"><span data-stu-id="7acc0-107">response</span></span> | <span data-ttu-id="7acc0-108">String</span><span class="sxs-lookup"><span data-stu-id="7acc0-108">String</span></span>         | <span data-ttu-id="7acc0-109">Der Antworttyp.</span><span class="sxs-lookup"><span data-stu-id="7acc0-109">The response type.</span></span> <span data-ttu-id="7acc0-110">Mögliche Werte: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.</span><span class="sxs-lookup"><span data-stu-id="7acc0-110">Possible values are: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.</span></span>
| <span data-ttu-id="7acc0-111">Uhrzeit</span><span class="sxs-lookup"><span data-stu-id="7acc0-111">time</span></span>     | <span data-ttu-id="7acc0-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7acc0-112">DateTimeOffset</span></span> | <span data-ttu-id="7acc0-113">Datum und Uhrzeit, an dem bzw. der die Antwort zurückgegeben wurde.</span><span class="sxs-lookup"><span data-stu-id="7acc0-113">The date and time that the response was returned.</span></span> <span data-ttu-id="7acc0-114">Hierfür wird das ISO 8601-Format, und die Angabe erfolgt immer in UTC-Zeit.</span><span class="sxs-lookup"><span data-stu-id="7acc0-114">It uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7acc0-115">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="7acc0-115">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'` Read-only.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7acc0-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7acc0-116">JSON representation</span></span>

<span data-ttu-id="7acc0-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7acc0-117">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.responseStatus"
}-->

```json
{
  "response": "String",
  "time": "String (timestamp)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "responseStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
