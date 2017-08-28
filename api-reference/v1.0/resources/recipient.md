# <a name="recipient-resource-type"></a><span data-ttu-id="7f2cc-101">recipient-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="7f2cc-101">recipient resource type</span></span>

<span data-ttu-id="7f2cc-102">Stellt Informationen zu einem Benutzer am sendenden oder empfangenden Ende eines Ereignisses, einer Nachricht oder einer Gruppenveröffentlichung dar.</span><span class="sxs-lookup"><span data-stu-id="7f2cc-102">Represents information about a user in the sending or receiving end of an event, message or group post.</span></span> 

## <a name="properties"></a><span data-ttu-id="7f2cc-103">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7f2cc-103">Properties</span></span>
| <span data-ttu-id="7f2cc-104">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7f2cc-104">Property</span></span>     | <span data-ttu-id="7f2cc-105">Typ</span><span class="sxs-lookup"><span data-stu-id="7f2cc-105">Type</span></span>   |<span data-ttu-id="7f2cc-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7f2cc-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7f2cc-107">emailAddress</span><span class="sxs-lookup"><span data-stu-id="7f2cc-107">emailAddress</span></span>|[<span data-ttu-id="7f2cc-108">EmailAddress</span><span class="sxs-lookup"><span data-stu-id="7f2cc-108">EmailAddress</span></span>](emailaddress.md)|<span data-ttu-id="7f2cc-109">Die E-Mail-Adresse des Empfängers.</span><span class="sxs-lookup"><span data-stu-id="7f2cc-109">The recipient's email address.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7f2cc-110">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7f2cc-110">JSON representation</span></span>

<span data-ttu-id="7f2cc-111">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7f2cc-111">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recipient"
}-->

```json
{
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recipient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->