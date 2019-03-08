---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: ListItem
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 435544db272b26e6fe3ac0e09803858eec9d05f6
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480880"
---
# <a name="listitem-resource"></a><span data-ttu-id="ce921-102">ListItem-Ressource</span><span class="sxs-lookup"><span data-stu-id="ce921-102">ListItem resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce921-103">Diese Ressource stellt ein Element in einer SharePoint-**[Liste][]** dar.</span><span class="sxs-lookup"><span data-stu-id="ce921-103">This resource represents an item in a SharePoint **[list][]**.</span></span>
<span data-ttu-id="ce921-104">Spaltenwerte in der Liste sind über das `fieldValueSet`-Wörterbuch verfügbar.</span><span class="sxs-lookup"><span data-stu-id="ce921-104">Column values in the list are available through the `fieldValueSet` dictionary.</span></span>

## <a name="tasks-on-a-listitem"></a><span data-ttu-id="ce921-105">Aufgaben zu einem listItem</span><span class="sxs-lookup"><span data-stu-id="ce921-105">Tasks on a listItem</span></span>

<span data-ttu-id="ce921-106">Die folgenden Aufgaben sind für **listItem**-Ressourcen verfügbar.</span><span class="sxs-lookup"><span data-stu-id="ce921-106">The following tasks are available for **listItem** resources.</span></span>
<span data-ttu-id="ce921-107">Alle Beispiele unten beziehen sich auf eine **[Liste][]**, z. B.: `https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}`.</span><span class="sxs-lookup"><span data-stu-id="ce921-107">All examples below are relative to a **[list][]**, eg: `https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}`.</span></span>

