# <a name="multivaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="9df3b-101">multiValueLegacyExtendedProperty-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9df3b-101">multiValueLegacyExtendedProperty resource type</span></span>

<span data-ttu-id="9df3b-102">Eine erweiterte Eigenschaft, die eine Sammlung von Werten enthält.</span><span class="sxs-lookup"><span data-stu-id="9df3b-102">An extended property that contains a collection of values.</span></span>

<span data-ttu-id="9df3b-103">Unter [Überblick über erweiterte Eigenschaften](../resources/extended-properties-overview.md) finden Sie weitere Informationen dazu, wann Datenerweiterungen oder erweiterte Eigenschaften verwendet werden sollten und wie erweiterte Eigenschaften angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="9df3b-103">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="methods"></a><span data-ttu-id="9df3b-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="9df3b-104">Methods</span></span>

| <span data-ttu-id="9df3b-105">Methode</span><span class="sxs-lookup"><span data-stu-id="9df3b-105">Method</span></span>           | <span data-ttu-id="9df3b-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="9df3b-106">Return Type</span></span>    |<span data-ttu-id="9df3b-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9df3b-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9df3b-108">Beitrag</span><span class="sxs-lookup"><span data-stu-id="9df3b-108">Post</span></span>](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | <span data-ttu-id="9df3b-p101">Eine unterstützte Ressourceninstanz: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md) oder [contactFolder](../resources/contactfolder.md). Beachten Sie, dass [post](../resources/post.md) für die Gruppe nicht unterstützt wird.</span><span class="sxs-lookup"><span data-stu-id="9df3b-p101">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), or [contactFolder](../resources/contactfolder.md). Note that group [post](../resources/post.md) is not supported.</span></span> | <span data-ttu-id="9df3b-111">Erstellen einer **multiValueLegacyExtendedProperty** in einer neuen oder vorhandenen Instanz einer unterstützten Ressource.</span><span class="sxs-lookup"><span data-stu-id="9df3b-111">Create a **multiValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="9df3b-112">Get</span><span class="sxs-lookup"><span data-stu-id="9df3b-112">Get</span></span>](../api/multivaluelegacyextendedproperty_get.md) |<span data-ttu-id="9df3b-113">Eine unterstützte Ressourceninstanz ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md) oder [post](../resources/post.md) für die Gruppe), erweitert mit einem [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="9df3b-113">A supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), or group [post](../resources/post.md)) expanded with a [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="9df3b-114">Abrufen einer Ressourceninstanz mit einer erweiterten Eigenschaft mithilfe von `$expand`.</span><span class="sxs-lookup"><span data-stu-id="9df3b-114">Get a resource instance with an extended property using `$expand`.</span></span>|

## <a name="properties"></a><span data-ttu-id="9df3b-115">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9df3b-115">Properties</span></span>
| <span data-ttu-id="9df3b-116">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9df3b-116">Property</span></span>     | <span data-ttu-id="9df3b-117">Typ</span><span class="sxs-lookup"><span data-stu-id="9df3b-117">Type</span></span>   |<span data-ttu-id="9df3b-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9df3b-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9df3b-119">id</span><span class="sxs-lookup"><span data-stu-id="9df3b-119">id</span></span>|<span data-ttu-id="9df3b-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9df3b-120">string</span></span>|<span data-ttu-id="9df3b-p102">Die Eigenschaften-ID. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9df3b-p102">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="9df3b-123">value</span><span class="sxs-lookup"><span data-stu-id="9df3b-123">value</span></span>|<span data-ttu-id="9df3b-124">string collection</span><span class="sxs-lookup"><span data-stu-id="9df3b-124">string collection</span></span>|<span data-ttu-id="9df3b-125">Eine Sammlung von Eigenschaftswerten.</span><span class="sxs-lookup"><span data-stu-id="9df3b-125">A collection of property values.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9df3b-126">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9df3b-126">Relationships</span></span>
<span data-ttu-id="9df3b-127">Keine</span><span class="sxs-lookup"><span data-stu-id="9df3b-127">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="9df3b-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9df3b-128">JSON representation</span></span>

<span data-ttu-id="9df3b-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9df3b-129">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty"
}-->

```json
{
  "id": "string (identifier)",
  "value": ["string"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "multiValueLegacyExtendedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->