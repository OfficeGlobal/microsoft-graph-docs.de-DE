# <a name="baseitemversion-resource-type"></a><span data-ttu-id="b3f80-101">BaseItemVersion-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b3f80-101">BaseItemVersion resource type</span></span>

<span data-ttu-id="b3f80-102">Die **baseItemVersion**-Ressource stellt eine frühere Version eines Elements oder einer Entität dar.</span><span class="sxs-lookup"><span data-stu-id="b3f80-102">The **baseItemVersion** resource represents a previous version of an item or entity.</span></span>


## <a name="json-representation"></a><span data-ttu-id="b3f80-103">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b3f80-103">JSON representation</span></span>

<!--{
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.baseItemVersion",
  "@type.aka": "oneDrive.baseItemVersion"
}-->

```json
{
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "publication": { "@odata.type": "microsoft.graph.publicationFacet" }
}
```

## <a name="properties"></a><span data-ttu-id="b3f80-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b3f80-104">Properties</span></span>

|      <span data-ttu-id="b3f80-105">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="b3f80-105">Property name</span></span>       |                         <span data-ttu-id="b3f80-106">Typ</span><span class="sxs-lookup"><span data-stu-id="b3f80-106">Type</span></span>                         |                               <span data-ttu-id="b3f80-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b3f80-107">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="b3f80-108">**ID**</span><span class="sxs-lookup"><span data-stu-id="b3f80-108">**id**</span></span>                   | <span data-ttu-id="b3f80-109">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b3f80-109">string</span></span>                                               | <span data-ttu-id="b3f80-110">Die ID der Version.</span><span class="sxs-lookup"><span data-stu-id="b3f80-110">The ID of the version.</span></span> <span data-ttu-id="b3f80-111">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b3f80-111">Read-only.</span></span>                                       |
| <span data-ttu-id="b3f80-112">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="b3f80-112">**lastModifiedBy**</span></span>       | [<span data-ttu-id="b3f80-113">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="b3f80-113">IdentitySet</span></span>](../resources/identitySet.md)           | <span data-ttu-id="b3f80-114">Die Identität des Benutzers, der die Version zuletzt geändert hat.</span><span class="sxs-lookup"><span data-stu-id="b3f80-114">Identity of the user which last modified the version.</span></span> <span data-ttu-id="b3f80-115">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b3f80-115">Read-only.</span></span>        |
| <span data-ttu-id="b3f80-116">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="b3f80-116">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="b3f80-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3f80-117">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="b3f80-118">Datum und Uhrzeit der letzten Änderung der Version.</span><span class="sxs-lookup"><span data-stu-id="b3f80-118">Date and time the version was last modified.</span></span> <span data-ttu-id="b3f80-119">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b3f80-119">Read-only.</span></span>                 |
| <span data-ttu-id="b3f80-120">**Veröffentlichung**</span><span class="sxs-lookup"><span data-stu-id="b3f80-120">**publication**</span></span>          | [<span data-ttu-id="b3f80-121">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="b3f80-121">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="b3f80-122">Zeigt den Veröffentlichungsstatus dieser bestimmten Version an.</span><span class="sxs-lookup"><span data-stu-id="b3f80-122">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="b3f80-123">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b3f80-123">Read-only.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
