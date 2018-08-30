# <a name="inferenceclassification-resource-type"></a><span data-ttu-id="f8bdb-101">inferenceClassification-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f8bdb-101">inferenceClassification resource type</span></span>

<span data-ttu-id="f8bdb-102">Klassifizierung der Nachrichten eines Benutzers, um den Fokus auf die Nachrichten zu legen, die für den Benutzer relevanter oder wichtiger sind.</span><span class="sxs-lookup"><span data-stu-id="f8bdb-102">Classification of a user's messages to enable focus on those that are more relevant or important to the user.</span></span> 

<span data-ttu-id="f8bdb-103">Weitere Informationen finden Sie unter [Posteingang mit Relevanz verwalten](manage_focused_inbox.md).</span><span class="sxs-lookup"><span data-stu-id="f8bdb-103">For more information, see [Manage Focused Inbox](manage_focused_inbox.md).</span></span>


## <a name="methods"></a><span data-ttu-id="f8bdb-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="f8bdb-104">Methods</span></span>

| <span data-ttu-id="f8bdb-105">Methode</span><span class="sxs-lookup"><span data-stu-id="f8bdb-105">Method</span></span>           | <span data-ttu-id="f8bdb-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="f8bdb-106">Return Type</span></span>    |<span data-ttu-id="f8bdb-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f8bdb-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f8bdb-108">inferenceClassificationOverride erstellen</span><span class="sxs-lookup"><span data-stu-id="f8bdb-108">Create inferenceClassificationOverride</span></span>](../api/inferenceclassification_post_overrides.md) |[<span data-ttu-id="f8bdb-109">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="f8bdb-109">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md)| <span data-ttu-id="f8bdb-p101">Erstellen einer Außerkraftsetzung für einen Absender, der durch eine SMTP-Adresse identifiziert wird. Künftige Nachrichten von dieser SMTP-Adresse werden durchgängig klassifiziert wie in der Außerkraftsetzung angegeben.</span><span class="sxs-lookup"><span data-stu-id="f8bdb-p101">Create an override for a sender identified by an SMTP address. Future messages from that SMTP address will be consistently classified as specified in the override.</span></span>|
|[<span data-ttu-id="f8bdb-112">Außerkraftsetzungen auflisten</span><span class="sxs-lookup"><span data-stu-id="f8bdb-112">List overrides</span></span>](../api/inferenceclassification_list_overrides.md) |<span data-ttu-id="f8bdb-113">[inferenceClassificationOverride](inferenceclassificationoverride.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="f8bdb-113">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="f8bdb-114">Dient zum Abrufen der Außerkraftsetzungen, die ein Benutzer eingerichtet hat, um Nachrichten von bestimmten Absendern immer auf eine bestimmte Art und Weise zu klassifizieren.</span><span class="sxs-lookup"><span data-stu-id="f8bdb-114">Get the overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>|

## <a name="properties"></a><span data-ttu-id="f8bdb-115">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f8bdb-115">Properties</span></span>
| <span data-ttu-id="f8bdb-116">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f8bdb-116">Property</span></span>     | <span data-ttu-id="f8bdb-117">Typ</span><span class="sxs-lookup"><span data-stu-id="f8bdb-117">Type</span></span>   |<span data-ttu-id="f8bdb-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f8bdb-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f8bdb-119">ID</span><span class="sxs-lookup"><span data-stu-id="f8bdb-119">id</span></span>|<span data-ttu-id="f8bdb-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f8bdb-120">string</span></span>| <span data-ttu-id="f8bdb-121">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f8bdb-121">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f8bdb-122">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f8bdb-122">Relationships</span></span>
| <span data-ttu-id="f8bdb-123">Beziehung</span><span class="sxs-lookup"><span data-stu-id="f8bdb-123">Relationship</span></span> | <span data-ttu-id="f8bdb-124">Typ</span><span class="sxs-lookup"><span data-stu-id="f8bdb-124">Type</span></span>   |<span data-ttu-id="f8bdb-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f8bdb-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f8bdb-126">Außerkraftsetzungen</span><span class="sxs-lookup"><span data-stu-id="f8bdb-126">overrides</span></span>|<span data-ttu-id="f8bdb-127">[inferenceClassificationOverride](inferenceclassificationoverride.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="f8bdb-127">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="f8bdb-p102">Eine Reihe von Außerkraftsetzungen für einen Benutzer, um Nachrichten von bestimmten Absendern immer auf eine bestimmte Art und Weise zu klassifizieren: `focused` oder `other`. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="f8bdb-p102">A set of overrides for a user to always classify messages from specific senders in certain ways: `focused`, or `other`. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f8bdb-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f8bdb-131">JSON representation</span></span>

<span data-ttu-id="f8bdb-132">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f8bdb-132">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.inferenceClassification",
  "@odata.annotations": [
    {
      "property": "overrides",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    }
  ]
}-->

```json
{
  "id": "string (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "inferenceClassification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->