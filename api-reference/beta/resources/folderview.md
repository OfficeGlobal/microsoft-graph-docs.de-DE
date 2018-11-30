---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: FolderView
ms.openlocfilehash: 1658751371f3a3ae186d5a092ae5610f016d26b4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058444"
---
# <a name="folderview-resource-type"></a><span data-ttu-id="bb8c9-102">FolderView-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="bb8c9-102">FolderView resource type</span></span>

> <span data-ttu-id="bb8c9-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="bb8c9-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bb8c9-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bb8c9-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bb8c9-105">Die **FolderView**-Ressource gibt Empfehlungen zur Benutzerfreundlichkeit eines Ordners oder legt sie fest.</span><span class="sxs-lookup"><span data-stu-id="bb8c9-105">The **FolderView** resource provides or sets recommendations on the user-experience of a folder.</span></span>

<span data-ttu-id="bb8c9-106">Es ist verfügbar über die Eigenschaft [folder][folder-facet] von Ressourcen des Typs [driveItem][item-resource].</span><span class="sxs-lookup"><span data-stu-id="bb8c9-106">It is available from the [folder][folder-facet] property of [driveItem][item-resource] resources.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bb8c9-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bb8c9-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.folderView" } -->

```json
{
  "sortBy": "default | name | type | size | takenOrCreatedDateTime | lastModifiedDateTime | sequence",
  "sortDescending": "ascending | descending",
  "viewType": "default | icons | details | thumbnails"
}
```

## <a name="properties"></a><span data-ttu-id="bb8c9-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bb8c9-108">Properties</span></span>

| <span data-ttu-id="bb8c9-109">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="bb8c9-109">Property name</span></span>         | <span data-ttu-id="bb8c9-110">Typ</span><span class="sxs-lookup"><span data-stu-id="bb8c9-110">Type</span></span>   | <span data-ttu-id="bb8c9-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bb8c9-111">Description</span></span>
|:----------------------|:-------|:--------------------------------------------
| <span data-ttu-id="bb8c9-112">**sortBy**</span><span class="sxs-lookup"><span data-stu-id="bb8c9-112">**sortBy**</span></span>            | <span data-ttu-id="bb8c9-113">string</span><span class="sxs-lookup"><span data-stu-id="bb8c9-113">string</span></span> | <span data-ttu-id="bb8c9-114">Diese Eigenschaft legt die Methode fest, auf deren Basis der Ordner sortiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="bb8c9-114">The method by which the folder should be sorted.</span></span>
| <span data-ttu-id="bb8c9-115">**sortOrder**</span><span class="sxs-lookup"><span data-stu-id="bb8c9-115">**sortOrder**</span></span>         | <span data-ttu-id="bb8c9-116">string</span><span class="sxs-lookup"><span data-stu-id="bb8c9-116">string</span></span> | <span data-ttu-id="bb8c9-117">Ist diese Eigenschaft auf „true“ gesetzt, sollen alle Elemente in absteigender Reihenfolge sortiert werden.</span><span class="sxs-lookup"><span data-stu-id="bb8c9-117">If true, indicates that items should be sorted in descending order.</span></span> <span data-ttu-id="bb8c9-118">Andernfalls sollen die Elemente in aufsteigender Reihenfolge sortiert werden.</span><span class="sxs-lookup"><span data-stu-id="bb8c9-118">Otherwise, items should be sorted ascending.</span></span>
| <span data-ttu-id="bb8c9-119">**viewType**</span><span class="sxs-lookup"><span data-stu-id="bb8c9-119">**viewType**</span></span>          | <span data-ttu-id="bb8c9-120">string</span><span class="sxs-lookup"><span data-stu-id="bb8c9-120">string</span></span> | <span data-ttu-id="bb8c9-121">Diese Eigenschaft legt die Ansicht fest, die zur Darstellung des Ordners verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="bb8c9-121">The type of view that should be used to represent the folder.</span></span>

<span data-ttu-id="bb8c9-122">Über die Eigenschaft _sortBy_ können Sie die Sortierreihenfolge von Elementen in allen Anwendungen steuern, die das Facet **viewType** berücksichtigen.</span><span class="sxs-lookup"><span data-stu-id="bb8c9-122">You can use the _sortBy_ property to control the sort order of the items in applications that respect the **viewType** facet.</span></span>

### <a name="sortby-values"></a><span data-ttu-id="bb8c9-123">Werte für „sortBy“</span><span class="sxs-lookup"><span data-stu-id="bb8c9-123">sortBy values</span></span>

<span data-ttu-id="bb8c9-124">Für die Eigenschaft **sortBy** sind die folgenden Werte definiert:</span><span class="sxs-lookup"><span data-stu-id="bb8c9-124">The following values are defined for the **sortBy** property.</span></span>

