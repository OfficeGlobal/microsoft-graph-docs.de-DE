# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="7143a-101">settingTemplateValue-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="7143a-101">settingTemplateValue resource type</span></span>

<span data-ttu-id="7143a-102">Stellt eine einzelne Vorlageneinstellungsdefinition dar, einschließlich des Standardwerts für die Einstellung, wenn die Einstellung nicht instanziiert wurde.</span><span class="sxs-lookup"><span data-stu-id="7143a-102">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>

### <a name="properties"></a><span data-ttu-id="7143a-103">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7143a-103">Properties</span></span>

| <span data-ttu-id="7143a-104">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7143a-104">Property</span></span> | <span data-ttu-id="7143a-105">Typ</span><span class="sxs-lookup"><span data-stu-id="7143a-105">Type</span></span> | <span data-ttu-id="7143a-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7143a-106">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="7143a-107">defaultValue</span><span class="sxs-lookup"><span data-stu-id="7143a-107">DefaultValue</span></span>|<span data-ttu-id="7143a-108">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7143a-108">String</span></span>| <span data-ttu-id="7143a-109">Der Standardwert für die Einstellung.</span><span class="sxs-lookup"><span data-stu-id="7143a-109">Default value for the setting.</span></span> |
|<span data-ttu-id="7143a-110">description</span><span class="sxs-lookup"><span data-stu-id="7143a-110">description</span></span>|<span data-ttu-id="7143a-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7143a-111">String</span></span>| <span data-ttu-id="7143a-112">Beschreibung der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="7143a-112">Description of the component.</span></span> |
|<span data-ttu-id="7143a-113">Name</span><span class="sxs-lookup"><span data-stu-id="7143a-113">name</span></span>|<span data-ttu-id="7143a-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7143a-114">String</span></span>| <span data-ttu-id="7143a-115">Der Name der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="7143a-115">Name of the setting.</span></span> |
|<span data-ttu-id="7143a-116">type</span><span class="sxs-lookup"><span data-stu-id="7143a-116">type</span></span>|<span data-ttu-id="7143a-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7143a-117">String</span></span>| <span data-ttu-id="7143a-118">Der Typ der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="7143a-118">Key of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="7143a-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7143a-119">JSON representation</span></span>

<span data-ttu-id="7143a-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7143a-120">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingTemplateValue"
}-->

```json
{
  "defaultValue": "String",
  "description": "String",
  "name": "String",
  "type": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "settingTemplateValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->