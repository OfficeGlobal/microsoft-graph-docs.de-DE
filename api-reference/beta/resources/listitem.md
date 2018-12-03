---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ListItem
ms.openlocfilehash: 18ba74fd677c83da5f8bfe5d13303f7b18ed43f2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059849"
---
# <a name="listitem-resource"></a><span data-ttu-id="4d522-102">ListItem-Ressource</span><span class="sxs-lookup"><span data-stu-id="4d522-102">ListItem resource</span></span>

> <span data-ttu-id="4d522-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4d522-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4d522-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4d522-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4d522-105">Diese Ressource stellt ein Element in einer SharePoint-**[Liste][]** dar.</span><span class="sxs-lookup"><span data-stu-id="4d522-105">This resource represents an item in a SharePoint **[list][]**.</span></span>
<span data-ttu-id="4d522-106">Spaltenwerte in der Liste sind über das `fieldValueSet`-Wörterbuch verfügbar.</span><span class="sxs-lookup"><span data-stu-id="4d522-106">Column values in the list are available through the `fieldValueSet` dictionary.</span></span>

## <a name="tasks-on-a-listitem"></a><span data-ttu-id="4d522-107">Aufgaben zu einem listItem</span><span class="sxs-lookup"><span data-stu-id="4d522-107">Tasks on a listItem</span></span>

<span data-ttu-id="4d522-108">Die folgenden Aufgaben sind für **listItem**-Ressourcen verfügbar.</span><span class="sxs-lookup"><span data-stu-id="4d522-108">The following tasks are available for **listItem** resources.</span></span>
<span data-ttu-id="4d522-109">Alle Beispiele unten beziehen sich auf eine **[Liste][]**, z. B.: `https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}`.</span><span class="sxs-lookup"><span data-stu-id="4d522-109">All examples below are relative to a **[list][]**, eg: `https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}`.</span></span>

| <span data-ttu-id="4d522-110">Häufige Aufgaben</span><span class="sxs-lookup"><span data-stu-id="4d522-110">Common task</span></span>                    | <span data-ttu-id="4d522-111">HTTP-Methode</span><span class="sxs-lookup"><span data-stu-id="4d522-111">HTTP method</span></span>
|:-------------------------------|:------------------------
| <span data-ttu-id="4d522-112">[Get][]</span><span class="sxs-lookup"><span data-stu-id="4d522-112">[Get][]</span></span>                        | <span data-ttu-id="4d522-113">GET /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="4d522-113">GET /items/{item-id}</span></span>
| <span data-ttu-id="4d522-114">[Abrufen von Spaltenwerten][Get]</span><span class="sxs-lookup"><span data-stu-id="4d522-114">[Get column values][Get]</span></span>       | <span data-ttu-id="4d522-115">GET /items/{item-id}?expand=fields</span><span class="sxs-lookup"><span data-stu-id="4d522-115">GET /items/{item-id}?expand=fields</span></span>
| <span data-ttu-id="4d522-116">[Abrufen von analytics][]</span><span class="sxs-lookup"><span data-stu-id="4d522-116">[Get analytics][]</span></span>              | <span data-ttu-id="4d522-117">GET-/items/ {Element-Id} / Analytics</span><span class="sxs-lookup"><span data-stu-id="4d522-117">GET /items/{item-id}/analytics</span></span>
| <span data-ttu-id="4d522-118">[Abrufen von Aktivitäten nach Intervall][]</span><span class="sxs-lookup"><span data-stu-id="4d522-118">[Get activities by interval][]</span></span> | <span data-ttu-id="4d522-119">GET-/items/ {Element-Id} / GetActivitiesByInterval</span><span class="sxs-lookup"><span data-stu-id="4d522-119">GET /items/{item-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="4d522-120">[Create][]</span><span class="sxs-lookup"><span data-stu-id="4d522-120">[Create][]</span></span>                     | <span data-ttu-id="4d522-121">POST /items</span><span class="sxs-lookup"><span data-stu-id="4d522-121">POST /items</span></span>
| <span data-ttu-id="4d522-122">[Delete][]</span><span class="sxs-lookup"><span data-stu-id="4d522-122">[Delete][]</span></span>                     | <span data-ttu-id="4d522-123">DELETE /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="4d522-123">DELETE /items/{item-id}</span></span>
| <span data-ttu-id="4d522-124">[Update][]</span><span class="sxs-lookup"><span data-stu-id="4d522-124">[Update][]</span></span>                     | <span data-ttu-id="4d522-125">PATCH /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="4d522-125">PATCH /items/{item-id}</span></span>
| <span data-ttu-id="4d522-126">[Aktualisieren von Spaltenwerten][Update]</span><span class="sxs-lookup"><span data-stu-id="4d522-126">[Update column values][Update]</span></span> | <span data-ttu-id="4d522-127">PATCH /items/{item-id}/fields</span><span class="sxs-lookup"><span data-stu-id="4d522-127">PATCH /items/{item-id}/fields</span></span>

[Get]: ../api/listitem-get.md
[Abrufen von analytics]: ../api/itemanalytics-get.md
[Get analytics]: ../api/itemanalytics-get.md
[Abrufen von Aktivitäten nach Intervall]: ../api/itemactivity-getbyinterval.md
[Get activities by interval]: ../api/itemactivity-getbyinterval.md
[Create]: ../api/listitem-create.md
[Delete]: ../api/listitem-delete.md
[Update]: ../api/listitem-update.md

## <a name="json-representation"></a><span data-ttu-id="4d522-134">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4d522-134">JSON representation</span></span>

<span data-ttu-id="4d522-135">Es folgt eine JSON-Darstellung einer **listItem**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="4d522-135">Here is a JSON representation of a **listItem** resource.</span></span>

<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.listItem"
}-->

