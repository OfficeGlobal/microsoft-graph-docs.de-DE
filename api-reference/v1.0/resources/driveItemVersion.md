# <a name="driveitemversion-resource-type"></a><span data-ttu-id="c405b-101">DriveItemVersion-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c405b-101">DriveItemVersion resource type</span></span>

<span data-ttu-id="c405b-102">Die **DriveItemVersion**-Ressource stellt eine bestimmte Version eines [DriveItem](driveitem.md) dar.</span><span class="sxs-lookup"><span data-stu-id="c405b-102">The **DriveItemVersion** resource represents a specific version of a [DriveItem](driveitem.md).</span></span>


## <a name="tasks-on-driveitemversion-resources"></a><span data-ttu-id="c405b-103">Aufgaben für DriveItemVersion-Ressourcen</span><span class="sxs-lookup"><span data-stu-id="c405b-103">Tasks on DriveItemVersion resources</span></span>

<span data-ttu-id="c405b-104">Die folgenden Aufgaben sind für driveItemVersion-Ressourcen verfügbar.</span><span class="sxs-lookup"><span data-stu-id="c405b-104">The following tasks are available for driveItemVersion resources.</span></span>

|            <span data-ttu-id="c405b-105">Häufige Aufgaben</span><span class="sxs-lookup"><span data-stu-id="c405b-105">Common task</span></span>             |         <span data-ttu-id="c405b-106">HTTP-Methode</span><span class="sxs-lookup"><span data-stu-id="c405b-106">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="c405b-107">[Versionen auflisten][version-list]</span><span class="sxs-lookup"><span data-stu-id="c405b-107">[List versions][version-list]</span></span>      | `GET /drive/items/{item-id}/versions`  |
| <span data-ttu-id="c405b-108">[Version abrufen][version-get]</span><span class="sxs-lookup"><span data-stu-id="c405b-108">[Get version][version-get]</span></span>         | `GET /drive/items/{item-id}/versions/{version-id}`     |
| <span data-ttu-id="c405b-109">[Inhalte abrufen][content-get]</span><span class="sxs-lookup"><span data-stu-id="c405b-109">[Get contents][content-get]</span></span>        | `GET /drive/items/{item-id}/versions/{version-id}/content` |
| <span data-ttu-id="c405b-110">[Version wiederherstellen][version-restore]</span><span class="sxs-lookup"><span data-stu-id="c405b-110">[Restore version][version-restore]</span></span> | `POST /drive/items/{item-id}/versions/{version-id}/restore` |

[version-list]: ../api/driveitem_list_versions.md
[version-get]: ../api/driveitemversion_get.md
[content-get]: ../api/driveitemversion_get_contents.md
[version-restore]: ../api/driveitemversion_restore.md

<span data-ttu-id="c405b-111">Im Beispiel der vorstehenden Tabelle wird `/drive` verwendet, aber es gibt viele gültige Abfragen.</span><span class="sxs-lookup"><span data-stu-id="c405b-111">In the previous table, the examples use `/drive`, but there are many valid requests.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c405b-112">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c405b-112">JSON representation</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.baseItemVersion",
  "@odata.type": "microsoft.graph.driveItemVersion",
  "@type.aka": "oneDrive.driveItemVersion"
}-->

```json
{
  "content": { "@odata.type": "Edm.Stream" },
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "publication": { "@odata.type": "microsoft.graph.publicationFacet" },
  "size": 12356
}
```

## <a name="properties"></a><span data-ttu-id="c405b-113">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c405b-113">Properties</span></span>

|      <span data-ttu-id="c405b-114">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="c405b-114">Property name</span></span>       |                         <span data-ttu-id="c405b-115">Typ</span><span class="sxs-lookup"><span data-stu-id="c405b-115">Type</span></span>                         |                               <span data-ttu-id="c405b-116">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c405b-116">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="c405b-117">**ID**</span><span class="sxs-lookup"><span data-stu-id="c405b-117">**id**</span></span>                   | <span data-ttu-id="c405b-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c405b-118">string</span></span>                                               | <span data-ttu-id="c405b-119">Die ID der Version.</span><span class="sxs-lookup"><span data-stu-id="c405b-119">The ID of the version.</span></span> <span data-ttu-id="c405b-120">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c405b-120">Read-only.</span></span>                                       |
| <span data-ttu-id="c405b-121">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="c405b-121">**lastModifiedBy**</span></span>       | [<span data-ttu-id="c405b-122">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="c405b-122">IdentitySet</span></span>](../resources/identitySet.md)           | <span data-ttu-id="c405b-123">Die Identität des Benutzers, der die Version zuletzt geändert hat.</span><span class="sxs-lookup"><span data-stu-id="c405b-123">Identity of the user which last modified the version.</span></span> <span data-ttu-id="c405b-124">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c405b-124">Read-only.</span></span>        |
| <span data-ttu-id="c405b-125">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="c405b-125">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="c405b-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c405b-126">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="c405b-127">Datum und Uhrzeit der letzten Änderung der Version.</span><span class="sxs-lookup"><span data-stu-id="c405b-127">Date and time the version was last modified.</span></span> <span data-ttu-id="c405b-128">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c405b-128">Read-only.</span></span>                 |
| <span data-ttu-id="c405b-129">**Veröffentlichung**</span><span class="sxs-lookup"><span data-stu-id="c405b-129">**publication**</span></span>          | [<span data-ttu-id="c405b-130">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="c405b-130">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="c405b-131">Zeigt den Veröffentlichungsstatus dieser bestimmten Version an.</span><span class="sxs-lookup"><span data-stu-id="c405b-131">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="c405b-132">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c405b-132">Read-only.</span></span> |
| <span data-ttu-id="c405b-133">**Größe**</span><span class="sxs-lookup"><span data-stu-id="c405b-133">**size**</span></span>                 | <span data-ttu-id="c405b-134">Int64</span><span class="sxs-lookup"><span data-stu-id="c405b-134">Int64</span></span>                                                | <span data-ttu-id="c405b-135">Gibt die Größe des Inhalt-Streams für diese Version des Elements an.</span><span class="sxs-lookup"><span data-stu-id="c405b-135">Indicates the size of the content stream for this version of the item.</span></span>  |
| <span data-ttu-id="c405b-136">**Inhalt**</span><span class="sxs-lookup"><span data-stu-id="c405b-136">**content**</span></span>              | <span data-ttu-id="c405b-137">Stream</span><span class="sxs-lookup"><span data-stu-id="c405b-137">Stream</span></span>                                               | <span data-ttu-id="c405b-138">Der Inhaltsstream für diese Version des Elements.</span><span class="sxs-lookup"><span data-stu-id="c405b-138">Indicates the size of the content stream for this version of the item.</span></span>                        |

<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
