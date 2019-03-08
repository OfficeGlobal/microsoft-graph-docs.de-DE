---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: ListItem
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: ba4b910f6d86caee23ce191b225d040ef023b4e7
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481615"
---
# <a name="listitem-resource"></a><span data-ttu-id="f3ff5-102">ListItem-Ressource</span><span class="sxs-lookup"><span data-stu-id="f3ff5-102">ListItem resource</span></span>

<span data-ttu-id="f3ff5-103">Diese Ressource stellt ein Element in einer SharePoint-**[Liste][]** dar.</span><span class="sxs-lookup"><span data-stu-id="f3ff5-103">This resource represents an item in a SharePoint **[list][]**.</span></span>
<span data-ttu-id="f3ff5-104">Spaltenwerte in der Liste sind über das `fieldValueSet`-Wörterbuch verfügbar.</span><span class="sxs-lookup"><span data-stu-id="f3ff5-104">Column values in the list are available through the `fieldValueSet` dictionary.</span></span>

## <a name="tasks-on-a-listitem"></a><span data-ttu-id="f3ff5-105">Aufgaben zu einem listItem</span><span class="sxs-lookup"><span data-stu-id="f3ff5-105">Tasks on a listItem</span></span>

<span data-ttu-id="f3ff5-106">Die folgenden Aufgaben sind für **listItem**-Ressourcen verfügbar.</span><span class="sxs-lookup"><span data-stu-id="f3ff5-106">The following tasks are available for **listItem** resources.</span></span>
<span data-ttu-id="f3ff5-107">Alle Beispiele unten beziehen sich auf eine **[Liste][]**, z. B.: `https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}`.</span><span class="sxs-lookup"><span data-stu-id="f3ff5-107">All examples below are relative to a **[list][]**, eg: `https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}`.</span></span>

| <span data-ttu-id="f3ff5-108">Häufige Aufgaben</span><span class="sxs-lookup"><span data-stu-id="f3ff5-108">Common task</span></span>                    | <span data-ttu-id="f3ff5-109">HTTP-Methode</span><span class="sxs-lookup"><span data-stu-id="f3ff5-109">HTTP method</span></span>
|:-------------------------------|:------------------------
| <span data-ttu-id="f3ff5-110">[Get][]</span><span class="sxs-lookup"><span data-stu-id="f3ff5-110">[Get][]</span></span>                        | <span data-ttu-id="f3ff5-111">GET /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="f3ff5-111">GET /items/{item-id}</span></span>
| <span data-ttu-id="f3ff5-112">[Abrufen von Spaltenwerten][Get]</span><span class="sxs-lookup"><span data-stu-id="f3ff5-112">[Get column values][Get]</span></span>       | <span data-ttu-id="f3ff5-113">GET /items/{item-id}?expand=fields</span><span class="sxs-lookup"><span data-stu-id="f3ff5-113">GET /items/{item-id}?expand=fields</span></span>
| <span data-ttu-id="f3ff5-114">[Create][]</span><span class="sxs-lookup"><span data-stu-id="f3ff5-114">[Create][]</span></span>                     | <span data-ttu-id="f3ff5-115">POST /items</span><span class="sxs-lookup"><span data-stu-id="f3ff5-115">POST /items</span></span>
| <span data-ttu-id="f3ff5-116">[Delete][]</span><span class="sxs-lookup"><span data-stu-id="f3ff5-116">[Delete][]</span></span>                     | <span data-ttu-id="f3ff5-117">DELETE /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="f3ff5-117">DELETE /items/{item-id}</span></span>
| <span data-ttu-id="f3ff5-118">[Update][]</span><span class="sxs-lookup"><span data-stu-id="f3ff5-118">[Update][]</span></span>                     | <span data-ttu-id="f3ff5-119">PATCH /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="f3ff5-119">PATCH /items/{item-id}</span></span>
| <span data-ttu-id="f3ff5-120">[Aktualisieren von Spaltenwerten][Update]</span><span class="sxs-lookup"><span data-stu-id="f3ff5-120">[Update column values][Update]</span></span> | <span data-ttu-id="f3ff5-121">PATCH /items/{item-id}/fields</span><span class="sxs-lookup"><span data-stu-id="f3ff5-121">PATCH /items/{item-id}/fields</span></span>

[Get]: ../api/listitem-get.md
[Create]: ../api/listitem-create.md
[Löschen]: ../api/listitem-delete.md
[Delete]: ../api/listitem-delete.md
[Update]: ../api/listitem-update.md

## <a name="json-representation"></a><span data-ttu-id="f3ff5-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f3ff5-126">JSON representation</span></span>