| <span data-ttu-id="bb8c9-125">Wert</span><span class="sxs-lookup"><span data-stu-id="bb8c9-125">Value</span></span>                    | <span data-ttu-id="bb8c9-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bb8c9-126">Description</span></span>
| ------------------------ | --------------------------------------------------
| `default`                | <span data-ttu-id="bb8c9-127">Dieser Wert steht für die Standardsortierreihenfolge der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="bb8c9-127">The default sort order of the application.</span></span>
| `name`                   | <span data-ttu-id="bb8c9-128">Elemente sollen auf Basis ihrer Eigenschaft **name** sortiert werden.</span><span class="sxs-lookup"><span data-stu-id="bb8c9-128">Items should be arranged by the **name** property of the items.</span></span>
| `type`                   | <span data-ttu-id="bb8c9-129">Elemente sollen auf Basis des Elementtyps sortiert werden.</span><span class="sxs-lookup"><span data-stu-id="bb8c9-129">Items should be arranged by the type of item.</span></span>
| `size`                   | <span data-ttu-id="bb8c9-130">Elemente sollen auf Basis ihrer Eigenschaft **size** sortiert werden.</span><span class="sxs-lookup"><span data-stu-id="bb8c9-130">Items should be arranged by the **size** property of the items.</span></span>
| `takenOrCreatedDateTime` | <span data-ttu-id="bb8c9-131">Elemente sollen auf Basis der Eigenschaft **takenDateTime** des Facet **photo** sortiert werden.</span><span class="sxs-lookup"><span data-stu-id="bb8c9-131">Items should be arranged by the **takenDateTime** property of the **photo** facet.</span></span> <span data-ttu-id="bb8c9-132">Ist diese nicht verfügbar, soll die Eigenschaft **createdDateTime** verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="bb8c9-132">If not available, the **createdDateTime** property should be used.</span></span>
| `lastModifiedDateTime`   | <span data-ttu-id="bb8c9-133">Elemente sollen auf Basis ihrer Eigenschaft **lastModifiedDateTime** sortiert werden.</span><span class="sxs-lookup"><span data-stu-id="bb8c9-133">Items should be arranged by the **lastModifiedDateTime** property of the items.</span></span>
| `sequence`               | <span data-ttu-id="bb8c9-134">Die Elemente folgen einer vom Benutzer angegebenen benutzerdefinierten Sequenz.</span><span class="sxs-lookup"><span data-stu-id="bb8c9-134">Items follow a custom sequence specified by the user.</span></span>


### <a name="sortorder-values"></a><span data-ttu-id="bb8c9-135">sortOrder-Werte</span><span class="sxs-lookup"><span data-stu-id="bb8c9-135">sortOrder values</span></span>

<span data-ttu-id="bb8c9-136">Für die Eigenschaft **sortOrder** sind die folgenden Werte definiert:</span><span class="sxs-lookup"><span data-stu-id="bb8c9-136">The following values are defined for the **sortOrder** property.</span></span>

| <span data-ttu-id="bb8c9-137">Wert</span><span class="sxs-lookup"><span data-stu-id="bb8c9-137">Value</span></span>        | <span data-ttu-id="bb8c9-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bb8c9-138">Description</span></span>
| ------------ | --------------------------------------------------------------
| `ascending`  | <span data-ttu-id="bb8c9-139">Elemente sollen in aufsteigender Reihenfolge sortiert werden.</span><span class="sxs-lookup"><span data-stu-id="bb8c9-139">Items should be arranged in ascending order.</span></span>
| `descending` | <span data-ttu-id="bb8c9-140">Elemente sollen in absteigender Reihenfolge sortiert werden.</span><span class="sxs-lookup"><span data-stu-id="bb8c9-140">Items should be arranged in descending order.</span></span>


### <a name="viewtype-values"></a><span data-ttu-id="bb8c9-141">Werte für „viewType“</span><span class="sxs-lookup"><span data-stu-id="bb8c9-141">viewType values</span></span>

<span data-ttu-id="bb8c9-142">Für die Eigenschaft **viewType** sind die folgenden Werte definiert:</span><span class="sxs-lookup"><span data-stu-id="bb8c9-142">The following values are defined for the **viewType** property.</span></span>

| <span data-ttu-id="bb8c9-143">Wert</span><span class="sxs-lookup"><span data-stu-id="bb8c9-143">Value</span></span>        | <span data-ttu-id="bb8c9-144">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bb8c9-144">Description</span></span>
| ------------ | --------------------------------------------------------------
| `default`    | <span data-ttu-id="bb8c9-145">Der Standardansichtstyp der Anwendung</span><span class="sxs-lookup"><span data-stu-id="bb8c9-145">The default view type for the application.</span></span>
| `icons`      | <span data-ttu-id="bb8c9-146">Eine Ansicht, die Ressourcen des Typs „driveItem“ als Symbole darstellt</span><span class="sxs-lookup"><span data-stu-id="bb8c9-146">A view that uses icons to represent driveItems.</span></span>
| `details`    | <span data-ttu-id="bb8c9-147">Eine Ansicht mit mehreren Spalten, die zusätzliche Details zu den einzelnen Elementen enthalten</span><span class="sxs-lookup"><span data-stu-id="bb8c9-147">A view with multiple columns that provide additional details about each item.</span></span>
| `thumbnails` | <span data-ttu-id="bb8c9-148">Eine Ansicht, die Elemente als größere Miniaturansichten von Ressourcen des Typs „driveItem“ darstellt</span><span class="sxs-lookup"><span data-stu-id="bb8c9-148">A view that uses larger thumbnails of driveItems to represent the items.</span></span>


[item-resource]: driveitem.md
[folder-facet]: folder.md

<!-- uuid: f9e446fd-190b-4692-a605-bb60e78f1f19
2017-05-03 02:34:40 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "folderView resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
