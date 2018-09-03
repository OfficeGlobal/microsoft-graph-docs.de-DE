# <a name="listitemversion-resource-type"></a><span data-ttu-id="b98d4-101">ListItemVersion-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b98d4-101">ListItemVersion resource type</span></span>

<span data-ttu-id="b98d4-102">Die **ListItemVersion**-Ressource stellt eine frühere Version der [ListItem](listitem.md)-Ressource dar.</span><span class="sxs-lookup"><span data-stu-id="b98d4-102">The **listItemVersion** resource represents a previous version of a [ListItem](listitem.md) resource.</span></span>

## <a name="tasks-on-listitemversion-resources"></a><span data-ttu-id="b98d4-103">Aufgaben für ListItemVersion-Ressourcen</span><span class="sxs-lookup"><span data-stu-id="b98d4-103">Tasks on ListItemVersion resources</span></span>

<span data-ttu-id="b98d4-104">Die folgenden Aufgaben sind für listItemVersion-Ressourcen verfügbar.</span><span class="sxs-lookup"><span data-stu-id="b98d4-104">The following tasks are available for listItemVersion resources.</span></span>

|            <span data-ttu-id="b98d4-105">Häufige Aufgaben</span><span class="sxs-lookup"><span data-stu-id="b98d4-105">Common task</span></span>             |         <span data-ttu-id="b98d4-106">HTTP-Methode</span><span class="sxs-lookup"><span data-stu-id="b98d4-106">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="b98d4-107">[Versionen auflisten][version-list]</span><span class="sxs-lookup"><span data-stu-id="b98d4-107">[List versions][version-list]</span></span>      | `GET /sites/{site-id}/items/{item-id}/versions`  |
| <span data-ttu-id="b98d4-108">[Version abrufen][version-get]</span><span class="sxs-lookup"><span data-stu-id="b98d4-108">[Get version][version-get]</span></span>         | `GET /sites/{site-id}/items/{item-id}/versions/{version-id}`     |
| <span data-ttu-id="b98d4-109">[Version wiederherstellen][version-restore]</span><span class="sxs-lookup"><span data-stu-id="b98d4-109">[Restore version][version-restore]</span></span> | `POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restore` |

[version-list]: ../api/listitem_list_versions.md
[version-get]: ../api/listitemversion_get.md
[version-restore]: ../api/listitemversion_restore.md


## <a name="json-representation"></a><span data-ttu-id="b98d4-110">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b98d4-110">JSON representation</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.baseItemVersion",
  "@odata.type": "microsoft.graph.listItemVersion",
  "@type.aka": "oneDrive.baseItemVersion"
}-->

```json
{
  "fields": { "@odata.type": "microsoft.graph.fieldValueSet" },
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "published": { "@odata.type": "microsoft.graph.publicationFacet" }
}
```

## <a name="properties"></a><span data-ttu-id="b98d4-111">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b98d4-111">Properties</span></span>

|      <span data-ttu-id="b98d4-112">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="b98d4-112">Property name</span></span>       |                         <span data-ttu-id="b98d4-113">Typ</span><span class="sxs-lookup"><span data-stu-id="b98d4-113">Type</span></span>                         |                               <span data-ttu-id="b98d4-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b98d4-114">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="b98d4-115">**ID**</span><span class="sxs-lookup"><span data-stu-id="b98d4-115">**id**</span></span>                   | <span data-ttu-id="b98d4-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b98d4-116">string</span></span>                                               | <span data-ttu-id="b98d4-117">Die ID der Version.</span><span class="sxs-lookup"><span data-stu-id="b98d4-117">The ID of the version.</span></span> <span data-ttu-id="b98d4-118">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b98d4-118">Read-only.</span></span>                                       |
| <span data-ttu-id="b98d4-119">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="b98d4-119">**lastModifiedBy**</span></span>       | [<span data-ttu-id="b98d4-120">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="b98d4-120">IdentitySet</span></span>](../resources/identitySet.md)           | <span data-ttu-id="b98d4-121">Die Identität des Benutzers, der die Version zuletzt geändert hat.</span><span class="sxs-lookup"><span data-stu-id="b98d4-121">Identity of the user which last modified the version.</span></span> <span data-ttu-id="b98d4-122">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b98d4-122">Read-only.</span></span>        |
| <span data-ttu-id="b98d4-123">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="b98d4-123">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="b98d4-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b98d4-124">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="b98d4-125">Datum und Uhrzeit der letzten Änderung der Version.</span><span class="sxs-lookup"><span data-stu-id="b98d4-125">Date and time the version was last modified.</span></span> <span data-ttu-id="b98d4-126">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b98d4-126">Read-only.</span></span>                 |
| <span data-ttu-id="b98d4-127">**published**</span><span class="sxs-lookup"><span data-stu-id="b98d4-127">**published**</span></span>            | [<span data-ttu-id="b98d4-128">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="b98d4-128">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="b98d4-129">Zeigt den Veröffentlichungsstatus dieser bestimmten Version an.</span><span class="sxs-lookup"><span data-stu-id="b98d4-129">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="b98d4-130">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b98d4-130">Read-only.</span></span> |


## <a name="relationships"></a><span data-ttu-id="b98d4-131">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b98d4-131">Relationships</span></span>

<span data-ttu-id="b98d4-132">In der folgenden Tabelle werden die Beziehungen der **driveItemVersion**-Ressource zu anderen Ressourcen angegeben.</span><span class="sxs-lookup"><span data-stu-id="b98d4-132">The following table defines the relationships that the **driveItemVersion** resource has to other resources.</span></span>

| <span data-ttu-id="b98d4-133">Beziehungsname</span><span class="sxs-lookup"><span data-stu-id="b98d4-133">Relationship name</span></span> |                      <span data-ttu-id="b98d4-134">Typ</span><span class="sxs-lookup"><span data-stu-id="b98d4-134">Type</span></span>                      |                               <span data-ttu-id="b98d4-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b98d4-135">Description</span></span>                                |
| :---------------- | :--------------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="b98d4-136">**Datenfelder**</span><span class="sxs-lookup"><span data-stu-id="b98d4-136">**fields**</span></span>        | [<span data-ttu-id="b98d4-137">fieldValueSet</span><span class="sxs-lookup"><span data-stu-id="b98d4-137">FieldValueSet</span></span>](../resources/fieldvalueset.md) | <span data-ttu-id="b98d4-138">Eine Auflistung der Felder und Werte für diese Version des Listenelements.</span><span class="sxs-lookup"><span data-stu-id="b98d4-138">A collection of the fields and values for this version of the list item.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
