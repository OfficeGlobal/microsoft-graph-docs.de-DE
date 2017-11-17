# <a name="extensionschemaproperty-resource-type"></a><span data-ttu-id="b13e5-101">extensionSchemaProperty-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b13e5-101">extensionSchemaProperty resource type</span></span>

<span data-ttu-id="b13e5-102">Verwenden Sie die **extensionSchemaProperty**-Ressource, um den Namen und den Typ einer Eigenschaft im Rahmen einer [schemaExtension](schemaextension.md)-Definition zu definieren.</span><span class="sxs-lookup"><span data-stu-id="b13e5-102">Use the **extensionSchemaProperty** resource to define a property's name and its type, as part of a [schemaExtension](schemaextension.md) definition.</span></span>


## <a name="properties"></a><span data-ttu-id="b13e5-103">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b13e5-103">Properties</span></span>
| <span data-ttu-id="b13e5-104">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b13e5-104">Property</span></span>     | <span data-ttu-id="b13e5-105">Typ</span><span class="sxs-lookup"><span data-stu-id="b13e5-105">Type</span></span>   |<span data-ttu-id="b13e5-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b13e5-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b13e5-107">name</span><span class="sxs-lookup"><span data-stu-id="b13e5-107">name</span></span>|<span data-ttu-id="b13e5-108">String</span><span class="sxs-lookup"><span data-stu-id="b13e5-108">String</span></span>| <span data-ttu-id="b13e5-109">Der Name der stark typisierten Eigenschaft, die im Rahmen der Schemaerweiterung definiert wird.</span><span class="sxs-lookup"><span data-stu-id="b13e5-109">The name of the strongly-typed property defined as part of a schema extension.</span></span>|
|<span data-ttu-id="b13e5-110">type</span><span class="sxs-lookup"><span data-stu-id="b13e5-110">type</span></span>|<span data-ttu-id="b13e5-111">String</span><span class="sxs-lookup"><span data-stu-id="b13e5-111">String</span></span>| <span data-ttu-id="b13e5-p101">Der Typ der Eigenschaft, die im Rahmen der Schemaerweiterung definiert wird.  Zulässige Werte sind *Binary, Boolean, DateTime, Integer* oder *String*.  Weitere Einzelheiten finden Sie in der Tabelle unten.</span><span class="sxs-lookup"><span data-stu-id="b13e5-p101">The type of the property that is defined as part of a schema extension.  Allowed values are *Binary, Boolean, DateTime, Integer* or *String*.  See the table below for more details.</span></span>|

#### <a name="supported-property-data-types"></a><span data-ttu-id="b13e5-115">Unterstützte Datentypen für Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b13e5-115">Supported property data types</span></span> 
<span data-ttu-id="b13e5-116">Die folgenden Datentypen werden beim Definieren einer Eigenschaft in einer Schemaerweiterung unterstützt:</span><span class="sxs-lookup"><span data-stu-id="b13e5-116">The following data types are supported when defining a property in a schema extension:</span></span>

| <span data-ttu-id="b13e5-117">Eigenschaftentyp</span><span class="sxs-lookup"><span data-stu-id="b13e5-117">Property Type</span></span> | <span data-ttu-id="b13e5-118">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="b13e5-118">Remarks</span></span> |
|-------------|------------|
| <span data-ttu-id="b13e5-119">Binär</span><span class="sxs-lookup"><span data-stu-id="b13e5-119">Binary</span></span> | <span data-ttu-id="b13e5-120">Maximal 256 Bytes.</span><span class="sxs-lookup"><span data-stu-id="b13e5-120">256 bytes maximum.</span></span> |
| <span data-ttu-id="b13e5-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="b13e5-121">Boolean</span></span> | <span data-ttu-id="b13e5-122">Nicht unterstützt für Kontakte, Nachrichten, Ereignisse und Beiträge.</span><span class="sxs-lookup"><span data-stu-id="b13e5-122">Not supported for messages, events and posts.</span></span> |
| <span data-ttu-id="b13e5-123">DateTime</span><span class="sxs-lookup"><span data-stu-id="b13e5-123">DateTime</span></span> | <span data-ttu-id="b13e5-p102">Muss im ISO 8601-Format angegeben werden. Wird in UTC gespeichert.</span><span class="sxs-lookup"><span data-stu-id="b13e5-p102">Must be specified in ISO 8601 format. Will be stored in UTC.</span></span> |
| <span data-ttu-id="b13e5-126">Ganze Zahl</span><span class="sxs-lookup"><span data-stu-id="b13e5-126">Integer</span></span> | <span data-ttu-id="b13e5-127">32-Bit-Wert.</span><span class="sxs-lookup"><span data-stu-id="b13e5-127">A 32-bit integer value.</span></span> <span data-ttu-id="b13e5-128">Nicht unterstützt für Kontakte, Nachrichten, Ereignisse und Beiträge.</span><span class="sxs-lookup"><span data-stu-id="b13e5-128">Not supported for messages, events and posts.</span></span> |
| <span data-ttu-id="b13e5-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b13e5-129">String</span></span> | <span data-ttu-id="b13e5-130">Maximal 256 Zeichen.</span><span class="sxs-lookup"><span data-stu-id="b13e5-130">256 characters maximum.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b13e5-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b13e5-131">JSON representation</span></span>
<span data-ttu-id="b13e5-132">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b13e5-132">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.extensionSchemaProperty"
}-->

```json
{
  "name": "String",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "extensionSchemaProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
