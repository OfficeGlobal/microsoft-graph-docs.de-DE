# <a name="alerttrigger-resource-type"></a><span data-ttu-id="7e08e-101">Ressourcentyp alertTrigger</span><span class="sxs-lookup"><span data-stu-id="7e08e-101">alertTrigger resource type</span></span>

<span data-ttu-id="7e08e-102">Enthält Informationen zu den Eigenschaften, die eine Erkennung ausgelöst haben (Eigenschaften sind in der Warnungsentität vorhanden).</span><span class="sxs-lookup"><span data-stu-id="7e08e-102">Contains information about the properties that triggered a detection (properties exist in the alert entity).</span></span>

## <a name="properties"></a><span data-ttu-id="7e08e-103">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7e08e-103">Properties</span></span>

| <span data-ttu-id="7e08e-104">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7e08e-104">Property</span></span>   | <span data-ttu-id="7e08e-105">Typ</span><span class="sxs-lookup"><span data-stu-id="7e08e-105">Type</span></span>|<span data-ttu-id="7e08e-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7e08e-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7e08e-107">Name</span><span class="sxs-lookup"><span data-stu-id="7e08e-107">name</span></span>|<span data-ttu-id="7e08e-108">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7e08e-108">String</span></span>|<span data-ttu-id="7e08e-109">Der Name der Eigenschaft, der als ein Erkennungstrigger gedient hat.</span><span class="sxs-lookup"><span data-stu-id="7e08e-109">Name of the property serving as a detection trigger.</span></span>|
|<span data-ttu-id="7e08e-110">Typ</span><span class="sxs-lookup"><span data-stu-id="7e08e-110">type</span></span>|<span data-ttu-id="7e08e-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7e08e-111">String</span></span>|<span data-ttu-id="7e08e-112">Typ der Eigenschaft im Schlüssel/Wert-Paar für die Auslegung.</span><span class="sxs-lookup"><span data-stu-id="7e08e-112">Type of the property in the key:value pair for interpretation.</span></span> <span data-ttu-id="7e08e-113">Bspw. String, Boolean, usw.</span><span class="sxs-lookup"><span data-stu-id="7e08e-113">For example, String, Boolean, etc.</span></span>|
|<span data-ttu-id="7e08e-114">Wert</span><span class="sxs-lookup"><span data-stu-id="7e08e-114">value</span></span>|<span data-ttu-id="7e08e-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7e08e-115">String</span></span>|<span data-ttu-id="7e08e-116">Der Wert der Eigenschaft, der als ein Erkennungstrigger gedient hat.</span><span class="sxs-lookup"><span data-stu-id="7e08e-116">Value of the property serving as a detection trigger.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7e08e-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7e08e-117">JSON representation</span></span>

<span data-ttu-id="7e08e-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7e08e-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alertTrigger"
}-->

```json
{
  "name": "String",
  "type": "String",
  "value": "String"
}

```

## <a name="example"></a><span data-ttu-id="7e08e-119">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7e08e-119">Example</span></span>

```json
{
  "name": "endpointAddress",
  "type": "networkConnection.sourceAddress",
  "value": "10.154.9.40"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alertTrigger resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->