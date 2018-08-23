# <a name="educationorganization-resource-type"></a><span data-ttu-id="9dd14-101">Ressourcentyp educationOrganization</span><span class="sxs-lookup"><span data-stu-id="9dd14-101">educationOrganization resource type</span></span>

<span data-ttu-id="9dd14-102">Abstrakte Entität zum Modellieren der Gemeinsamkeit zwischen verschiedenen Organisationstypen im Bildungsbereichs.</span><span class="sxs-lookup"><span data-stu-id="9dd14-102">Abstract entity used to model the commonality between different organization types within the education sector.</span></span>

## <a name="properties"></a><span data-ttu-id="9dd14-103">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9dd14-103">Properties</span></span>
| <span data-ttu-id="9dd14-104">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9dd14-104">Property</span></span>     | <span data-ttu-id="9dd14-105">Typ</span><span class="sxs-lookup"><span data-stu-id="9dd14-105">Type</span></span>   |<span data-ttu-id="9dd14-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9dd14-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9dd14-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9dd14-107">description</span></span>|<span data-ttu-id="9dd14-108">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9dd14-108">String</span></span>| <span data-ttu-id="9dd14-109">Beschreibung der Organisation.</span><span class="sxs-lookup"><span data-stu-id="9dd14-109">Organization description.</span></span>|
|<span data-ttu-id="9dd14-110">displayName</span><span class="sxs-lookup"><span data-stu-id="9dd14-110">displayName</span></span>|<span data-ttu-id="9dd14-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9dd14-111">String</span></span>| <span data-ttu-id="9dd14-112">Anzeigename der Organisation.</span><span class="sxs-lookup"><span data-stu-id="9dd14-112">Organization display name.</span></span>|
|<span data-ttu-id="9dd14-113">externalSource</span><span class="sxs-lookup"><span data-stu-id="9dd14-113">externalSource</span></span>|<span data-ttu-id="9dd14-114">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="9dd14-114">educationExternalSource</span></span>| <span data-ttu-id="9dd14-115">Die Quelle, aus der diese Organisation erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="9dd14-115">Source where this organization was created from.</span></span> <span data-ttu-id="9dd14-116">Mögliche Werte sind: `sis`, `manual` und `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="9dd14-116">The possible values are:</span></span>|

## <a name="relationships"></a><span data-ttu-id="9dd14-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9dd14-117">Relationships</span></span>
<span data-ttu-id="9dd14-118">Keine.</span><span class="sxs-lookup"><span data-stu-id="9dd14-118">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="9dd14-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9dd14-119">JSON representation</span></span>

<span data-ttu-id="9dd14-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9dd14-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOrganization"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "externalSource": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationOrganization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->