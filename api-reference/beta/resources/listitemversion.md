---
author: rgregg
ms.author: rgregg
ms.date: 09/17/2017
title: ListItemVersion
localization_priority: Normal
ms.openlocfilehash: 0ffdda98d941ef197bd956146ba796ace037cb8f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849623"
---
# <a name="listitemversion-resource-type"></a><span data-ttu-id="2ddb6-102">ListItemVersion-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="2ddb6-102">ListItemVersion resource type</span></span>

> <span data-ttu-id="2ddb6-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2ddb6-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2ddb6-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2ddb6-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2ddb6-105">Die **ListItemVersion**-Ressource stellt eine frühere Version der [ListItem](listitem.md)-Ressource dar.</span><span class="sxs-lookup"><span data-stu-id="2ddb6-105">The **listItemVersion** resource represents a previous version of a [ListItem](listitem.md) resource.</span></span>

## <a name="tasks-on-listitemversion-resources"></a><span data-ttu-id="2ddb6-106">Aufgaben für ListItemVersion-Ressourcen</span><span class="sxs-lookup"><span data-stu-id="2ddb6-106">Tasks on ListItemVersion resources</span></span>

<span data-ttu-id="2ddb6-107">Die folgenden Aufgaben sind für listItemVersion-Ressourcen verfügbar.</span><span class="sxs-lookup"><span data-stu-id="2ddb6-107">The following tasks are available for listItemVersion resources.</span></span>

|            <span data-ttu-id="2ddb6-108">Häufige Aufgaben</span><span class="sxs-lookup"><span data-stu-id="2ddb6-108">Common task</span></span>             |         <span data-ttu-id="2ddb6-109">HTTP-Methode</span><span class="sxs-lookup"><span data-stu-id="2ddb6-109">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="2ddb6-110">[Versionen auflisten][version-list]</span><span class="sxs-lookup"><span data-stu-id="2ddb6-110">[List versions][version-list]</span></span>      | `GET /sites/{site-id}/items/{item-id}/versions`  |
| <span data-ttu-id="2ddb6-111">[Version abrufen][version-get]</span><span class="sxs-lookup"><span data-stu-id="2ddb6-111">[Get version][version-get]</span></span>         | `GET /sites/{site-id}/items/versions/{version-id}`     |
| <span data-ttu-id="2ddb6-112">[Version wiederherstellen][version-restore]</span><span class="sxs-lookup"><span data-stu-id="2ddb6-112">[Restore version][version-restore]</span></span> | `POST /sites/{site-id}/items/versions/{version-id}/restore` |

[version-list]: ../api/listitem-list-versions.md
[version-get]: ../api/listitemversion-get.md
[version-restore]: ../api/listitemversion-restore.md


## <a name="json-representation"></a><span data-ttu-id="2ddb6-113">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2ddb6-113">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="2ddb6-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2ddb6-114">Properties</span></span>

|      <span data-ttu-id="2ddb6-115">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="2ddb6-115">Property name</span></span>       |                         <span data-ttu-id="2ddb6-116">Typ</span><span class="sxs-lookup"><span data-stu-id="2ddb6-116">Type</span></span>                         |                               <span data-ttu-id="2ddb6-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2ddb6-117">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="2ddb6-118">**id**</span><span class="sxs-lookup"><span data-stu-id="2ddb6-118">**id**</span></span>                   | <span data-ttu-id="2ddb6-119">string</span><span class="sxs-lookup"><span data-stu-id="2ddb6-119">string</span></span>                                               | <span data-ttu-id="2ddb6-120">Die ID der Version.</span><span class="sxs-lookup"><span data-stu-id="2ddb6-120">The ID of the version.</span></span> <span data-ttu-id="2ddb6-121">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2ddb6-121">Read-only.</span></span>                                       |
| <span data-ttu-id="2ddb6-122">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="2ddb6-122">**lastModifiedBy**</span></span>       | [<span data-ttu-id="2ddb6-123">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="2ddb6-123">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="2ddb6-124">Die Identität des Benutzers, der die Version zuletzt geändert hat.</span><span class="sxs-lookup"><span data-stu-id="2ddb6-124">Identity of the user which last modified the version.</span></span> <span data-ttu-id="2ddb6-125">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2ddb6-125">Read-only.</span></span>        |
| <span data-ttu-id="2ddb6-126">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="2ddb6-126">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="2ddb6-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ddb6-127">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="2ddb6-128">Datum und Uhrzeit der letzten Änderung der Version.</span><span class="sxs-lookup"><span data-stu-id="2ddb6-128">Date and time the version was last modified.</span></span> <span data-ttu-id="2ddb6-129">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2ddb6-129">Read-only.</span></span>                 |
| <span data-ttu-id="2ddb6-130">**published**</span><span class="sxs-lookup"><span data-stu-id="2ddb6-130">**published**</span></span>            | [<span data-ttu-id="2ddb6-131">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="2ddb6-131">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="2ddb6-132">Zeigt den Veröffentlichungsstatus dieser bestimmten Version an.</span><span class="sxs-lookup"><span data-stu-id="2ddb6-132">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="2ddb6-133">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2ddb6-133">Read-only.</span></span> |


## <a name="relationships"></a><span data-ttu-id="2ddb6-134">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="2ddb6-134">Relationships</span></span>

<span data-ttu-id="2ddb6-135">In der folgenden Tabelle werden die Beziehungen der **driveItemVersion**-Ressource zu anderen Ressourcen angegeben.</span><span class="sxs-lookup"><span data-stu-id="2ddb6-135">The following table defines the relationships that the **driveItemVersion** resource has to other resources.</span></span>

| <span data-ttu-id="2ddb6-136">Beziehungsname</span><span class="sxs-lookup"><span data-stu-id="2ddb6-136">Relationship name</span></span> |                      <span data-ttu-id="2ddb6-137">Typ</span><span class="sxs-lookup"><span data-stu-id="2ddb6-137">Type</span></span>                      |                               <span data-ttu-id="2ddb6-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2ddb6-138">Description</span></span>                                |
| :---------------- | :--------------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="2ddb6-139">**fields**</span><span class="sxs-lookup"><span data-stu-id="2ddb6-139">**fields**</span></span>        | [<span data-ttu-id="2ddb6-140">fieldValueSet</span><span class="sxs-lookup"><span data-stu-id="2ddb6-140">FieldValueSet</span></span>](../resources/fieldvalueset.md) | <span data-ttu-id="2ddb6-141">Eine Auflistung der Felder und Werte für diese Version des Listenelements.</span><span class="sxs-lookup"><span data-stu-id="2ddb6-141">A collection of the fields and values for this version of the list item.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