```json
{
  "contentType": { "@odata.type": "microsoft.graph.contentTypeInfo" },
  "fields": { "@odata.type": "microsoft.graph.fieldValueSet" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },

  /* relationships */
  "activities": [{"@odata.type": "microsoft.graph.itemActivity"}],
  "analytics": { "@odata.type": "microsoft.graph.itemAnalytics" },
  "driveItem": { "@odata.type": "microsoft.graph.driveItem" },
  "versions": [{"@odata.type": "microsoft.graph.listItemVersion"}],

  /* inherited from baseItem */
  "id": "string",
  "name": "name of resource",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "timestamp",
  "description": "description of resource",
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "timestamp",
  "parentReference": { "@odata.type": "microsoft.graph.itemReference"},
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="4d522-136">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4d522-136">Properties</span></span>

<span data-ttu-id="4d522-137">Die **listItem**-Ressource weist folgende Eigenschaften auf.</span><span class="sxs-lookup"><span data-stu-id="4d522-137">The **listItem** resource has the following properties.</span></span>

| <span data-ttu-id="4d522-138">Eigenschaftsname</span><span class="sxs-lookup"><span data-stu-id="4d522-138">Property name</span></span> | <span data-ttu-id="4d522-139">Typ</span><span class="sxs-lookup"><span data-stu-id="4d522-139">Type</span></span>                | <span data-ttu-id="4d522-140">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4d522-140">Description</span></span>
|:--------------|:--------------------|:-------------------------------
| <span data-ttu-id="4d522-141">contentType</span><span class="sxs-lookup"><span data-stu-id="4d522-141">contentType</span></span>   | <span data-ttu-id="4d522-142">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="4d522-142">[contentTypeInfo][]</span></span> | <span data-ttu-id="4d522-143">Der Inhaltstyp dieses Listenelements</span><span class="sxs-lookup"><span data-stu-id="4d522-143">The content type of this list item</span></span>

<span data-ttu-id="4d522-144">Die folgenden Eigenschaften werden von  **[baseItem][]** geerbt.</span><span class="sxs-lookup"><span data-stu-id="4d522-144">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="4d522-145">Eigenschaftsname</span><span class="sxs-lookup"><span data-stu-id="4d522-145">Property name</span></span>        | <span data-ttu-id="4d522-146">Typ</span><span class="sxs-lookup"><span data-stu-id="4d522-146">Type</span></span>              | <span data-ttu-id="4d522-147">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4d522-147">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="4d522-148">id</span><span class="sxs-lookup"><span data-stu-id="4d522-148">id</span></span>                   | <span data-ttu-id="4d522-149">string</span><span class="sxs-lookup"><span data-stu-id="4d522-149">string</span></span>            | <span data-ttu-id="4d522-p104">Der eindeutige Bezeichner des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="4d522-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="4d522-152">name</span><span class="sxs-lookup"><span data-stu-id="4d522-152">name</span></span>                 | <span data-ttu-id="4d522-153">string</span><span class="sxs-lookup"><span data-stu-id="4d522-153">string</span></span>            | <span data-ttu-id="4d522-154">Der Name/Titel des Elements.</span><span class="sxs-lookup"><span data-stu-id="4d522-154">The name / title of the item.</span></span>
| <span data-ttu-id="4d522-155">createdBy</span><span class="sxs-lookup"><span data-stu-id="4d522-155">createdBy</span></span>            | <span data-ttu-id="4d522-156">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="4d522-156">[identitySet][]</span></span>   | <span data-ttu-id="4d522-157">Die Identität des Erstellers dieses Elements.</span><span class="sxs-lookup"><span data-stu-id="4d522-157">Identity of the creator of this item.</span></span> <span data-ttu-id="4d522-158">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="4d522-158">Read-only.</span></span>
| <span data-ttu-id="4d522-159">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4d522-159">createdDateTime</span></span>      | <span data-ttu-id="4d522-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d522-160">DateTimeOffset</span></span>    | <span data-ttu-id="4d522-p106">Das Datum und die Uhrzeit der Erstellung des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="4d522-p106">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="4d522-163">description</span><span class="sxs-lookup"><span data-stu-id="4d522-163">description</span></span>          | <span data-ttu-id="4d522-164">string</span><span class="sxs-lookup"><span data-stu-id="4d522-164">string</span></span>            | <span data-ttu-id="4d522-165">Der beschreibende Text für das Element.</span><span class="sxs-lookup"><span data-stu-id="4d522-165">The descriptive text for the item.</span></span>
| <span data-ttu-id="4d522-166">eTag</span><span class="sxs-lookup"><span data-stu-id="4d522-166">eTag</span></span>                 | <span data-ttu-id="4d522-167">string</span><span class="sxs-lookup"><span data-stu-id="4d522-167">string</span></span>            | <span data-ttu-id="4d522-p107">ETag für das Element. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="4d522-p107">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="4d522-170">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="4d522-170">lastModifiedBy</span></span>       | <span data-ttu-id="4d522-171">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="4d522-171">[identitySet][]</span></span>   | <span data-ttu-id="4d522-172">Die Identität derPerson, die dieses Element zuletzt geändert hat.</span><span class="sxs-lookup"><span data-stu-id="4d522-172">Identity of the last modifier of this item.</span></span> <span data-ttu-id="4d522-173">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="4d522-173">Read-only.</span></span>
| <span data-ttu-id="4d522-174">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4d522-174">lastModifiedDateTime</span></span> | <span data-ttu-id="4d522-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d522-175">DateTimeOffset</span></span>    | <span data-ttu-id="4d522-p109">Das Datum und die Uhrzeit der letzten Änderung des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="4d522-p109">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="4d522-178">parentReference</span><span class="sxs-lookup"><span data-stu-id="4d522-178">parentReference</span></span>      | <span data-ttu-id="4d522-179">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="4d522-179">[itemReference][]</span></span> | <span data-ttu-id="4d522-p110">Informationen zum übergeordneten Element, wenn das Element ein übergeordnetes Element hat. Lese-/Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="4d522-p110">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="4d522-182">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="4d522-182">sharepointIds</span></span>        | <span data-ttu-id="4d522-183">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="4d522-183">[sharepointIds][]</span></span> | <span data-ttu-id="4d522-p111">Gibt Bezeichner zurück, die für SharePoint REST-Kompatibilität nützlich sind. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="4d522-p111">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="4d522-186">webUrl</span><span class="sxs-lookup"><span data-stu-id="4d522-186">webUrl</span></span>               | <span data-ttu-id="4d522-187">String (URL)</span><span class="sxs-lookup"><span data-stu-id="4d522-187">string (url)</span></span>      | <span data-ttu-id="4d522-p112">URL, über die das Element im Browser angezeigt werden kann. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="4d522-p112">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="4d522-190">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="4d522-190">Relationships</span></span>

 <span data-ttu-id="4d522-191">Die **listItem**-Ressource weist folgende Beziehungen zu anderen Ressourcen auf.</span><span class="sxs-lookup"><span data-stu-id="4d522-191">The **listItem** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="4d522-192">Beziehungsname</span><span class="sxs-lookup"><span data-stu-id="4d522-192">Relationship name</span></span> | <span data-ttu-id="4d522-193">Typ</span><span class="sxs-lookup"><span data-stu-id="4d522-193">Type</span></span>                           | <span data-ttu-id="4d522-194">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4d522-194">Description</span></span>
|:------------------|:-------------------------------|:-------------------------------
| <span data-ttu-id="4d522-195">Aktivitäten</span><span class="sxs-lookup"><span data-stu-id="4d522-195">activities</span></span>        | <span data-ttu-id="4d522-196">[ItemActivity][]-Sammlung</span><span class="sxs-lookup"><span data-stu-id="4d522-196">[itemActivity][] collection</span></span>    | <span data-ttu-id="4d522-197">Die Liste der letzten Aktivitäten, die für dieses Element durchgeführt wurden.</span><span class="sxs-lookup"><span data-stu-id="4d522-197">The list of recent activities that took place on this item.</span></span>
| <span data-ttu-id="4d522-198">Analytics</span><span class="sxs-lookup"><span data-stu-id="4d522-198">analytics</span></span>         | <span data-ttu-id="4d522-199">[ItemAnalytics][] -Ressource</span><span class="sxs-lookup"><span data-stu-id="4d522-199">[itemAnalytics][] resource</span></span>     | <span data-ttu-id="4d522-200">Analytics über die Aktivitäten anzeigen, die für dieses Element ausgeführt wurden.</span><span class="sxs-lookup"><span data-stu-id="4d522-200">Analytics about the view activities that took place on this item.</span></span>
| <span data-ttu-id="4d522-201">driveItem</span><span class="sxs-lookup"><span data-stu-id="4d522-201">driveItem</span></span>         | <span data-ttu-id="4d522-202">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="4d522-202">[driveItem][]</span></span>                  | <span data-ttu-id="4d522-203">Für Dokumentbibliotheken macht die **DriveItem** Beziehung das ListItem als \*\* [DriveItem][]\*\* verfügbar</span><span class="sxs-lookup"><span data-stu-id="4d522-203">For document libraries, the **driveItem** relationship exposes the listItem as a **[driveItem][]**</span></span>
| <span data-ttu-id="4d522-204">fields</span><span class="sxs-lookup"><span data-stu-id="4d522-204">fields</span></span>            | <span data-ttu-id="4d522-205">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="4d522-205">[fieldValueSet][]</span></span>              | <span data-ttu-id="4d522-206">Die Werte der für dieses Listenelement festgelegten Spalte.</span><span class="sxs-lookup"><span data-stu-id="4d522-206">The values of the columns set on this list item.</span></span>
| <span data-ttu-id="4d522-207">Versionen</span><span class="sxs-lookup"><span data-stu-id="4d522-207">versions</span></span>          | <span data-ttu-id="4d522-208">[ListItemVersion][] -Auflistung</span><span class="sxs-lookup"><span data-stu-id="4d522-208">[listItemVersion][] collection</span></span> | <span data-ttu-id="4d522-209">Die Liste der vorherigen Versionen des Listenelements.</span><span class="sxs-lookup"><span data-stu-id="4d522-209">The list of previous versions of the list item.</span></span>

[baseItem]: baseitem.md
[contentTypeInfo]: contenttypeinfo.md
[driveItem]: driveitem.md
[fieldValueSet]: fieldvalueset.md
[identitySet]: identityset.md
[itemActivity]: itemactivity.md
[itemAnalytics]: itemanalytics.md
[itemReference]: itemreference.md
[list]: list.md
[listItemVersion]: listitemversion.md
[sharepointIds]: sharepointids.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ListItem",
  "tocBookmarks": {
    "ListItem": "#"
  }
} -->
