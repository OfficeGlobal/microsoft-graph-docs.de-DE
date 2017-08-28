# <a name="emailaddress-resource-type"></a><span data-ttu-id="f21aa-101">emailAddress-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f21aa-101">emailAddress resource type</span></span>

<span data-ttu-id="f21aa-102">Name und E-Mail-Adresse eines Kontakts oder eines Empfängers der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="f21aa-102">The name and email address of a contact or message recipient.</span></span>

## <a name="properties"></a><span data-ttu-id="f21aa-103">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f21aa-103">Properties</span></span>
| <span data-ttu-id="f21aa-104">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f21aa-104">Property</span></span>     | <span data-ttu-id="f21aa-105">Typ</span><span class="sxs-lookup"><span data-stu-id="f21aa-105">Type</span></span>   |<span data-ttu-id="f21aa-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f21aa-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f21aa-107">address</span><span class="sxs-lookup"><span data-stu-id="f21aa-107">address</span></span>|<span data-ttu-id="f21aa-108">String</span><span class="sxs-lookup"><span data-stu-id="f21aa-108">String</span></span>|<span data-ttu-id="f21aa-109">Die E-Mail-Adresse der Person oder Organisation.</span><span class="sxs-lookup"><span data-stu-id="f21aa-109">The email address of the person or entity.</span></span>|
|<span data-ttu-id="f21aa-110">name</span><span class="sxs-lookup"><span data-stu-id="f21aa-110">name</span></span>|<span data-ttu-id="f21aa-111">String</span><span class="sxs-lookup"><span data-stu-id="f21aa-111">String</span></span>|<span data-ttu-id="f21aa-112">Der Anzeigename der Person oder Entität.</span><span class="sxs-lookup"><span data-stu-id="f21aa-112">The display name of the person or entity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f21aa-113">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f21aa-113">JSON representation</span></span>

<span data-ttu-id="f21aa-114">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f21aa-114">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.emailAddress"
}-->

```json
{
  "address": "string",
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "emailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
