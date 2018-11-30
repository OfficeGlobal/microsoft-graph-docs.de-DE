---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ListItem
ms.openlocfilehash: b7293398314ea91dcb5ac6985031f91d6531e78f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019263"
---
# <a name="listitem-resource"></a><span data-ttu-id="cc8af-102">ListItem-Ressource</span><span class="sxs-lookup"><span data-stu-id="cc8af-102">ListItem resource</span></span>

<span data-ttu-id="cc8af-103">Diese Ressource stellt ein Element in einer SharePoint-**[Liste][]** dar.</span><span class="sxs-lookup"><span data-stu-id="cc8af-103">This resource represents an item in a SharePoint **[list][]**.</span></span>
<span data-ttu-id="cc8af-104">Spaltenwerte in der Liste sind über das `fieldValueSet`-Wörterbuch verfügbar.</span><span class="sxs-lookup"><span data-stu-id="cc8af-104">Column values in the list are available through the `fieldValueSet` dictionary.</span></span>

## <a name="tasks-on-a-listitem"></a><span data-ttu-id="cc8af-105">Aufgaben zu einem listItem</span><span class="sxs-lookup"><span data-stu-id="cc8af-105">Tasks on a listItem</span></span>

<span data-ttu-id="cc8af-106">Die folgenden Aufgaben sind für **listItem**-Ressourcen verfügbar.</span><span class="sxs-lookup"><span data-stu-id="cc8af-106">The following tasks are available for **listItem** resources.</span></span>
<span data-ttu-id="cc8af-107">Alle Beispiele unten beziehen sich auf eine **[Liste][]**, z. B.: `https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}`.</span><span class="sxs-lookup"><span data-stu-id="cc8af-107">All examples below are relative to a **[list][]**, eg: `https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}`.</span></span>

| <span data-ttu-id="cc8af-108">Häufige Aufgaben</span><span class="sxs-lookup"><span data-stu-id="cc8af-108">Common task</span></span>                    | <span data-ttu-id="cc8af-109">HTTP-Methode</span><span class="sxs-lookup"><span data-stu-id="cc8af-109">HTTP method</span></span>
|:-------------------------------|:------------------------
| <span data-ttu-id="cc8af-110">[Get][]</span><span class="sxs-lookup"><span data-stu-id="cc8af-110">[Get][]</span></span>                        | <span data-ttu-id="cc8af-111">GET /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="cc8af-111">GET /items/{item-id}</span></span>
| <span data-ttu-id="cc8af-112">[Abrufen von Spaltenwerten][Get]</span><span class="sxs-lookup"><span data-stu-id="cc8af-112">[Get column values][Get]</span></span>       | <span data-ttu-id="cc8af-113">GET /items/{item-id}?expand=fields</span><span class="sxs-lookup"><span data-stu-id="cc8af-113">GET /items/{item-id}?expand=fields</span></span>
| <span data-ttu-id="cc8af-114">[Create][]</span><span class="sxs-lookup"><span data-stu-id="cc8af-114">[Create][]</span></span>                     | <span data-ttu-id="cc8af-115">POST /items</span><span class="sxs-lookup"><span data-stu-id="cc8af-115">POST /items</span></span>
| <span data-ttu-id="cc8af-116">[Delete][]</span><span class="sxs-lookup"><span data-stu-id="cc8af-116">[Delete][]</span></span>                     | <span data-ttu-id="cc8af-117">DELETE /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="cc8af-117">DELETE /items/{item-id}</span></span>
| <span data-ttu-id="cc8af-118">[Update][]</span><span class="sxs-lookup"><span data-stu-id="cc8af-118">[Update][]</span></span>                     | <span data-ttu-id="cc8af-119">PATCH /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="cc8af-119">PATCH /items/{item-id}</span></span>
| <span data-ttu-id="cc8af-120">[Aktualisieren von Spaltenwerten][Update]</span><span class="sxs-lookup"><span data-stu-id="cc8af-120">[Update column values][Update]</span></span> | <span data-ttu-id="cc8af-121">PATCH /items/{item-id}/fields</span><span class="sxs-lookup"><span data-stu-id="cc8af-121">PATCH /items/{item-id}/fields</span></span>

[Get]: ../api/listitem-get.md
[Create]: ../api/listitem-create.md
[Delete]: ../api/listitem-delete.md
[Update]: ../api/listitem-update.md

## <a name="json-representation"></a><span data-ttu-id="cc8af-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="cc8af-126">JSON representation</span></span>

