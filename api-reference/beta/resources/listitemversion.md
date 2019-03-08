---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/17/2017
title: ListItemVersion
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: d9b06b54d12abddd3a1586a11b99f7c600ac4508
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482301"
---
# <a name="listitemversion-resource-type"></a><span data-ttu-id="8ce58-102">ListItemVersion-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8ce58-102">ListItemVersion resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ce58-103">Die **ListItemVersion**-Ressource stellt eine frühere Version der [ListItem](listitem.md)-Ressource dar.</span><span class="sxs-lookup"><span data-stu-id="8ce58-103">The **listItemVersion** resource represents a previous version of a [ListItem](listitem.md) resource.</span></span>

## <a name="tasks-on-listitemversion-resources"></a><span data-ttu-id="8ce58-104">Aufgaben für ListItemVersion-Ressourcen</span><span class="sxs-lookup"><span data-stu-id="8ce58-104">Tasks on ListItemVersion resources</span></span>

<span data-ttu-id="8ce58-105">Die folgenden Aufgaben sind für listItemVersion-Ressourcen verfügbar.</span><span class="sxs-lookup"><span data-stu-id="8ce58-105">The following tasks are available for listItemVersion resources.</span></span>

|            <span data-ttu-id="8ce58-106">Häufige Aufgaben</span><span class="sxs-lookup"><span data-stu-id="8ce58-106">Common task</span></span>             |         <span data-ttu-id="8ce58-107">HTTP-Methode</span><span class="sxs-lookup"><span data-stu-id="8ce58-107">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="8ce58-108">[Versionen auflisten][version-list]</span><span class="sxs-lookup"><span data-stu-id="8ce58-108">[List versions][version-list]</span></span>      | `GET /sites/{site-id}/items/{item-id}/versions`  |
| <span data-ttu-id="8ce58-109">[Version abrufen][version-get]</span><span class="sxs-lookup"><span data-stu-id="8ce58-109">[Get version][version-get]</span></span>         | `GET /sites/{site-id}/items/versions/{version-id}`     |
| <span data-ttu-id="8ce58-110">[Version wiederherstellen][version-restore]</span><span class="sxs-lookup"><span data-stu-id="8ce58-110">[Restore version][version-restore]</span></span> | `POST /sites/{site-id}/items/versions/{version-id}/restore` |

[version-list]: ../api/listitem-list-versions.md
[version-get]: ../api/listitemversion-get.md
[version-restore]: ../api/listitemversion-restore.md


## <a name="json-representation"></a><span data-ttu-id="8ce58-111">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8ce58-111">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.listItemVersion", "@type.aka": "oneDrive.baseItemVersion" } -->

```json
{
  "content": { "@odata.type": "Edm.Stream" },
  "fields": { "@odata.type": "microsoft.graph.fieldValueSet" },
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "published": { "@odata.type": "microsoft.graph.publicationFacet" }
}
```

## <a name="properties"></a><span data-ttu-id="8ce58-112">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8ce58-112">Properties</span></span>

|      <span data-ttu-id="8ce58-113">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="8ce58-113">Property name</span></span>       |                         <span data-ttu-id="8ce58-114">Typ</span><span class="sxs-lookup"><span data-stu-id="8ce58-114">Type</span></span>                         |                               <span data-ttu-id="8ce58-115">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8ce58-115">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="8ce58-116">**id**</span><span class="sxs-lookup"><span data-stu-id="8ce58-116">**id**</span></span>                   | <span data-ttu-id="8ce58-117">string</span><span class="sxs-lookup"><span data-stu-id="8ce58-117">string</span></span>                                               | <span data-ttu-id="8ce58-118">Die ID der Version.</span><span class="sxs-lookup"><span data-stu-id="8ce58-118">The ID of the version.</span></span> <span data-ttu-id="8ce58-119">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8ce58-119">Read-only.</span></span>                                       |
| <span data-ttu-id="8ce58-120">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="8ce58-120">**lastModifiedBy**</span></span>       | [<span data-ttu-id="8ce58-121">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="8ce58-121">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="8ce58-122">Die Identität des Benutzers, der die Version zuletzt geändert hat.</span><span class="sxs-lookup"><span data-stu-id="8ce58-122">Identity of the user which last modified the version.</span></span> <span data-ttu-id="8ce58-123">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8ce58-123">Read-only.</span></span>        |
| <span data-ttu-id="8ce58-124">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="8ce58-124">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="8ce58-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ce58-125">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="8ce58-126">Datum und Uhrzeit der letzten Änderung der Version.</span><span class="sxs-lookup"><span data-stu-id="8ce58-126">Date and time the version was last modified.</span></span> <span data-ttu-id="8ce58-127">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8ce58-127">Read-only.</span></span>                 |
| <span data-ttu-id="8ce58-128">**published**</span><span class="sxs-lookup"><span data-stu-id="8ce58-128">**published**</span></span>            | [<span data-ttu-id="8ce58-129">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="8ce58-129">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="8ce58-130">Zeigt den Veröffentlichungsstatus dieser bestimmten Version an.</span><span class="sxs-lookup"><span data-stu-id="8ce58-130">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="8ce58-131">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8ce58-131">Read-only.</span></span> |


## <a name="relationships"></a><span data-ttu-id="8ce58-132">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8ce58-132">Relationships</span></span>

<span data-ttu-id="8ce58-133">In der folgenden Tabelle werden die Beziehungen der **driveItemVersion**-Ressource zu anderen Ressourcen angegeben.</span><span class="sxs-lookup"><span data-stu-id="8ce58-133">The following table defines the relationships that the **driveItemVersion** resource has to other resources.</span></span>

| <span data-ttu-id="8ce58-134">Beziehungsname</span><span class="sxs-lookup"><span data-stu-id="8ce58-134">Relationship name</span></span> |                      <span data-ttu-id="8ce58-135">Typ</span><span class="sxs-lookup"><span data-stu-id="8ce58-135">Type</span></span>                      |                               <span data-ttu-id="8ce58-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8ce58-136">Description</span></span>                                |
| :---------------- | :--------------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="8ce58-137">**fields**</span><span class="sxs-lookup"><span data-stu-id="8ce58-137">**fields**</span></span>        | [<span data-ttu-id="8ce58-138">fieldValueSet</span><span class="sxs-lookup"><span data-stu-id="8ce58-138">FieldValueSet</span></span>](../resources/fieldvalueset.md) | <span data-ttu-id="8ce58-139">Eine Auflistung der Felder und Werte für diese Version des Listenelements.</span><span class="sxs-lookup"><span data-stu-id="8ce58-139">A collection of the fields and values for this version of the list item.</span></span> |


<!--
{
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version",
  "suppressions": [
    "Error: /api-reference/beta/resources/listitemversion.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
