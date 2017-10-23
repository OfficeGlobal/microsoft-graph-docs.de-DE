---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ListItem
ms.openlocfilehash: eabb88eb6ad2eee7a032b2486555aa26c557ba1a
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/28/2017
---
# <a name="listitem-resource"></a><span data-ttu-id="94b93-102">ListItem-Ressource</span><span class="sxs-lookup"><span data-stu-id="94b93-102">ListItem resource</span></span>

<span data-ttu-id="94b93-103">Diese Ressource stellt ein Element in einer SharePoint-**[Liste][]** dar.</span><span class="sxs-lookup"><span data-stu-id="94b93-103">This resource represents an item in a SharePoint **[list][]**.</span></span>
<span data-ttu-id="94b93-104">Spaltenwerte in der Liste sind über das `fieldValueSet`-Wörterbuch verfügbar.</span><span class="sxs-lookup"><span data-stu-id="94b93-104">Column values in the list are available through the `fieldValueSet` dictionary.</span></span>

## <a name="tasks-on-a-listitem"></a><span data-ttu-id="94b93-105">Aufgaben zu einem listItem</span><span class="sxs-lookup"><span data-stu-id="94b93-105">Tasks on a listItem</span></span>

<span data-ttu-id="94b93-106">Die folgenden Aufgaben sind für **listItem**-Ressourcen verfügbar.</span><span class="sxs-lookup"><span data-stu-id="94b93-106">The following tasks are available for {type} resources.</span></span>
<span data-ttu-id="94b93-107">Alle Beispiele unten beziehen sich auf eine **[Liste][]**, z. B.: `https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}`.</span><span class="sxs-lookup"><span data-stu-id="94b93-107">All examples below are relative to a **[list][]**, eg: `https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}`.</span></span>

| <span data-ttu-id="94b93-108">Häufige Aufgaben</span><span class="sxs-lookup"><span data-stu-id="94b93-108">Common task</span></span>                    | <span data-ttu-id="94b93-109">HTTP-Methode</span><span class="sxs-lookup"><span data-stu-id="94b93-109">HTTP method</span></span>
|:-------------------------------|:------------------------
| <span data-ttu-id="94b93-110">[Get][]</span><span class="sxs-lookup"><span data-stu-id="94b93-110">[Get][]</span></span>                        | <span data-ttu-id="94b93-111">GET /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="94b93-111">GET /items/{item-id}</span></span>
| <span data-ttu-id="94b93-112">[Abrufen von Spaltenwerten][Get]</span><span class="sxs-lookup"><span data-stu-id="94b93-112">[Get column values][Get]</span></span>       | <span data-ttu-id="94b93-113">GET /items/{item-id}?expand=fields</span><span class="sxs-lookup"><span data-stu-id="94b93-113">GET /items/{item-id}?expand=fields</span></span>
| <span data-ttu-id="94b93-114">[Create][]</span><span class="sxs-lookup"><span data-stu-id="94b93-114">[Create][]</span></span>                     | <span data-ttu-id="94b93-115">POST /items</span><span class="sxs-lookup"><span data-stu-id="94b93-115">Post items</span></span>
| <span data-ttu-id="94b93-116">[Delete][]</span><span class="sxs-lookup"><span data-stu-id="94b93-116">[Delete][]</span></span>                     | <span data-ttu-id="94b93-117">DELETE /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="94b93-117">DELETE /items/{item-id}</span></span>
| <span data-ttu-id="94b93-118">[Update][]</span><span class="sxs-lookup"><span data-stu-id="94b93-118">[Update][]</span></span>                     | <span data-ttu-id="94b93-119">PATCH /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="94b93-119">PATCH /items/{item-id}</span></span>
| <span data-ttu-id="94b93-120">[Aktualisieren von Spaltenwerten][Update]</span><span class="sxs-lookup"><span data-stu-id="94b93-120">[Update column values][Update]</span></span> | <span data-ttu-id="94b93-121">PATCH /items/{item-id}/fields</span><span class="sxs-lookup"><span data-stu-id="94b93-121">PATCH /items/{item-id}/fields</span></span>

