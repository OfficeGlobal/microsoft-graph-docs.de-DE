---
title: ListItemVersion-Ressourcentyp
description: Die **ListItemVersion**-Ressource stellt eine frühere Version der ListItem-Ressource dar.
ms.openlocfilehash: f036ea217abe766806e7f3c6b24bee4394f54889
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016118"
---
# <a name="listitemversion-resource-type"></a><span data-ttu-id="509c8-103">ListItemVersion-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="509c8-103">ListItemVersion resource type</span></span>

<span data-ttu-id="509c8-104">Die **ListItemVersion**-Ressource stellt eine frühere Version der [ListItem](listitem.md)-Ressource dar.</span><span class="sxs-lookup"><span data-stu-id="509c8-104">The **listItemVersion** resource represents a previous version of a [ListItem](listitem.md) resource.</span></span>

## <a name="tasks-on-listitemversion-resources"></a><span data-ttu-id="509c8-105">Aufgaben für ListItemVersion-Ressourcen</span><span class="sxs-lookup"><span data-stu-id="509c8-105">Tasks on ListItemVersion resources</span></span>

<span data-ttu-id="509c8-106">Die folgenden Aufgaben sind für listItemVersion-Ressourcen verfügbar.</span><span class="sxs-lookup"><span data-stu-id="509c8-106">The following tasks are available for listItemVersion resources.</span></span>

|            <span data-ttu-id="509c8-107">Häufige Aufgaben</span><span class="sxs-lookup"><span data-stu-id="509c8-107">Common task</span></span>             |         <span data-ttu-id="509c8-108">HTTP-Methode</span><span class="sxs-lookup"><span data-stu-id="509c8-108">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="509c8-109">[Versionen auflisten][version-list]</span><span class="sxs-lookup"><span data-stu-id="509c8-109">[List versions][version-list]</span></span>      | `GET /sites/{site-id}/items/{item-id}/versions`  |
| <span data-ttu-id="509c8-110">[Version abrufen][version-get]</span><span class="sxs-lookup"><span data-stu-id="509c8-110">[Get version][version-get]</span></span>         | `GET /sites/{site-id}/items/{item-id}/versions/{version-id}`     |
| <span data-ttu-id="509c8-111">[Version wiederherstellen][version-restore]</span><span class="sxs-lookup"><span data-stu-id="509c8-111">[Restore version][version-restore]</span></span> | `POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restore` |

[version-list]: ../api/listitem-list-versions.md
[version-get]: ../api/listitemversion-get.md
[version-restore]: ../api/listitemversion-restore.md


## <a name="json-representation"></a><span data-ttu-id="509c8-112">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="509c8-112">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="509c8-113">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="509c8-113">Properties</span></span>

|      <span data-ttu-id="509c8-114">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="509c8-114">Property name</span></span>       |                         <span data-ttu-id="509c8-115">Typ</span><span class="sxs-lookup"><span data-stu-id="509c8-115">Type</span></span>                         |                               <span data-ttu-id="509c8-116">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="509c8-116">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="509c8-117">**id**</span><span class="sxs-lookup"><span data-stu-id="509c8-117">**id**</span></span>                   | <span data-ttu-id="509c8-118">string</span><span class="sxs-lookup"><span data-stu-id="509c8-118">string</span></span>                                               | <span data-ttu-id="509c8-119">Die ID der Version.</span><span class="sxs-lookup"><span data-stu-id="509c8-119">The ID of the version.</span></span> <span data-ttu-id="509c8-120">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="509c8-120">Read-only.</span></span>                                       |
| <span data-ttu-id="509c8-121">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="509c8-121">**lastModifiedBy**</span></span>       | [<span data-ttu-id="509c8-122">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="509c8-122">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="509c8-123">Die Identität des Benutzers, der die Version zuletzt geändert hat.</span><span class="sxs-lookup"><span data-stu-id="509c8-123">Identity of the user which last modified the version.</span></span> <span data-ttu-id="509c8-124">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="509c8-124">Read-only.</span></span>        |
| <span data-ttu-id="509c8-125">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="509c8-125">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="509c8-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="509c8-126">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="509c8-127">Datum und Uhrzeit der letzten Änderung der Version.</span><span class="sxs-lookup"><span data-stu-id="509c8-127">Date and time the version was last modified.</span></span> <span data-ttu-id="509c8-128">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="509c8-128">Read-only.</span></span>                 |
| <span data-ttu-id="509c8-129">**published**</span><span class="sxs-lookup"><span data-stu-id="509c8-129">**published**</span></span>            | [<span data-ttu-id="509c8-130">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="509c8-130">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="509c8-131">Zeigt den Veröffentlichungsstatus dieser bestimmten Version an.</span><span class="sxs-lookup"><span data-stu-id="509c8-131">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="509c8-132">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="509c8-132">Read-only.</span></span> |


## <a name="relationships"></a><span data-ttu-id="509c8-133">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="509c8-133">Relationships</span></span>

<span data-ttu-id="509c8-134">In der folgenden Tabelle werden die Beziehungen der **driveItemVersion**-Ressource zu anderen Ressourcen angegeben.</span><span class="sxs-lookup"><span data-stu-id="509c8-134">The following table defines the relationships that the **driveItemVersion** resource has to other resources.</span></span>

| <span data-ttu-id="509c8-135">Beziehungsname</span><span class="sxs-lookup"><span data-stu-id="509c8-135">Relationship name</span></span> |                      <span data-ttu-id="509c8-136">Typ</span><span class="sxs-lookup"><span data-stu-id="509c8-136">Type</span></span>                      |                               <span data-ttu-id="509c8-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="509c8-137">Description</span></span>                                |
| :---------------- | :--------------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="509c8-138">**fields**</span><span class="sxs-lookup"><span data-stu-id="509c8-138">**fields**</span></span>        | [<span data-ttu-id="509c8-139">fieldValueSet</span><span class="sxs-lookup"><span data-stu-id="509c8-139">FieldValueSet</span></span>](../resources/fieldvalueset.md) | <span data-ttu-id="509c8-140">Eine Auflistung der Felder und Werte für diese Version des Listenelements.</span><span class="sxs-lookup"><span data-stu-id="509c8-140">A collection of the fields and values for this version of the list item.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
