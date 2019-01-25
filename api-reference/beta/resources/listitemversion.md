---
author: rgregg
ms.author: rgregg
ms.date: 09/17/2017
title: listItemVersion
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 1d153a8ae8291e0299d1a470db6c8c7e0c8bd3e4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524751"
---
# <a name="listitemversion-resource-type"></a><span data-ttu-id="d1536-102">ListItemVersion-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d1536-102">ListItemVersion resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1536-103">Die **ListItemVersion**-Ressource stellt eine frühere Version der [ListItem](listitem.md)-Ressource dar.</span><span class="sxs-lookup"><span data-stu-id="d1536-103">The **listItemVersion** resource represents a previous version of a [ListItem](listitem.md) resource.</span></span>

## <a name="tasks-on-listitemversion-resources"></a><span data-ttu-id="d1536-104">Aufgaben für ListItemVersion-Ressourcen</span><span class="sxs-lookup"><span data-stu-id="d1536-104">Tasks on ListItemVersion resources</span></span>

<span data-ttu-id="d1536-105">Die folgenden Aufgaben sind für listItemVersion-Ressourcen verfügbar.</span><span class="sxs-lookup"><span data-stu-id="d1536-105">The following tasks are available for listItemVersion resources.</span></span>

|            <span data-ttu-id="d1536-106">Häufige Aufgaben</span><span class="sxs-lookup"><span data-stu-id="d1536-106">Common task</span></span>             |         <span data-ttu-id="d1536-107">HTTP-Methode</span><span class="sxs-lookup"><span data-stu-id="d1536-107">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="d1536-108">[Versionen auflisten][version-list]</span><span class="sxs-lookup"><span data-stu-id="d1536-108">[List versions][version-list]</span></span>      | `GET /sites/{site-id}/items/{item-id}/versions`  |
| <span data-ttu-id="d1536-109">[Version abrufen][version-get]</span><span class="sxs-lookup"><span data-stu-id="d1536-109">[Get version][version-get]</span></span>         | `GET /sites/{site-id}/items/versions/{version-id}`     |
| <span data-ttu-id="d1536-110">[Version wiederherstellen][version-restore]</span><span class="sxs-lookup"><span data-stu-id="d1536-110">[Restore version][version-restore]</span></span> | `POST /sites/{site-id}/items/versions/{version-id}/restore` |

[version-list]: ../api/listitem-list-versions.md
[version-get]: ../api/listitemversion-get.md
[version-restore]: ../api/listitemversion-restore.md


## <a name="json-representation"></a><span data-ttu-id="d1536-111">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d1536-111">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="d1536-112">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d1536-112">Properties</span></span>

|      <span data-ttu-id="d1536-113">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="d1536-113">Property name</span></span>       |                         <span data-ttu-id="d1536-114">Typ</span><span class="sxs-lookup"><span data-stu-id="d1536-114">Type</span></span>                         |                               <span data-ttu-id="d1536-115">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d1536-115">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="d1536-116">**id**</span><span class="sxs-lookup"><span data-stu-id="d1536-116">**id**</span></span>                   | <span data-ttu-id="d1536-117">string</span><span class="sxs-lookup"><span data-stu-id="d1536-117">string</span></span>                                               | <span data-ttu-id="d1536-118">Die ID der Version.</span><span class="sxs-lookup"><span data-stu-id="d1536-118">The ID of the version.</span></span> <span data-ttu-id="d1536-119">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d1536-119">Read-only.</span></span>                                       |
| <span data-ttu-id="d1536-120">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="d1536-120">**lastModifiedBy**</span></span>       | [<span data-ttu-id="d1536-121">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="d1536-121">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="d1536-122">Die Identität des Benutzers, der die Version zuletzt geändert hat.</span><span class="sxs-lookup"><span data-stu-id="d1536-122">Identity of the user which last modified the version.</span></span> <span data-ttu-id="d1536-123">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d1536-123">Read-only.</span></span>        |
| <span data-ttu-id="d1536-124">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="d1536-124">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="d1536-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1536-125">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="d1536-126">Datum und Uhrzeit der letzten Änderung der Version.</span><span class="sxs-lookup"><span data-stu-id="d1536-126">Date and time the version was last modified.</span></span> <span data-ttu-id="d1536-127">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d1536-127">Read-only.</span></span>                 |
| <span data-ttu-id="d1536-128">**published**</span><span class="sxs-lookup"><span data-stu-id="d1536-128">**published**</span></span>            | [<span data-ttu-id="d1536-129">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="d1536-129">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="d1536-130">Zeigt den Veröffentlichungsstatus dieser bestimmten Version an.</span><span class="sxs-lookup"><span data-stu-id="d1536-130">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="d1536-131">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d1536-131">Read-only.</span></span> |


## <a name="relationships"></a><span data-ttu-id="d1536-132">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d1536-132">Relationships</span></span>

<span data-ttu-id="d1536-133">In der folgenden Tabelle werden die Beziehungen der **driveItemVersion**-Ressource zu anderen Ressourcen angegeben.</span><span class="sxs-lookup"><span data-stu-id="d1536-133">The following table defines the relationships that the **driveItemVersion** resource has to other resources.</span></span>

| <span data-ttu-id="d1536-134">Beziehungsname</span><span class="sxs-lookup"><span data-stu-id="d1536-134">Relationship name</span></span> |                      <span data-ttu-id="d1536-135">Typ</span><span class="sxs-lookup"><span data-stu-id="d1536-135">Type</span></span>                      |                               <span data-ttu-id="d1536-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d1536-136">Description</span></span>                                |
| :---------------- | :--------------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="d1536-137">**fields**</span><span class="sxs-lookup"><span data-stu-id="d1536-137">**fields**</span></span>        | [<span data-ttu-id="d1536-138">fieldValueSet</span><span class="sxs-lookup"><span data-stu-id="d1536-138">FieldValueSet</span></span>](../resources/fieldvalueset.md) | <span data-ttu-id="d1536-139">Eine Auflistung der Felder und Werte für diese Version des Listenelements.</span><span class="sxs-lookup"><span data-stu-id="d1536-139">A collection of the fields and values for this version of the list item.</span></span> |


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