[Get]: ../api/listItem_get.md
[Create]: ../api/listItem_create.md
[Delete]: ../api/listItem_delete.md
[Update]: ../api/listItem_update.md

## <a name="json-representation"></a><span data-ttu-id="94b93-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="94b93-126">JSON representation</span></span>

<span data-ttu-id="94b93-127">Es folgt eine JSON-Darstellung einer **listItem**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="94b93-127">Here is a JSON representation of a **baseItem** resource.</span></span>

<!-- { "blockType": "resource", 
       "@odata.type": "microsoft.graph.listItem",
       "keyProperty": "id" } -->

```json
{
  "contentType": { "@odata.type": "microsoft.graph.contentType" },
  "fields": { "@odata.type": "microsoft.graph.fieldValueSet" },

  /* relationships */
  "driveItem": { "@odata.type": "microsoft.graph.driveItem" },

  /* inherited from baseItem */
  "id": "string",
  "name": "name of resource",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "timestamp",
  "description": "description of resource",
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "timestamp",
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="94b93-128">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="94b93-128">Properties</span></span>

<span data-ttu-id="94b93-129">Die **listItem**-Ressource weist folgende Eigenschaften auf.</span><span class="sxs-lookup"><span data-stu-id="94b93-129">The **listItem** resource has the following properties.</span></span>

| <span data-ttu-id="94b93-130">Eigenschaftsname</span><span class="sxs-lookup"><span data-stu-id="94b93-130">Property name</span></span> | <span data-ttu-id="94b93-131">Typ</span><span class="sxs-lookup"><span data-stu-id="94b93-131">Type</span></span>                | <span data-ttu-id="94b93-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="94b93-132">Description</span></span>
|:--------------|:--------------------|:-------------------------------
| <span data-ttu-id="94b93-133">contentType</span><span class="sxs-lookup"><span data-stu-id="94b93-133">contentType</span></span>   | <span data-ttu-id="94b93-134">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="94b93-134">[contentTypeInfo][]</span></span> | <span data-ttu-id="94b93-135">Der Inhaltstyp dieses Listenelements</span><span class="sxs-lookup"><span data-stu-id="94b93-135">The content type of this list item</span></span>
| <span data-ttu-id="94b93-136">fields</span><span class="sxs-lookup"><span data-stu-id="94b93-136">fields</span></span>        | <span data-ttu-id="94b93-137">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="94b93-137">[fieldValueSet][]</span></span>   | <span data-ttu-id="94b93-138">Die Werte der für dieses Listenelement festgelegten Spalte.</span><span class="sxs-lookup"><span data-stu-id="94b93-138">The values of the columns set on this list item.</span></span>

<span data-ttu-id="94b93-139">Die folgenden Eigenschaften werden von  ** [baseItem][]** geerbt.</span><span class="sxs-lookup"><span data-stu-id="94b93-139">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="94b93-140">Eigenschaftsname</span><span class="sxs-lookup"><span data-stu-id="94b93-140">Property name</span></span>        | <span data-ttu-id="94b93-141">Typ</span><span class="sxs-lookup"><span data-stu-id="94b93-141">Type</span></span>             | <span data-ttu-id="94b93-142">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="94b93-142">Description</span></span>
|:---------------------|:-----------------|:-----------------------------------
| <span data-ttu-id="94b93-143">id</span><span class="sxs-lookup"><span data-stu-id="94b93-143">id</span></span>                   | <span data-ttu-id="94b93-144">string</span><span class="sxs-lookup"><span data-stu-id="94b93-144">string</span></span>           | <span data-ttu-id="94b93-p103">Der eindeutige Bezeichner des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="94b93-p103">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="94b93-147">name</span><span class="sxs-lookup"><span data-stu-id="94b93-147">name</span></span>                 | <span data-ttu-id="94b93-148">string</span><span class="sxs-lookup"><span data-stu-id="94b93-148">string</span></span>           | <span data-ttu-id="94b93-149">Der Name/Titel des Elements.</span><span class="sxs-lookup"><span data-stu-id="94b93-149">The name / title of the item.</span></span>
| <span data-ttu-id="94b93-150">createdBy</span><span class="sxs-lookup"><span data-stu-id="94b93-150">createdBy</span></span>            | <span data-ttu-id="94b93-151">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="94b93-151">[identitySet][]</span></span>  | <span data-ttu-id="94b93-152">Die Identität des Erstellers dieses Elements.</span><span class="sxs-lookup"><span data-stu-id="94b93-152">Identity of the creator of this item.</span></span> <span data-ttu-id="94b93-153">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="94b93-153">Read-only.</span></span>
| <span data-ttu-id="94b93-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="94b93-154">createdDateTime</span></span>      | <span data-ttu-id="94b93-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94b93-155">DateTimeOffset</span></span>   | <span data-ttu-id="94b93-p105">Das Datum und die Uhrzeit der Erstellung des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="94b93-p105">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="94b93-158">description</span><span class="sxs-lookup"><span data-stu-id="94b93-158">description</span></span>          | <span data-ttu-id="94b93-159">string</span><span class="sxs-lookup"><span data-stu-id="94b93-159">string</span></span>           | <span data-ttu-id="94b93-160">Der beschreibende Text für das Element.</span><span class="sxs-lookup"><span data-stu-id="94b93-160">The descriptive text for the site.</span></span>
| <span data-ttu-id="94b93-161">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="94b93-161">lastModifiedBy</span></span>       | <span data-ttu-id="94b93-162">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="94b93-162">[identitySet][]</span></span>  | <span data-ttu-id="94b93-163">Die Identität der Person, die dieses Element zuletzt geändert hat.</span><span class="sxs-lookup"><span data-stu-id="94b93-163">Identity of the last modifier of this item.</span></span> <span data-ttu-id="94b93-164">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="94b93-164">Read-only.</span></span>
| <span data-ttu-id="94b93-165">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="94b93-165">lastModifiedDateTime</span></span> | <span data-ttu-id="94b93-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94b93-166">DateTimeOffset</span></span>   | <span data-ttu-id="94b93-p107">Das Datum und die Uhrzeit der letzten Änderung des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="94b93-p107">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="94b93-169">webUrl</span><span class="sxs-lookup"><span data-stu-id="94b93-169">webUrl</span></span>               | <span data-ttu-id="94b93-170">String (URL)</span><span class="sxs-lookup"><span data-stu-id="94b93-170">string (url)</span></span>     | <span data-ttu-id="94b93-p108">URL, über die das Element im Browser angezeigt werden kann. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="94b93-p108">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="94b93-173">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="94b93-173">Relationships</span></span>

 <span data-ttu-id="94b93-174">Die **listItem**-Ressource weist folgende Beziehungen zu anderen Ressourcen auf.</span><span class="sxs-lookup"><span data-stu-id="94b93-174">The **listItem** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="94b93-175">Beziehungsname</span><span class="sxs-lookup"><span data-stu-id="94b93-175">Relationship name</span></span> | <span data-ttu-id="94b93-176">Typ</span><span class="sxs-lookup"><span data-stu-id="94b93-176">Type</span></span>                        | <span data-ttu-id="94b93-177">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="94b93-177">Description</span></span>
|:------------------|:----------------------------|:-------------------------------
| <span data-ttu-id="94b93-178">driveItem</span><span class="sxs-lookup"><span data-stu-id="94b93-178">driveItem</span></span>         | <span data-ttu-id="94b93-179">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="94b93-179">[driveItem][]</span></span>               | <span data-ttu-id="94b93-180">Für Dokumentbibliotheken macht die **DriveItem** Beziehung das ListItem als ** [DriveItem][]** verfügbar</span><span class="sxs-lookup"><span data-stu-id="94b93-180">For document libraries, the **driveItem** relationship exposes the listItem as a **[driveItem][]**</span></span>

[baseItem]: baseItem.md
[contentTypeInfo]: contentTypeInfo.md
[driveItem]: driveItem.md
[fieldValueSet]: fieldValueSet.md
[identitySet]: identitySet.md
[list]: list.md

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