<span data-ttu-id="f3ff5-127">Es folgt eine JSON-Darstellung einer **listItem**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="f3ff5-127">Here is a JSON representation of a **listItem** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="f3ff5-128">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f3ff5-128">Properties</span></span>

<span data-ttu-id="f3ff5-129">Die **listItem**-Ressource weist folgende Eigenschaften auf.</span><span class="sxs-lookup"><span data-stu-id="f3ff5-129">The **listItem** resource has the following properties.</span></span>

| <span data-ttu-id="f3ff5-130">Eigenschaftsname</span><span class="sxs-lookup"><span data-stu-id="f3ff5-130">Property name</span></span> | <span data-ttu-id="f3ff5-131">Typ</span><span class="sxs-lookup"><span data-stu-id="f3ff5-131">Type</span></span>                | <span data-ttu-id="f3ff5-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f3ff5-132">Description</span></span>
|:--------------|:--------------------|:-------------------------------
| <span data-ttu-id="f3ff5-133">contentType</span><span class="sxs-lookup"><span data-stu-id="f3ff5-133">contentType</span></span>   | <span data-ttu-id="f3ff5-134">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="f3ff5-134">[contentTypeInfo][]</span></span> | <span data-ttu-id="f3ff5-135">Der Inhaltstyp dieses Listenelements</span><span class="sxs-lookup"><span data-stu-id="f3ff5-135">The content type of this list item</span></span>

<span data-ttu-id="f3ff5-136">Die folgenden Eigenschaften werden von  **[baseItem][]** geerbt.</span><span class="sxs-lookup"><span data-stu-id="f3ff5-136">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="f3ff5-137">Eigenschaftsname</span><span class="sxs-lookup"><span data-stu-id="f3ff5-137">Property name</span></span>        | <span data-ttu-id="f3ff5-138">Typ</span><span class="sxs-lookup"><span data-stu-id="f3ff5-138">Type</span></span>              | <span data-ttu-id="f3ff5-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f3ff5-139">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="f3ff5-140">id</span><span class="sxs-lookup"><span data-stu-id="f3ff5-140">id</span></span>                   | <span data-ttu-id="f3ff5-141">string</span><span class="sxs-lookup"><span data-stu-id="f3ff5-141">string</span></span>            | <span data-ttu-id="f3ff5-p103">Der eindeutige Bezeichner des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f3ff5-p103">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="f3ff5-144">name</span><span class="sxs-lookup"><span data-stu-id="f3ff5-144">name</span></span>                 | <span data-ttu-id="f3ff5-145">string</span><span class="sxs-lookup"><span data-stu-id="f3ff5-145">string</span></span>            | <span data-ttu-id="f3ff5-146">Der Name/Titel des Elements.</span><span class="sxs-lookup"><span data-stu-id="f3ff5-146">The name / title of the item.</span></span>
| <span data-ttu-id="f3ff5-147">createdBy</span><span class="sxs-lookup"><span data-stu-id="f3ff5-147">createdBy</span></span>            | <span data-ttu-id="f3ff5-148">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="f3ff5-148">[identitySet][]</span></span>   | <span data-ttu-id="f3ff5-149">Die Identität des Erstellers dieses Elements.</span><span class="sxs-lookup"><span data-stu-id="f3ff5-149">Identity of the creator of this item.</span></span> <span data-ttu-id="f3ff5-150">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f3ff5-150">Read-only.</span></span>
| <span data-ttu-id="f3ff5-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f3ff5-151">createdDateTime</span></span>      | <span data-ttu-id="f3ff5-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3ff5-152">DateTimeOffset</span></span>    | <span data-ttu-id="f3ff5-p105">Das Datum und die Uhrzeit der Erstellung des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f3ff5-p105">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="f3ff5-155">description</span><span class="sxs-lookup"><span data-stu-id="f3ff5-155">description</span></span>          | <span data-ttu-id="f3ff5-156">string</span><span class="sxs-lookup"><span data-stu-id="f3ff5-156">string</span></span>            | <span data-ttu-id="f3ff5-157">Der beschreibende Text für das Element.</span><span class="sxs-lookup"><span data-stu-id="f3ff5-157">The descriptive text for the item.</span></span>
| <span data-ttu-id="f3ff5-158">eTag</span><span class="sxs-lookup"><span data-stu-id="f3ff5-158">eTag</span></span>                 | <span data-ttu-id="f3ff5-159">string</span><span class="sxs-lookup"><span data-stu-id="f3ff5-159">string</span></span>            | <span data-ttu-id="f3ff5-p106">ETag für das Element. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f3ff5-p106">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="f3ff5-162">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="f3ff5-162">lastModifiedBy</span></span>       | <span data-ttu-id="f3ff5-163">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="f3ff5-163">[identitySet][]</span></span>   | <span data-ttu-id="f3ff5-164">Die Identität derPerson, die dieses Element zuletzt geändert hat.</span><span class="sxs-lookup"><span data-stu-id="f3ff5-164">Identity of the last modifier of this item.</span></span> <span data-ttu-id="f3ff5-165">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f3ff5-165">Read-only.</span></span>
| <span data-ttu-id="f3ff5-166">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f3ff5-166">lastModifiedDateTime</span></span> | <span data-ttu-id="f3ff5-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3ff5-167">DateTimeOffset</span></span>    | <span data-ttu-id="f3ff5-p108">Das Datum und die Uhrzeit der letzten Änderung des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f3ff5-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="f3ff5-170">parentReference</span><span class="sxs-lookup"><span data-stu-id="f3ff5-170">parentReference</span></span>      | <span data-ttu-id="f3ff5-171">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="f3ff5-171">[itemReference][]</span></span> | <span data-ttu-id="f3ff5-p109">Informationen zum übergeordneten Element, wenn das Element ein übergeordnetes Element hat. Lese-/Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="f3ff5-p109">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="f3ff5-174">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="f3ff5-174">sharepointIds</span></span>        | <span data-ttu-id="f3ff5-175">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="f3ff5-175">[sharepointIds][]</span></span> | <span data-ttu-id="f3ff5-p110">Gibt Bezeichner zurück, die für SharePoint REST-Kompatibilität nützlich sind. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f3ff5-p110">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="f3ff5-178">webUrl</span><span class="sxs-lookup"><span data-stu-id="f3ff5-178">webUrl</span></span>               | <span data-ttu-id="f3ff5-179">String (URL)</span><span class="sxs-lookup"><span data-stu-id="f3ff5-179">string (url)</span></span>      | <span data-ttu-id="f3ff5-p111">URL, über die das Element im Browser angezeigt werden kann. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f3ff5-p111">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="f3ff5-182">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f3ff5-182">Relationships</span></span>

 <span data-ttu-id="f3ff5-183">Die **listItem**-Ressource weist folgende Beziehungen zu anderen Ressourcen auf.</span><span class="sxs-lookup"><span data-stu-id="f3ff5-183">The **listItem** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="f3ff5-184">Beziehungsname</span><span class="sxs-lookup"><span data-stu-id="f3ff5-184">Relationship name</span></span> | <span data-ttu-id="f3ff5-185">Typ</span><span class="sxs-lookup"><span data-stu-id="f3ff5-185">Type</span></span>                           | <span data-ttu-id="f3ff5-186">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f3ff5-186">Description</span></span>
