# <a name="timezoneinformation-resource-type"></a><span data-ttu-id="88c1c-101">timeZoneInformation-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="88c1c-101">timeZoneInformation resource type</span></span>


<span data-ttu-id="88c1c-102">Stellt eine Zeitzone dar.</span><span class="sxs-lookup"><span data-stu-id="88c1c-102">Represents information about a time zone.</span></span> <span data-ttu-id="88c1c-103">Das unterstützte Format ist Windows und auch das Format der [IANA-Zeitzone (Internet Assigned Numbers Authority)](http://www.iana.org/time-zones) (auch bekannt als Olson-Zeitzone) wenn das derzeitige bekannte Problem behoben ist.</span><span class="sxs-lookup"><span data-stu-id="88c1c-103">The supported format is Windows, and [Internet Assigned Numbers Authority (IANA) time zone](http://www.iana.org/time-zones) (also known as Olson time zone) format as well when the current known problem is fixed.</span></span>

## <a name="properties"></a><span data-ttu-id="88c1c-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="88c1c-104">Properties</span></span>
| <span data-ttu-id="88c1c-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="88c1c-105">Property</span></span>     | <span data-ttu-id="88c1c-106">Typ</span><span class="sxs-lookup"><span data-stu-id="88c1c-106">Type</span></span>   |<span data-ttu-id="88c1c-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="88c1c-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="88c1c-108">Alias</span><span class="sxs-lookup"><span data-stu-id="88c1c-108">alias</span></span>|<span data-ttu-id="88c1c-109">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="88c1c-109">string</span></span>|<span data-ttu-id="88c1c-110">Ein Bezeichner für die Zeitzone.</span><span class="sxs-lookup"><span data-stu-id="88c1c-110">An identifier for the time zone.</span></span>|
|<span data-ttu-id="88c1c-111">displayName</span><span class="sxs-lookup"><span data-stu-id="88c1c-111">displayName</span></span>|<span data-ttu-id="88c1c-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="88c1c-112">string</span></span>|<span data-ttu-id="88c1c-113">Eine Anzeigezeichenfolge, die die Zeitzone darstellt.</span><span class="sxs-lookup"><span data-stu-id="88c1c-113">A display string that represents the time zone.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="88c1c-114">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="88c1c-114">JSON representation</span></span>

<span data-ttu-id="88c1c-115">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="88c1c-115">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeZoneInformation"
}-->

```json
{
  "alias": "string",
  "displayName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeZoneInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->