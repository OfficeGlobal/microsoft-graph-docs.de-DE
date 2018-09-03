# <a name="inferenceclassificationoverride-resource-type"></a><span data-ttu-id="e8734-101">inferenceClassificationOverride-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e8734-101">inferenceClassificationOverride resource type</span></span>

<span data-ttu-id="e8734-102">Stellt die Außerkraftsetzung eines Benutzers dafür dar, wie eingehende Nachrichten von einem bestimmten Absender immer klassifiziert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="e8734-102">Represents a user's override for how incoming messages from a specific sender should always be classified as.</span></span>


## <a name="methods"></a><span data-ttu-id="e8734-103">Methoden</span><span class="sxs-lookup"><span data-stu-id="e8734-103">Methods</span></span>

| <span data-ttu-id="e8734-104">Methode</span><span class="sxs-lookup"><span data-stu-id="e8734-104">Method</span></span>           | <span data-ttu-id="e8734-105">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="e8734-105">Return Type</span></span>    |<span data-ttu-id="e8734-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e8734-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e8734-107">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="e8734-107">Update</span></span>](../api/inferenceclassificationoverride_update.md) | [<span data-ttu-id="e8734-108">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="e8734-108">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md) |<span data-ttu-id="e8734-109">Ändert das **classifyAs**-Feld einer Außerkraftsetzung wie angegeben.</span><span class="sxs-lookup"><span data-stu-id="e8734-109">Change the **classifyAs** field of an override as specified.</span></span> |
|[<span data-ttu-id="e8734-110">Löschen</span><span class="sxs-lookup"><span data-stu-id="e8734-110">Delete</span></span>](../api/inferenceclassificationoverride_delete.md) | <span data-ttu-id="e8734-111">Keine</span><span class="sxs-lookup"><span data-stu-id="e8734-111">None</span></span> |<span data-ttu-id="e8734-112">Löscht eine Außerkraftsetzung, die durch ihre ID angegeben ist.</span><span class="sxs-lookup"><span data-stu-id="e8734-112">Delete an override specified by its ID.</span></span> |

## <a name="properties"></a><span data-ttu-id="e8734-113">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e8734-113">Properties</span></span>
| <span data-ttu-id="e8734-114">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e8734-114">Property</span></span>     | <span data-ttu-id="e8734-115">Typ</span><span class="sxs-lookup"><span data-stu-id="e8734-115">Type</span></span>   |<span data-ttu-id="e8734-116">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e8734-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e8734-117">classifyAs</span><span class="sxs-lookup"><span data-stu-id="e8734-117">classifyAs</span></span>|<span data-ttu-id="e8734-118">inferenceClassificationType</span><span class="sxs-lookup"><span data-stu-id="e8734-118">InferenceClassificationType</span></span>| <span data-ttu-id="e8734-119">Gibt an, wie eingehende Nachrichten von einem bestimmten Absender stets klassifiziert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="e8734-119">Specifies how incoming messages from a specific sender should always be classified as. Possible values are: , .</span></span> <span data-ttu-id="e8734-120">Die möglichen Werte sind: `focused`, `other`.</span><span class="sxs-lookup"><span data-stu-id="e8734-120">The possible values are:</span></span>|
|<span data-ttu-id="e8734-121">id</span><span class="sxs-lookup"><span data-stu-id="e8734-121">id</span></span>|<span data-ttu-id="e8734-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e8734-122">string</span></span>| <span data-ttu-id="e8734-p102">Der eindeutige Bezeichner der Außerkraftsetzung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e8734-p102">The unique identifier of the override. Read-only.</span></span>|
|<span data-ttu-id="e8734-125">senderEmailAddress</span><span class="sxs-lookup"><span data-stu-id="e8734-125">senderEmailAddress</span></span>|[<span data-ttu-id="e8734-126">emailAddress</span><span class="sxs-lookup"><span data-stu-id="e8734-126">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="e8734-127">Die E-Mail-Adressinformationen des Absenders, für den die Außerkraftsetzung erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="e8734-127">The email address information of the sender for whom the override is created.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e8734-128">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e8734-128">Relationships</span></span>
<span data-ttu-id="e8734-129">Keine</span><span class="sxs-lookup"><span data-stu-id="e8734-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e8734-130">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e8734-130">JSON representation</span></span>

<span data-ttu-id="e8734-131">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e8734-131">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.inferenceClassificationOverride"
}-->

```json
{
  "classifyAs": "string",
  "id": "string (identifier)",
  "senderEmailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "inferenceClassificationOverride resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->