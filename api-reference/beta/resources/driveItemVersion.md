---
author: rgregg
ms.author: rgregg
ms.date: 09/17/2017
title: driveItemVersion
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 25b480a22b93ce454927177d2d842390496f54de
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528970"
---
# <a name="driveitemversion-resource-type"></a><span data-ttu-id="1f244-102">DriveItemVersion-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="1f244-102">DriveItemVersion resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f244-103">Die **DriveItemVersion**-Ressource stellt eine bestimmte Version eines [DriveItem](driveitem.md) dar.</span><span class="sxs-lookup"><span data-stu-id="1f244-103">The **DriveItemVersion** resource represents a specific version of a [DriveItem](driveitem.md).</span></span>


## <a name="tasks-on-driveitemversion-resources"></a><span data-ttu-id="1f244-104">Aufgaben für DriveItemVersion-Ressourcen</span><span class="sxs-lookup"><span data-stu-id="1f244-104">Tasks on DriveItemVersion resources</span></span>

<span data-ttu-id="1f244-105">Die folgenden Aufgaben sind für driveItemVersion-Ressourcen verfügbar.</span><span class="sxs-lookup"><span data-stu-id="1f244-105">The following tasks are available for driveItemVersion resources.</span></span>

|            <span data-ttu-id="1f244-106">Häufige Aufgaben</span><span class="sxs-lookup"><span data-stu-id="1f244-106">Common task</span></span>             |         <span data-ttu-id="1f244-107">HTTP-Methode</span><span class="sxs-lookup"><span data-stu-id="1f244-107">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="1f244-108">[Versionen auflisten][version-list]</span><span class="sxs-lookup"><span data-stu-id="1f244-108">[List versions][version-list]</span></span>      | `GET /drive/items/{item-id}/versions`  |
| <span data-ttu-id="1f244-109">[Version abrufen][version-get]</span><span class="sxs-lookup"><span data-stu-id="1f244-109">[Get version][version-get]</span></span>         | `GET /drive/items/{item-id}/versions/{version-id}`     |
| <span data-ttu-id="1f244-110">[Inhalte abrufen][content-get]</span><span class="sxs-lookup"><span data-stu-id="1f244-110">[Get contents][content-get]</span></span>        | `GET /drive/items/{item-id}/versions/{version-id}/content` |
| <span data-ttu-id="1f244-111">[Version wiederherstellen][version-restore]</span><span class="sxs-lookup"><span data-stu-id="1f244-111">[Restore version][version-restore]</span></span> | `POST /drive/items/{item-id}/versions/{version-id}/restore` |

[version-list]: ../api/driveitem-list-versions.md
[version-get]: ../api/driveitemversion-get.md
[content-get]: ../api/driveitemversion-get-contents.md
[version-restore]: ../api/driveitemversion-restore.md

<span data-ttu-id="1f244-112">Im Beispiel der vorstehenden Tabelle wird `/drive` verwendet, aber es gibt viele gültige Abfragen.</span><span class="sxs-lookup"><span data-stu-id="1f244-112">In the previous table, the examples use `/drive`, but there are many valid requests.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1f244-113">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1f244-113">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.driveItemVersion", "@type.aka": "oneDrive.driveItemVersion" } -->

```json
{
  "content": { "@odata.type": "Edm.Stream" },
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "publication": { "@odata.type": "microsoft.graph.publicationFacet" }
}
```

## <a name="properties"></a><span data-ttu-id="1f244-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1f244-114">Properties</span></span>

|      <span data-ttu-id="1f244-115">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="1f244-115">Property name</span></span>       |                         <span data-ttu-id="1f244-116">Typ</span><span class="sxs-lookup"><span data-stu-id="1f244-116">Type</span></span>                         |                               <span data-ttu-id="1f244-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1f244-117">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="1f244-118">**id**</span><span class="sxs-lookup"><span data-stu-id="1f244-118">**id**</span></span>                   | <span data-ttu-id="1f244-119">string</span><span class="sxs-lookup"><span data-stu-id="1f244-119">string</span></span>                                               | <span data-ttu-id="1f244-120">Die ID der Version.</span><span class="sxs-lookup"><span data-stu-id="1f244-120">The ID of the version.</span></span> <span data-ttu-id="1f244-121">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="1f244-121">Read-only.</span></span>                                       |
| <span data-ttu-id="1f244-122">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="1f244-122">**lastModifiedBy**</span></span>       | [<span data-ttu-id="1f244-123">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="1f244-123">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="1f244-124">Die Identität des Benutzers, der die Version zuletzt geändert hat.</span><span class="sxs-lookup"><span data-stu-id="1f244-124">Identity of the user which last modified the version.</span></span> <span data-ttu-id="1f244-125">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="1f244-125">Read-only.</span></span>        |
| <span data-ttu-id="1f244-126">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="1f244-126">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="1f244-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f244-127">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="1f244-128">Datum und Uhrzeit der letzten Änderung der Version.</span><span class="sxs-lookup"><span data-stu-id="1f244-128">Date and time the version was last modified.</span></span> <span data-ttu-id="1f244-129">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="1f244-129">Read-only.</span></span>                 |
| <span data-ttu-id="1f244-130">Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="1f244-130">**publication**</span></span>          | [<span data-ttu-id="1f244-131">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="1f244-131">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="1f244-132">Zeigt den Veröffentlichungsstatus dieser bestimmten Version an.</span><span class="sxs-lookup"><span data-stu-id="1f244-132">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="1f244-133">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="1f244-133">Read-only.</span></span> |
| <span data-ttu-id="1f244-134">**size**</span><span class="sxs-lookup"><span data-stu-id="1f244-134">**size**</span></span>                 | <span data-ttu-id="1f244-135">Int64</span><span class="sxs-lookup"><span data-stu-id="1f244-135">Int64</span></span>                                                | <span data-ttu-id="1f244-136">Gibt die Größe des Inhalt-Streams für diese Version des Elements an.</span><span class="sxs-lookup"><span data-stu-id="1f244-136">Indicates the size of the content stream for this version of the item.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="1f244-137">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="1f244-137">Relationships</span></span>

<span data-ttu-id="1f244-138">In der folgenden Tabelle werden die Beziehungen der **driveItemVersion**-Ressource zu anderen Ressourcen angegeben.</span><span class="sxs-lookup"><span data-stu-id="1f244-138">The following table defines the relationships that the **driveItemVersion** resource has to other resources.</span></span>

| <span data-ttu-id="1f244-139">Beziehungsname</span><span class="sxs-lookup"><span data-stu-id="1f244-139">Relationship name</span></span> |  <span data-ttu-id="1f244-140">Typ</span><span class="sxs-lookup"><span data-stu-id="1f244-140">Type</span></span>  |            <span data-ttu-id="1f244-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1f244-141">Description</span></span>             |
| :---------------- | :----- | :--------------------------------- |
| <span data-ttu-id="1f244-142">**content**</span><span class="sxs-lookup"><span data-stu-id="1f244-142">**content**</span></span>       | <span data-ttu-id="1f244-143">Stream</span><span class="sxs-lookup"><span data-stu-id="1f244-143">Stream</span></span> | <span data-ttu-id="1f244-144">Der Inhalt-Stream der Version.</span><span class="sxs-lookup"><span data-stu-id="1f244-144">The content stream of the version.</span></span> |

<!--
{
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version",
  "suppressions": [
    "Error: /api-reference/beta/resources/driveItemVersion.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
