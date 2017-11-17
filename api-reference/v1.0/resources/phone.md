# <a name="phone-resource-type"></a><span data-ttu-id="08334-101">phone-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="08334-101">phone resource type</span></span>

<span data-ttu-id="08334-102">Gibt eine Telefonnummer an.</span><span class="sxs-lookup"><span data-stu-id="08334-102">Represents a phone number identified in an item.</span></span>


## <a name="properties"></a><span data-ttu-id="08334-103">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="08334-103">Properties</span></span>
| <span data-ttu-id="08334-104">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="08334-104">Property</span></span>     | <span data-ttu-id="08334-105">Typ</span><span class="sxs-lookup"><span data-stu-id="08334-105">Type</span></span>   |<span data-ttu-id="08334-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="08334-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="08334-107">number</span><span class="sxs-lookup"><span data-stu-id="08334-107">number</span></span>|<span data-ttu-id="08334-108">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="08334-108">string</span></span>|<span data-ttu-id="08334-109">Die Telefonnummer</span><span class="sxs-lookup"><span data-stu-id="08334-109">The contact's mobile phone number.</span></span>|
|<span data-ttu-id="08334-110">type</span><span class="sxs-lookup"><span data-stu-id="08334-110">type</span></span>|<span data-ttu-id="08334-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="08334-111">String</span></span>|<span data-ttu-id="08334-p101">Der Typ der Telefonnummer. Mögliche Werte sind: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span><span class="sxs-lookup"><span data-stu-id="08334-p101">The type of phone number. Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="08334-114">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="08334-114">JSON representation</span></span>

<span data-ttu-id="08334-115">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="08334-115">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.phone"
}-->

```json
{
  "number": "string",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "phone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->