| <span data-ttu-id="ce921-108">Häufige Aufgaben</span><span class="sxs-lookup"><span data-stu-id="ce921-108">Common task</span></span>                    | <span data-ttu-id="ce921-109">HTTP-Methode</span><span class="sxs-lookup"><span data-stu-id="ce921-109">HTTP method</span></span>
|:-------------------------------|:------------------------
| <span data-ttu-id="ce921-110">[Get][]</span><span class="sxs-lookup"><span data-stu-id="ce921-110">[Get][]</span></span>                        | <span data-ttu-id="ce921-111">GET /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="ce921-111">GET /items/{item-id}</span></span>
| <span data-ttu-id="ce921-112">[Abrufen von Spaltenwerten][Get]</span><span class="sxs-lookup"><span data-stu-id="ce921-112">[Get column values][Get]</span></span>       | <span data-ttu-id="ce921-113">GET /items/{item-id}?expand=fields</span><span class="sxs-lookup"><span data-stu-id="ce921-113">GET /items/{item-id}?expand=fields</span></span>
| <span data-ttu-id="ce921-114">[Analysen abrufen][]</span><span class="sxs-lookup"><span data-stu-id="ce921-114">[Get analytics][]</span></span>              | <span data-ttu-id="ce921-115">/Items/{Item-ID}/Analytics abrufen</span><span class="sxs-lookup"><span data-stu-id="ce921-115">GET /items/{item-id}/analytics</span></span>
| <span data-ttu-id="ce921-116">[Aktivitäten nach Intervall abrufen][]</span><span class="sxs-lookup"><span data-stu-id="ce921-116">[Get activities by interval][]</span></span> | <span data-ttu-id="ce921-117">/Items/{item-id}/getActivitiesByInterval abrufen</span><span class="sxs-lookup"><span data-stu-id="ce921-117">GET /items/{item-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="ce921-118">[Create][]</span><span class="sxs-lookup"><span data-stu-id="ce921-118">[Create][]</span></span>                     | <span data-ttu-id="ce921-119">POST /items</span><span class="sxs-lookup"><span data-stu-id="ce921-119">POST /items</span></span>
| <span data-ttu-id="ce921-120">[Delete][]</span><span class="sxs-lookup"><span data-stu-id="ce921-120">[Delete][]</span></span>                     | <span data-ttu-id="ce921-121">DELETE /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="ce921-121">DELETE /items/{item-id}</span></span>
| <span data-ttu-id="ce921-122">[Update][]</span><span class="sxs-lookup"><span data-stu-id="ce921-122">[Update][]</span></span>                     | <span data-ttu-id="ce921-123">PATCH /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="ce921-123">PATCH /items/{item-id}</span></span>
| <span data-ttu-id="ce921-124">[Aktualisieren von Spaltenwerten][Update]</span><span class="sxs-lookup"><span data-stu-id="ce921-124">[Update column values][Update]</span></span> | <span data-ttu-id="ce921-125">PATCH /items/{item-id}/fields</span><span class="sxs-lookup"><span data-stu-id="ce921-125">PATCH /items/{item-id}/fields</span></span>

[Get]: ../api/listitem-get.md
[Analysen abrufen]: ../api/itemanalytics-get.md
[Get analytics]: ../api/itemanalytics-get.md
[Aktivitäten nach Intervall abrufen]: ../api/itemactivity-getbyinterval.md
[Get activities by interval]: ../api/itemactivity-getbyinterval.md
[Create]: ../api/listitem-create.md
[Delete]: ../api/listitem-delete.md
[Update]: ../api/listitem-update.md

## <a name="json-representation"></a><span data-ttu-id="ce921-132">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ce921-132">JSON representation</span></span>

<span data-ttu-id="ce921-133">Es folgt eine JSON-Darstellung einer **listItem**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="ce921-133">Here is a JSON representation of a **listItem** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="ce921-134">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ce921-134">Properties</span></span>

<span data-ttu-id="ce921-135">Die **listItem**-Ressource weist folgende Eigenschaften auf.</span><span class="sxs-lookup"><span data-stu-id="ce921-135">The **listItem** resource has the following properties.</span></span>

| <span data-ttu-id="ce921-136">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="ce921-136">Property name</span></span> | <span data-ttu-id="ce921-137">Typ</span><span class="sxs-lookup"><span data-stu-id="ce921-137">Type</span></span>                | <span data-ttu-id="ce921-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ce921-138">Description</span></span>
|:--------------|:--------------------|:-------------------------------
| <span data-ttu-id="ce921-139">contentType</span><span class="sxs-lookup"><span data-stu-id="ce921-139">contentType</span></span>   | <span data-ttu-id="ce921-140">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="ce921-140">[contentTypeInfo][]</span></span> | <span data-ttu-id="ce921-141">Der Inhaltstyp dieses Listenelements</span><span class="sxs-lookup"><span data-stu-id="ce921-141">The content type of this list item</span></span>

<span data-ttu-id="ce921-142">Die folgenden Eigenschaften werden von \*\* [baseItem][]\*\* geerbt.</span><span class="sxs-lookup"><span data-stu-id="ce921-142">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="ce921-143">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="ce921-143">Property name</span></span>        | <span data-ttu-id="ce921-144">Typ</span><span class="sxs-lookup"><span data-stu-id="ce921-144">Type</span></span>              | <span data-ttu-id="ce921-145">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ce921-145">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="ce921-146">id</span><span class="sxs-lookup"><span data-stu-id="ce921-146">id</span></span>                   | <span data-ttu-id="ce921-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ce921-147">string</span></span>            | <span data-ttu-id="ce921-p103">Der eindeutige Bezeichner des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ce921-p103">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="ce921-150">name</span><span class="sxs-lookup"><span data-stu-id="ce921-150">name</span></span>                 | <span data-ttu-id="ce921-151">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ce921-151">string</span></span>            | <span data-ttu-id="ce921-152">Der Name/Titel des Elements.</span><span class="sxs-lookup"><span data-stu-id="ce921-152">The name / title of the item.</span></span>
| <span data-ttu-id="ce921-153">createdBy</span><span class="sxs-lookup"><span data-stu-id="ce921-153">createdBy</span></span>            | <span data-ttu-id="ce921-154">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="ce921-154">[identitySet][]</span></span>   | <span data-ttu-id="ce921-155">Die Identität des Erstellers dieses Elements.</span><span class="sxs-lookup"><span data-stu-id="ce921-155">Identity of the creator of this item.</span></span> <span data-ttu-id="ce921-156">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ce921-156">Read-only.</span></span>
| <span data-ttu-id="ce921-157">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ce921-157">createdDateTime</span></span>      | <span data-ttu-id="ce921-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce921-158">DateTimeOffset</span></span>    | <span data-ttu-id="ce921-p105">Das Datum und die Uhrzeit der Erstellung des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ce921-p105">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="ce921-161">description</span><span class="sxs-lookup"><span data-stu-id="ce921-161">description</span></span>          | <span data-ttu-id="ce921-162">string</span><span class="sxs-lookup"><span data-stu-id="ce921-162">string</span></span>            | <span data-ttu-id="ce921-163">Der beschreibende Text für das Element.</span><span class="sxs-lookup"><span data-stu-id="ce921-163">The descriptive text for the item.</span></span>
| <span data-ttu-id="ce921-164">eTag</span><span class="sxs-lookup"><span data-stu-id="ce921-164">eTag</span></span>                 | <span data-ttu-id="ce921-165">string</span><span class="sxs-lookup"><span data-stu-id="ce921-165">string</span></span>            | <span data-ttu-id="ce921-p106">ETag für das Element. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ce921-p106">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="ce921-168">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="ce921-168">lastModifiedBy</span></span>       | <span data-ttu-id="ce921-169">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="ce921-169">[identitySet][]</span></span>   | <span data-ttu-id="ce921-170">Die Identität derPerson, die dieses Element zuletzt geändert hat.</span><span class="sxs-lookup"><span data-stu-id="ce921-170">Identity of the last modifier of this item.</span></span> <span data-ttu-id="ce921-171">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ce921-171">Read-only.</span></span>
| <span data-ttu-id="ce921-172">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ce921-172">lastModifiedDateTime</span></span> | <span data-ttu-id="ce921-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce921-173">DateTimeOffset</span></span>    | <span data-ttu-id="ce921-p108">Das Datum und die Uhrzeit der letzten Änderung des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ce921-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="ce921-176">parentReference</span><span class="sxs-lookup"><span data-stu-id="ce921-176">parentReference</span></span>      | <span data-ttu-id="ce921-177">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="ce921-177">[itemReference][]</span></span> | <span data-ttu-id="ce921-p109">Informationen zum übergeordneten Element, wenn das Element ein übergeordnetes Element hat. Lese-/Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="ce921-p109">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="ce921-180">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="ce921-180">sharepointIds</span></span>        | <span data-ttu-id="ce921-181">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="ce921-181">[sharepointIds][]</span></span> | <span data-ttu-id="ce921-p110">Gibt Bezeichner zurück, die für SharePoint REST-Kompatibilität nützlich sind. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ce921-p110">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="ce921-184">webUrl</span><span class="sxs-lookup"><span data-stu-id="ce921-184">webUrl</span></span>               | <span data-ttu-id="ce921-185">String (URL)</span><span class="sxs-lookup"><span data-stu-id="ce921-185">string (url)</span></span>      | <span data-ttu-id="ce921-p111">URL, über die das Element im Browser angezeigt werden kann. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ce921-p111">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="ce921-188">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ce921-188">Relationships</span></span>

 <span data-ttu-id="ce921-189">Die **listItem**-Ressource weist folgende Beziehungen zu anderen Ressourcen auf.</span><span class="sxs-lookup"><span data-stu-id="ce921-189">The **listItem** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="ce921-190">Beziehungsname</span><span class="sxs-lookup"><span data-stu-id="ce921-190">Relationship name</span></span> | <span data-ttu-id="ce921-191">Typ</span><span class="sxs-lookup"><span data-stu-id="ce921-191">Type</span></span>                           | <span data-ttu-id="ce921-192">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ce921-192">Description</span></span>
|:------------------|:-------------------------------|:-------------------------------
| <span data-ttu-id="ce921-193">Aktivitäten</span><span class="sxs-lookup"><span data-stu-id="ce921-193">activities</span></span>        | <span data-ttu-id="ce921-194">[ItemActivity][]-Sammlung</span><span class="sxs-lookup"><span data-stu-id="ce921-194">[itemActivity][] collection</span></span>    | <span data-ttu-id="ce921-195">Die Liste der letzten Aktivitäten, die für dieses Element durchgeführt wurden.</span><span class="sxs-lookup"><span data-stu-id="ce921-195">The list of recent activities that took place on this item.</span></span>
| <span data-ttu-id="ce921-196">Analyse</span><span class="sxs-lookup"><span data-stu-id="ce921-196">analytics</span></span>         | <span data-ttu-id="ce921-197">[itemAnalytics][]-Ressource</span><span class="sxs-lookup"><span data-stu-id="ce921-197">[itemAnalytics][] resource</span></span>     | <span data-ttu-id="ce921-198">Analysen zu den Ansichts Aktivitäten, die für dieses Element durchgeführt wurden.</span><span class="sxs-lookup"><span data-stu-id="ce921-198">Analytics about the view activities that took place on this item.</span></span>
| <span data-ttu-id="ce921-199">driveItem</span><span class="sxs-lookup"><span data-stu-id="ce921-199">driveItem</span></span>         | <span data-ttu-id="ce921-200">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="ce921-200">[driveItem][]</span></span>                  | <span data-ttu-id="ce921-201">Für Dokumentbibliotheken macht die **DriveItem** Beziehung das ListItem als \*\* [DriveItem][]\*\* verfügbar</span><span class="sxs-lookup"><span data-stu-id="ce921-201">For document libraries, the **driveItem** relationship exposes the listItem as a **[driveItem][]**</span></span>
| <span data-ttu-id="ce921-202">fields</span><span class="sxs-lookup"><span data-stu-id="ce921-202">fields</span></span>            | <span data-ttu-id="ce921-203">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="ce921-203">[fieldValueSet][]</span></span>              | <span data-ttu-id="ce921-204">Die Werte der für dieses Listenelement festgelegten Spalte.</span><span class="sxs-lookup"><span data-stu-id="ce921-204">The values of the columns set on this list item.</span></span>
| <span data-ttu-id="ce921-205">versions</span><span class="sxs-lookup"><span data-stu-id="ce921-205">versions</span></span>          | <span data-ttu-id="ce921-206">[listItemVersion][] -Sammlung</span><span class="sxs-lookup"><span data-stu-id="ce921-206">[listItemVersion][] collection</span></span> | <span data-ttu-id="ce921-207">Die Liste der vorherigen Versionen des Listenelements.</span><span class="sxs-lookup"><span data-stu-id="ce921-207">The list of previous versions of the list item.</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ListItem",
  "tocBookmarks": {
    "ListItem": "#"
  },
  "suppressions": [
    "Error: /api-reference/beta/resources/listitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