<span data-ttu-id="cc8af-127">Es folgt eine JSON-Darstellung einer **listItem**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="cc8af-127">Here is a JSON representation of a **listItem** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="cc8af-128">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="cc8af-128">Properties</span></span>

<span data-ttu-id="cc8af-129">Die **listItem**-Ressource weist folgende Eigenschaften auf.</span><span class="sxs-lookup"><span data-stu-id="cc8af-129">The **listItem** resource has the following properties.</span></span>

| <span data-ttu-id="cc8af-130">Eigenschaftsname</span><span class="sxs-lookup"><span data-stu-id="cc8af-130">Property name</span></span> | <span data-ttu-id="cc8af-131">Typ</span><span class="sxs-lookup"><span data-stu-id="cc8af-131">Type</span></span>                | <span data-ttu-id="cc8af-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cc8af-132">Description</span></span>
|:--------------|:--------------------|:-------------------------------
| <span data-ttu-id="cc8af-133">contentType</span><span class="sxs-lookup"><span data-stu-id="cc8af-133">contentType</span></span>   | <span data-ttu-id="cc8af-134">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="cc8af-134">[contentTypeInfo][]</span></span> | <span data-ttu-id="cc8af-135">Der Inhaltstyp dieses Listenelements</span><span class="sxs-lookup"><span data-stu-id="cc8af-135">The content type of this list item</span></span>

<span data-ttu-id="cc8af-136">Die folgenden Eigenschaften werden von  **[baseItem][]** geerbt.</span><span class="sxs-lookup"><span data-stu-id="cc8af-136">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="cc8af-137">Eigenschaftsname</span><span class="sxs-lookup"><span data-stu-id="cc8af-137">Property name</span></span>        | <span data-ttu-id="cc8af-138">Typ</span><span class="sxs-lookup"><span data-stu-id="cc8af-138">Type</span></span>              | <span data-ttu-id="cc8af-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cc8af-139">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="cc8af-140">id</span><span class="sxs-lookup"><span data-stu-id="cc8af-140">id</span></span>                   | <span data-ttu-id="cc8af-141">string</span><span class="sxs-lookup"><span data-stu-id="cc8af-141">string</span></span>            | <span data-ttu-id="cc8af-p103">Der eindeutige Bezeichner des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="cc8af-p103">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="cc8af-144">name</span><span class="sxs-lookup"><span data-stu-id="cc8af-144">name</span></span>                 | <span data-ttu-id="cc8af-145">string</span><span class="sxs-lookup"><span data-stu-id="cc8af-145">string</span></span>            | <span data-ttu-id="cc8af-146">Der Name/Titel des Elements.</span><span class="sxs-lookup"><span data-stu-id="cc8af-146">The name / title of the item.</span></span>
| <span data-ttu-id="cc8af-147">createdBy</span><span class="sxs-lookup"><span data-stu-id="cc8af-147">createdBy</span></span>            | <span data-ttu-id="cc8af-148">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="cc8af-148">[identitySet][]</span></span>   | <span data-ttu-id="cc8af-149">Die Identität des Erstellers dieses Elements.</span><span class="sxs-lookup"><span data-stu-id="cc8af-149">Identity of the creator of this item.</span></span> <span data-ttu-id="cc8af-150">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="cc8af-150">Read-only.</span></span>
| <span data-ttu-id="cc8af-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cc8af-151">createdDateTime</span></span>      | <span data-ttu-id="cc8af-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc8af-152">DateTimeOffset</span></span>    | <span data-ttu-id="cc8af-p105">Das Datum und die Uhrzeit der Erstellung des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="cc8af-p105">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="cc8af-155">description</span><span class="sxs-lookup"><span data-stu-id="cc8af-155">description</span></span>          | <span data-ttu-id="cc8af-156">string</span><span class="sxs-lookup"><span data-stu-id="cc8af-156">string</span></span>            | <span data-ttu-id="cc8af-157">Der beschreibende Text für das Element.</span><span class="sxs-lookup"><span data-stu-id="cc8af-157">The descriptive text for the item.</span></span>
| <span data-ttu-id="cc8af-158">eTag</span><span class="sxs-lookup"><span data-stu-id="cc8af-158">eTag</span></span>                 | <span data-ttu-id="cc8af-159">string</span><span class="sxs-lookup"><span data-stu-id="cc8af-159">string</span></span>            | <span data-ttu-id="cc8af-p106">ETag für das Element. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="cc8af-p106">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="cc8af-162">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="cc8af-162">lastModifiedBy</span></span>       | <span data-ttu-id="cc8af-163">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="cc8af-163">[identitySet][]</span></span>   | <span data-ttu-id="cc8af-164">Die Identität derPerson, die dieses Element zuletzt geändert hat.</span><span class="sxs-lookup"><span data-stu-id="cc8af-164">Identity of the last modifier of this item.</span></span> <span data-ttu-id="cc8af-165">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="cc8af-165">Read-only.</span></span>
| <span data-ttu-id="cc8af-166">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cc8af-166">lastModifiedDateTime</span></span> | <span data-ttu-id="cc8af-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc8af-167">DateTimeOffset</span></span>    | <span data-ttu-id="cc8af-p108">Das Datum und die Uhrzeit der letzten Änderung des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="cc8af-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="cc8af-170">parentReference</span><span class="sxs-lookup"><span data-stu-id="cc8af-170">parentReference</span></span>      | <span data-ttu-id="cc8af-171">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="cc8af-171">[itemReference][]</span></span> | <span data-ttu-id="cc8af-p109">Informationen zum übergeordneten Element, wenn das Element ein übergeordnetes Element hat. Lese-/Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="cc8af-p109">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="cc8af-174">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="cc8af-174">sharepointIds</span></span>        | <span data-ttu-id="cc8af-175">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="cc8af-175">[sharepointIds][]</span></span> | <span data-ttu-id="cc8af-p110">Gibt Bezeichner zurück, die für SharePoint REST-Kompatibilität nützlich sind. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="cc8af-p110">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="cc8af-178">webUrl</span><span class="sxs-lookup"><span data-stu-id="cc8af-178">webUrl</span></span>               | <span data-ttu-id="cc8af-179">String (URL)</span><span class="sxs-lookup"><span data-stu-id="cc8af-179">string (url)</span></span>      | <span data-ttu-id="cc8af-p111">URL, über die das Element im Browser angezeigt werden kann. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="cc8af-p111">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="cc8af-182">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="cc8af-182">Relationships</span></span>

 <span data-ttu-id="cc8af-183">Die **listItem**-Ressource weist folgende Beziehungen zu anderen Ressourcen auf.</span><span class="sxs-lookup"><span data-stu-id="cc8af-183">The **listItem** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="cc8af-184">Beziehungsname</span><span class="sxs-lookup"><span data-stu-id="cc8af-184">Relationship name</span></span> | <span data-ttu-id="cc8af-185">Typ</span><span class="sxs-lookup"><span data-stu-id="cc8af-185">Type</span></span>                           | <span data-ttu-id="cc8af-186">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cc8af-186">Description</span></span>
