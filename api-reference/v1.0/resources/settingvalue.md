# <a name="settingvalue-resource-type"></a><span data-ttu-id="ce2cd-101">settingValue-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ce2cd-101">settingValue resource type</span></span>

<span data-ttu-id="ce2cd-102">Eine Einstellung, die durch ein Name/Wertpaar dargestellt wird.</span><span class="sxs-lookup"><span data-stu-id="ce2cd-102">A setting represented by a name/value pair.</span></span>

### <a name="properties"></a><span data-ttu-id="ce2cd-103">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ce2cd-103">Properties</span></span>

| <span data-ttu-id="ce2cd-104">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ce2cd-104">Property</span></span> | <span data-ttu-id="ce2cd-105">Typ</span><span class="sxs-lookup"><span data-stu-id="ce2cd-105">Type</span></span> | <span data-ttu-id="ce2cd-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ce2cd-106">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="ce2cd-107">name</span><span class="sxs-lookup"><span data-stu-id="ce2cd-107">name</span></span>|<span data-ttu-id="ce2cd-108">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ce2cd-108">String</span></span>| <span data-ttu-id="ce2cd-109">Name der Einstellung (entsprechend der [groupSettingTemplate](groupsettingtemplate.md)-Definition).</span><span class="sxs-lookup"><span data-stu-id="ce2cd-109">Name of the setting (as defined by the [groupSettingTemplate](groupsettingtemplate.md)).</span></span> |
|<span data-ttu-id="ce2cd-110">Wert</span><span class="sxs-lookup"><span data-stu-id="ce2cd-110">value</span></span>|<span data-ttu-id="ce2cd-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ce2cd-111">String</span></span>| <span data-ttu-id="ce2cd-112">Wert der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="ce2cd-112">Value of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="ce2cd-113">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ce2cd-113">JSON representation</span></span>

<span data-ttu-id="ce2cd-114">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ce2cd-114">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingValue"
}-->

```json
{
  "name": "String",
  "value": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "settingValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->