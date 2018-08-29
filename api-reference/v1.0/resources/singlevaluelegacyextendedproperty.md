# <a name="singlevaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="21d48-101">singleValueLegacyExtendedProperty-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="21d48-101">singleValueLegacyExtendedProperty resource type</span></span>

<span data-ttu-id="21d48-102">Eine erweiterte Eigenschaft, die einen einzelnen Wert enthält.</span><span class="sxs-lookup"><span data-stu-id="21d48-102">An extended property that contains a single value.</span></span> 

<span data-ttu-id="21d48-103">Unter [Überblick über erweiterte Eigenschaften](../resources/extended-properties-overview.md) finden Sie weitere Informationen dazu, wann Datenerweiterungen oder erweiterte Eigenschaften verwendet werden sollten und wie erweiterte Eigenschaften angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="21d48-103">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span> 


## <a name="methods"></a><span data-ttu-id="21d48-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="21d48-104">Methods</span></span>

| <span data-ttu-id="21d48-105">Methode</span><span class="sxs-lookup"><span data-stu-id="21d48-105">Method</span></span>           | <span data-ttu-id="21d48-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="21d48-106">Return Type</span></span>    |<span data-ttu-id="21d48-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="21d48-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="21d48-108">Post</span><span class="sxs-lookup"><span data-stu-id="21d48-108">Post</span></span>](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) | <span data-ttu-id="21d48-109">Eine unterstützte Ressourceninstanz: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md) oder [contactFolder](../resources/contactfolder.md), aber nicht [post](../resources/post.md) für die Gruppe.</span><span class="sxs-lookup"><span data-stu-id="21d48-109">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), or [contactFolder](../resources/contactfolder.md), but not group [post](../resources/post.md).</span></span> | <span data-ttu-id="21d48-110">Erstellen einer **singleValueLegacyExtendedProperty** in einer neuen oder vorhandenen Instanz einer unterstützten Ressource.</span><span class="sxs-lookup"><span data-stu-id="21d48-110">Create a **singleValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="21d48-111">Get</span><span class="sxs-lookup"><span data-stu-id="21d48-111">Get</span></span>](../api/singlevaluelegacyextendedproperty_get.md) |<span data-ttu-id="21d48-112">Eine unterstützte Ressourceninstanz oder eine Sammlung von unterstützten Ressourceninstanzen ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md) oder [post](../resources/post.md) für die Gruppe) oder eine solche Instanz erweitert mit einem [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="21d48-112">One or a collection of supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), or group [post](../resources/post.md)), or one such instance expanded with a [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="21d48-113">Abrufen einer Ressourceninstanz mit einer erweiterten Eigenschaft mithilfe von `$expand` oder `$filter`.</span><span class="sxs-lookup"><span data-stu-id="21d48-113">Get a resource instance with an extended property using `$expand` or `$filter`.</span></span>|

## <a name="properties"></a><span data-ttu-id="21d48-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="21d48-114">Properties</span></span>
| <span data-ttu-id="21d48-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="21d48-115">Property</span></span>     | <span data-ttu-id="21d48-116">Typ</span><span class="sxs-lookup"><span data-stu-id="21d48-116">Type</span></span>   |<span data-ttu-id="21d48-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="21d48-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="21d48-118">id</span><span class="sxs-lookup"><span data-stu-id="21d48-118">id</span></span>|<span data-ttu-id="21d48-119">string</span><span class="sxs-lookup"><span data-stu-id="21d48-119">string</span></span>|<span data-ttu-id="21d48-p101">Die Eigenschafts-ID, die zum Identifizieren der Eigenschaft verwendet wird. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="21d48-p101">The property ID used to identify the property. Read-only.</span></span>|
|<span data-ttu-id="21d48-122">value</span><span class="sxs-lookup"><span data-stu-id="21d48-122">value</span></span>|<span data-ttu-id="21d48-123">string</span><span class="sxs-lookup"><span data-stu-id="21d48-123">string</span></span>|<span data-ttu-id="21d48-124">Ein Eigenschaftswert.</span><span class="sxs-lookup"><span data-stu-id="21d48-124">A property value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="21d48-125">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="21d48-125">Relationships</span></span>
<span data-ttu-id="21d48-126">Keine</span><span class="sxs-lookup"><span data-stu-id="21d48-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="21d48-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="21d48-127">JSON representation</span></span>

<span data-ttu-id="21d48-128">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="21d48-128">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty"
}-->

```json
{
  "id": "string (identifier)",
  "value": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "singleValueLegacyExtendedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->