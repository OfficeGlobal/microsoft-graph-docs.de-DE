# <a name="timezonebase-resource-type"></a><span data-ttu-id="a523f-101">timeZoneBase-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a523f-101">timeZoneBase resource type</span></span>

<span data-ttu-id="a523f-102">Die grundlegende Darstellung einer Zeitzone.</span><span class="sxs-lookup"><span data-stu-id="a523f-102">The basic representation of a time zone.</span></span>


## <a name="properties"></a><span data-ttu-id="a523f-103">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a523f-103">Properties</span></span>
| <span data-ttu-id="a523f-104">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a523f-104">Property</span></span>     | <span data-ttu-id="a523f-105">Typ</span><span class="sxs-lookup"><span data-stu-id="a523f-105">Type</span></span>   |<span data-ttu-id="a523f-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a523f-106">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a523f-107">name</span><span class="sxs-lookup"><span data-stu-id="a523f-107">name</span></span> | <span data-ttu-id="a523f-108">string</span><span class="sxs-lookup"><span data-stu-id="a523f-108">string</span></span> | <span data-ttu-id="a523f-109">Der Name einer Zeitzone.</span><span class="sxs-lookup"><span data-stu-id="a523f-109">The name of a time zone.</span></span> <span data-ttu-id="a523f-110">Dies kann ein standardmäßiger Name für eine Zeitzone sein, z. B. „Hawaii-Aleutian Normalzeit“ oder „Benutzerdefinierte Zeitzone“ für eine benutzerdefinierte Zeitzone.</span><span class="sxs-lookup"><span data-stu-id="a523f-110">It can be a standard time zone name such as "Hawaii-Aleutian Standard Time", or "Customized Time Zone" for a custom time zone.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="a523f-111">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a523f-111">JSON representation</span></span>

<span data-ttu-id="a523f-112">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a523f-112">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeZoneBase"
}-->

```json
{
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeZoneBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->