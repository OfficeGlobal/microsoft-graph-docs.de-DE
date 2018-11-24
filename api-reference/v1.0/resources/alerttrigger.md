# <a name="alerttrigger-resource-type"></a><span data-ttu-id="0f508-101">Ressourcentyp alertTrigger</span><span class="sxs-lookup"><span data-stu-id="0f508-101">alertTrigger resource type</span></span>

<span data-ttu-id="0f508-102">Enthält Informationen zu den Eigenschaften, die eine Erkennung ausgelöst (Eigenschaften sind in der Warnung Entität vorhanden).</span><span class="sxs-lookup"><span data-stu-id="0f508-102">Contains information about the properties that triggered a detection (properties exist in the alert entity).</span></span>

## <a name="properties"></a><span data-ttu-id="0f508-103">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0f508-103">Properties</span></span>

| <span data-ttu-id="0f508-104">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0f508-104">Property</span></span>   | <span data-ttu-id="0f508-105">Typ</span><span class="sxs-lookup"><span data-stu-id="0f508-105">Type</span></span>|<span data-ttu-id="0f508-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0f508-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0f508-107">name</span><span class="sxs-lookup"><span data-stu-id="0f508-107">name</span></span>|<span data-ttu-id="0f508-108">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0f508-108">String</span></span>|<span data-ttu-id="0f508-109">Der Name der Eigenschaft, die als eine Erkennung Trigger.</span><span class="sxs-lookup"><span data-stu-id="0f508-109">Name of the property serving as a detection trigger.</span></span>|
|<span data-ttu-id="0f508-110">Typ</span><span class="sxs-lookup"><span data-stu-id="0f508-110">type</span></span>|<span data-ttu-id="0f508-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0f508-111">String</span></span>|<span data-ttu-id="0f508-112">Typ der Eigenschaft im Schlüssel / Wert-Paar für Auslegung.</span><span class="sxs-lookup"><span data-stu-id="0f508-112">Type of the property in the key:value pair for interpretation.</span></span> <span data-ttu-id="0f508-113">String, Boolean, beispielsweise usw.</span><span class="sxs-lookup"><span data-stu-id="0f508-113">For example, String, Boolean, etc.</span></span>|
|<span data-ttu-id="0f508-114">Wert</span><span class="sxs-lookup"><span data-stu-id="0f508-114">value</span></span>|<span data-ttu-id="0f508-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0f508-115">String</span></span>|<span data-ttu-id="0f508-116">Der Wert der Eigenschaft, die als eine Erkennung Trigger.</span><span class="sxs-lookup"><span data-stu-id="0f508-116">Value of the property serving as a detection trigger.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0f508-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0f508-117">JSON representation</span></span>

<span data-ttu-id="0f508-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0f508-118">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="0f508-119">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0f508-119">Example</span></span>

```json
{
  "name": "hostState.privateIpAddress",
  "type": "String",
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