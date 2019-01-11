---
author: rgregg
ms.author: rgregg
ms.date: 09/17/2017
title: DriveItemVersion
localization_priority: Normal
ms.openlocfilehash: 4267a82cc2dee7f0b9b301e13073f32cf95c6844
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841741"
---
# <a name="driveitemversion-resource-type"></a><span data-ttu-id="6c041-102">DriveItemVersion-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6c041-102">DriveItemVersion resource type</span></span>

> <span data-ttu-id="6c041-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6c041-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6c041-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6c041-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6c041-105">Die **DriveItemVersion**-Ressource stellt eine bestimmte Version eines [DriveItem](driveitem.md) dar.</span><span class="sxs-lookup"><span data-stu-id="6c041-105">The **DriveItemVersion** resource represents a specific version of a [DriveItem](driveitem.md).</span></span>


## <a name="tasks-on-driveitemversion-resources"></a><span data-ttu-id="6c041-106">Aufgaben für DriveItemVersion-Ressourcen</span><span class="sxs-lookup"><span data-stu-id="6c041-106">Tasks on DriveItemVersion resources</span></span>

<span data-ttu-id="6c041-107">Die folgenden Aufgaben sind für driveItemVersion-Ressourcen verfügbar.</span><span class="sxs-lookup"><span data-stu-id="6c041-107">The following tasks are available for driveItemVersion resources.</span></span>

|            <span data-ttu-id="6c041-108">Häufige Aufgaben</span><span class="sxs-lookup"><span data-stu-id="6c041-108">Common task</span></span>             |         <span data-ttu-id="6c041-109">HTTP-Methode</span><span class="sxs-lookup"><span data-stu-id="6c041-109">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="6c041-110">[Versionen auflisten][version-list]</span><span class="sxs-lookup"><span data-stu-id="6c041-110">[List versions][version-list]</span></span>      | `GET /drive/items/{item-id}/versions`  |
| <span data-ttu-id="6c041-111">[Version abrufen][version-get]</span><span class="sxs-lookup"><span data-stu-id="6c041-111">[Get version][version-get]</span></span>         | `GET /drive/items/{item-id}/versions/{version-id}`     |
| <span data-ttu-id="6c041-112">[Inhalte abrufen][content-get]</span><span class="sxs-lookup"><span data-stu-id="6c041-112">[Get contents][content-get]</span></span>        | `GET /drive/items/{item-id}/versions/{version-id}/content` |
| <span data-ttu-id="6c041-113">[Version wiederherstellen][version-restore]</span><span class="sxs-lookup"><span data-stu-id="6c041-113">[Restore version][version-restore]</span></span> | `POST /drive/items/{item-id}/versions/{version-id}/restore` |

[version-list]: ../api/driveitem-list-versions.md
[version-get]: ../api/driveitemversion-get.md
[content-get]: ../api/driveitemversion-get-contents.md
[version-restore]: ../api/driveitemversion-restore.md

<span data-ttu-id="6c041-114">Im Beispiel der vorstehenden Tabelle wird `/drive` verwendet, aber es gibt viele gültige Abfragen.</span><span class="sxs-lookup"><span data-stu-id="6c041-114">In the previous table, the examples use `/drive`, but there are many valid requests.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6c041-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6c041-115">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="6c041-116">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6c041-116">Properties</span></span>

|      <span data-ttu-id="6c041-117">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="6c041-117">Property name</span></span>       |                         <span data-ttu-id="6c041-118">Typ</span><span class="sxs-lookup"><span data-stu-id="6c041-118">Type</span></span>                         |                               <span data-ttu-id="6c041-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6c041-119">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="6c041-120">**id**</span><span class="sxs-lookup"><span data-stu-id="6c041-120">**id**</span></span>                   | <span data-ttu-id="6c041-121">string</span><span class="sxs-lookup"><span data-stu-id="6c041-121">string</span></span>                                               | <span data-ttu-id="6c041-122">Die ID der Version.</span><span class="sxs-lookup"><span data-stu-id="6c041-122">The ID of the version.</span></span> <span data-ttu-id="6c041-123">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="6c041-123">Read-only.</span></span>                                       |
| <span data-ttu-id="6c041-124">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="6c041-124">**lastModifiedBy**</span></span>       | [<span data-ttu-id="6c041-125">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="6c041-125">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="6c041-126">Die Identität des Benutzers, der die Version zuletzt geändert hat.</span><span class="sxs-lookup"><span data-stu-id="6c041-126">Identity of the user which last modified the version.</span></span> <span data-ttu-id="6c041-127">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="6c041-127">Read-only.</span></span>        |
| <span data-ttu-id="6c041-128">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="6c041-128">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="6c041-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c041-129">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="6c041-130">Datum und Uhrzeit der letzten Änderung der Version.</span><span class="sxs-lookup"><span data-stu-id="6c041-130">Date and time the version was last modified.</span></span> <span data-ttu-id="6c041-131">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="6c041-131">Read-only.</span></span>                 |
| <span data-ttu-id="6c041-132">**Veröffentlichung**</span><span class="sxs-lookup"><span data-stu-id="6c041-132">**publication**</span></span>          | [<span data-ttu-id="6c041-133">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="6c041-133">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="6c041-134">Zeigt den Veröffentlichungsstatus dieser bestimmten Version an.</span><span class="sxs-lookup"><span data-stu-id="6c041-134">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="6c041-135">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="6c041-135">Read-only.</span></span> |
| <span data-ttu-id="6c041-136">**size**</span><span class="sxs-lookup"><span data-stu-id="6c041-136">**size**</span></span>                 | <span data-ttu-id="6c041-137">Int64</span><span class="sxs-lookup"><span data-stu-id="6c041-137">Int64</span></span>                                                | <span data-ttu-id="6c041-138">Gibt die Größe des Inhalt-Streams für diese Version des Elements an.</span><span class="sxs-lookup"><span data-stu-id="6c041-138">Indicates the size of the content stream for this version of the item.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="6c041-139">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6c041-139">Relationships</span></span>

<span data-ttu-id="6c041-140">In der folgenden Tabelle werden die Beziehungen der **driveItemVersion**-Ressource zu anderen Ressourcen angegeben.</span><span class="sxs-lookup"><span data-stu-id="6c041-140">The following table defines the relationships that the **driveItemVersion** resource has to other resources.</span></span>

| <span data-ttu-id="6c041-141">Beziehungsname</span><span class="sxs-lookup"><span data-stu-id="6c041-141">Relationship name</span></span> |  <span data-ttu-id="6c041-142">Typ</span><span class="sxs-lookup"><span data-stu-id="6c041-142">Type</span></span>  |            <span data-ttu-id="6c041-143">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6c041-143">Description</span></span>             |
| :---------------- | :----- | :--------------------------------- |
| <span data-ttu-id="6c041-144">**content**</span><span class="sxs-lookup"><span data-stu-id="6c041-144">**content**</span></span>       | <span data-ttu-id="6c041-145">Stream</span><span class="sxs-lookup"><span data-stu-id="6c041-145">Stream</span></span> | <span data-ttu-id="6c041-146">Der Inhalt-Stream der Version.</span><span class="sxs-lookup"><span data-stu-id="6c041-146">The content stream of the version.</span></span> |

<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