|:------------------|:-------------------------------|:-------------------------------
| <span data-ttu-id="cc8af-187">driveItem</span><span class="sxs-lookup"><span data-stu-id="cc8af-187">driveItem</span></span>         | <span data-ttu-id="cc8af-188">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="cc8af-188">[driveItem][]</span></span>                  | <span data-ttu-id="cc8af-189">Für Dokumentbibliotheken macht die **DriveItem** Beziehung das ListItem als \*\* [DriveItem][]\*\* verfügbar</span><span class="sxs-lookup"><span data-stu-id="cc8af-189">For document libraries, the **driveItem** relationship exposes the listItem as a **[driveItem][]**</span></span>
| <span data-ttu-id="cc8af-190">fields</span><span class="sxs-lookup"><span data-stu-id="cc8af-190">fields</span></span>            | <span data-ttu-id="cc8af-191">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="cc8af-191">[fieldValueSet][]</span></span>              | <span data-ttu-id="cc8af-192">Die Werte der für dieses Listenelement festgelegten Spalte.</span><span class="sxs-lookup"><span data-stu-id="cc8af-192">The values of the columns set on this list item.</span></span>
| <span data-ttu-id="cc8af-193">Versionen</span><span class="sxs-lookup"><span data-stu-id="cc8af-193">versions</span></span>          | <span data-ttu-id="cc8af-194">[ListItemVersion][] -Auflistung</span><span class="sxs-lookup"><span data-stu-id="cc8af-194">[listItemVersion][] collection</span></span> | <span data-ttu-id="cc8af-195">Die Liste der vorherigen Versionen des Listenelements.</span><span class="sxs-lookup"><span data-stu-id="cc8af-195">The list of previous versions of the list item.</span></span>

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
