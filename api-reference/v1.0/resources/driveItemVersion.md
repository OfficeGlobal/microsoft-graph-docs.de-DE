---
title: DriveItemVersion-Ressourcentyp
description: Die Ressource **DriveItemVersion** stellt eine bestimmte Version von einer DriveItem dar.
ms.openlocfilehash: e257e800b0ac8ad4d94027f9c8040ffb3b20ea90
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017655"
---
# <a name="driveitemversion-resource-type"></a><span data-ttu-id="75079-103">DriveItemVersion-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="75079-103">DriveItemVersion resource type</span></span>

<span data-ttu-id="75079-104">Die **DriveItemVersion**-Ressource stellt eine bestimmte Version eines [DriveItem](driveitem.md) dar.</span><span class="sxs-lookup"><span data-stu-id="75079-104">The **DriveItemVersion** resource represents a specific version of a [DriveItem](driveitem.md).</span></span>


## <a name="tasks-on-driveitemversion-resources"></a><span data-ttu-id="75079-105">Aufgaben für DriveItemVersion-Ressourcen</span><span class="sxs-lookup"><span data-stu-id="75079-105">Tasks on DriveItemVersion resources</span></span>

<span data-ttu-id="75079-106">Die folgenden Aufgaben sind für driveItemVersion-Ressourcen verfügbar.</span><span class="sxs-lookup"><span data-stu-id="75079-106">The following tasks are available for driveItemVersion resources.</span></span>

|            <span data-ttu-id="75079-107">Häufige Aufgaben</span><span class="sxs-lookup"><span data-stu-id="75079-107">Common task</span></span>             |         <span data-ttu-id="75079-108">HTTP-Methode</span><span class="sxs-lookup"><span data-stu-id="75079-108">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="75079-109">[Versionen auflisten][version-list]</span><span class="sxs-lookup"><span data-stu-id="75079-109">[List versions][version-list]</span></span>      | `GET /drive/items/{item-id}/versions`  |
| <span data-ttu-id="75079-110">[Version abrufen][version-get]</span><span class="sxs-lookup"><span data-stu-id="75079-110">[Get version][version-get]</span></span>         | `GET /drive/items/{item-id}/versions/{version-id}`     |
| <span data-ttu-id="75079-111">[Inhalte abrufen][content-get]</span><span class="sxs-lookup"><span data-stu-id="75079-111">[Get contents][content-get]</span></span>        | `GET /drive/items/{item-id}/versions/{version-id}/content` |
| <span data-ttu-id="75079-112">[Version wiederherstellen][version-restore]</span><span class="sxs-lookup"><span data-stu-id="75079-112">[Restore version][version-restore]</span></span> | `POST /drive/items/{item-id}/versions/{version-id}/restore` |

[version-list]: ../api/driveitem-list-versions.md
[version-get]: ../api/driveitemversion-get.md
[content-get]: ../api/driveitemversion-get-contents.md
[version-restore]: ../api/driveitemversion-restore.md

<span data-ttu-id="75079-113">Im Beispiel der vorstehenden Tabelle wird `/drive` verwendet, aber es gibt viele gültige Abfragen.</span><span class="sxs-lookup"><span data-stu-id="75079-113">In the previous table, the examples use `/drive`, but there are many valid requests.</span></span>

## <a name="json-representation"></a><span data-ttu-id="75079-114">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="75079-114">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="75079-115">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="75079-115">Properties</span></span>

|      <span data-ttu-id="75079-116">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="75079-116">Property name</span></span>       |                         <span data-ttu-id="75079-117">Typ</span><span class="sxs-lookup"><span data-stu-id="75079-117">Type</span></span>                         |                               <span data-ttu-id="75079-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="75079-118">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="75079-119">**id**</span><span class="sxs-lookup"><span data-stu-id="75079-119">**id**</span></span>                   | <span data-ttu-id="75079-120">string</span><span class="sxs-lookup"><span data-stu-id="75079-120">string</span></span>                                               | <span data-ttu-id="75079-121">Die ID der Version.</span><span class="sxs-lookup"><span data-stu-id="75079-121">The ID of the version.</span></span> <span data-ttu-id="75079-122">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="75079-122">Read-only.</span></span>                                       |
| <span data-ttu-id="75079-123">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="75079-123">**lastModifiedBy**</span></span>       | [<span data-ttu-id="75079-124">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="75079-124">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="75079-125">Die Identität des Benutzers, der die Version zuletzt geändert hat.</span><span class="sxs-lookup"><span data-stu-id="75079-125">Identity of the user which last modified the version.</span></span> <span data-ttu-id="75079-126">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="75079-126">Read-only.</span></span>        |
| <span data-ttu-id="75079-127">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="75079-127">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="75079-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75079-128">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="75079-129">Datum und Uhrzeit der letzten Änderung der Version.</span><span class="sxs-lookup"><span data-stu-id="75079-129">Date and time the version was last modified.</span></span> <span data-ttu-id="75079-130">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="75079-130">Read-only.</span></span>                 |
| <span data-ttu-id="75079-131">**Veröffentlichung**</span><span class="sxs-lookup"><span data-stu-id="75079-131">**publication**</span></span>          | [<span data-ttu-id="75079-132">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="75079-132">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="75079-133">Zeigt den Veröffentlichungsstatus dieser bestimmten Version an.</span><span class="sxs-lookup"><span data-stu-id="75079-133">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="75079-134">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="75079-134">Read-only.</span></span> |
| <span data-ttu-id="75079-135">**size**</span><span class="sxs-lookup"><span data-stu-id="75079-135">**size**</span></span>                 | <span data-ttu-id="75079-136">Int64</span><span class="sxs-lookup"><span data-stu-id="75079-136">Int64</span></span>                                                | <span data-ttu-id="75079-137">Gibt die Größe des Inhalt-Streams für diese Version des Elements an.</span><span class="sxs-lookup"><span data-stu-id="75079-137">Indicates the size of the content stream for this version of the item.</span></span>  |
| <span data-ttu-id="75079-138">**content**</span><span class="sxs-lookup"><span data-stu-id="75079-138">**content**</span></span>              | <span data-ttu-id="75079-139">Stream</span><span class="sxs-lookup"><span data-stu-id="75079-139">Stream</span></span>                                               | <span data-ttu-id="75079-140">Der Inhaltsstream für diese Version des Elements.</span><span class="sxs-lookup"><span data-stu-id="75079-140">The content stream for this version of the item.</span></span>                        |

<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