|:------------------|:-------------------------------|:-------------------------------
| <span data-ttu-id="f3ff5-187">driveItem</span><span class="sxs-lookup"><span data-stu-id="f3ff5-187">driveItem</span></span>         | <span data-ttu-id="f3ff5-188">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="f3ff5-188">[driveItem][]</span></span>                  | <span data-ttu-id="f3ff5-189">Für Dokumentbibliotheken macht die **DriveItem** Beziehung das ListItem als \*\* [DriveItem][]\*\* verfügbar</span><span class="sxs-lookup"><span data-stu-id="f3ff5-189">For document libraries, the **driveItem** relationship exposes the listItem as a **[driveItem][]**</span></span>
| <span data-ttu-id="f3ff5-190">fields</span><span class="sxs-lookup"><span data-stu-id="f3ff5-190">fields</span></span>            | <span data-ttu-id="f3ff5-191">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="f3ff5-191">[fieldValueSet][]</span></span>              | <span data-ttu-id="f3ff5-192">Die Werte der für dieses Listenelement festgelegten Spalte.</span><span class="sxs-lookup"><span data-stu-id="f3ff5-192">The values of the columns set on this list item.</span></span>
| <span data-ttu-id="f3ff5-193">Versionen</span><span class="sxs-lookup"><span data-stu-id="f3ff5-193">versions</span></span>          | <span data-ttu-id="f3ff5-194">[listItemVersion][]-Sammlung</span><span class="sxs-lookup"><span data-stu-id="f3ff5-194">[listItemVersion][] collection</span></span> | <span data-ttu-id="f3ff5-195">Die Liste der früheren Versionen des Listenelements.</span><span class="sxs-lookup"><span data-stu-id="f3ff5-195">The list of previous versions of the item.</span></span>

[baseItem]: baseitem.md
[contentTypeInfo]: contenttypeinfo.md
[driveItem]: driveitem.md
[fieldValueSet]: fieldvalueset.md
[identitySet]: identityset.md
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
