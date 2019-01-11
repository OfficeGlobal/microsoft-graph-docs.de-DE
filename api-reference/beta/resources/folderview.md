---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: FolderView
localization_priority: Normal
ms.openlocfilehash: 717dd93d82f109926cabf0168e4e176d7c68cd35
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861537"
---
# <a name="folderview-resource-type"></a><span data-ttu-id="f2e7f-102">FolderView-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f2e7f-102">FolderView resource type</span></span>

> <span data-ttu-id="f2e7f-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f2e7f-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f2e7f-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f2e7f-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f2e7f-105">Die **FolderView**-Ressource gibt Empfehlungen zur Benutzerfreundlichkeit eines Ordners oder legt sie fest.</span><span class="sxs-lookup"><span data-stu-id="f2e7f-105">The **FolderView** resource provides or sets recommendations on the user-experience of a folder.</span></span>

<span data-ttu-id="f2e7f-106">Es ist verfügbar über die Eigenschaft [folder][folder-facet] von Ressourcen des Typs [driveItem][item-resource].</span><span class="sxs-lookup"><span data-stu-id="f2e7f-106">It is available from the [folder][folder-facet] property of [driveItem][item-resource] resources.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f2e7f-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f2e7f-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.folderView" } -->

```json
{
  "sortBy": "default | name | type | size | takenOrCreatedDateTime | lastModifiedDateTime | sequence",
  "sortDescending": "ascending | descending",
  "viewType": "default | icons | details | thumbnails"
}
```

## <a name="properties"></a><span data-ttu-id="f2e7f-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f2e7f-108">Properties</span></span>

| <span data-ttu-id="f2e7f-109">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="f2e7f-109">Property name</span></span>         | <span data-ttu-id="f2e7f-110">Typ</span><span class="sxs-lookup"><span data-stu-id="f2e7f-110">Type</span></span>   | <span data-ttu-id="f2e7f-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f2e7f-111">Description</span></span>
|:----------------------|:-------|:--------------------------------------------
| <span data-ttu-id="f2e7f-112">**sortBy**</span><span class="sxs-lookup"><span data-stu-id="f2e7f-112">**sortBy**</span></span>            | <span data-ttu-id="f2e7f-113">string</span><span class="sxs-lookup"><span data-stu-id="f2e7f-113">string</span></span> | <span data-ttu-id="f2e7f-114">Diese Eigenschaft legt die Methode fest, auf deren Basis der Ordner sortiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="f2e7f-114">The method by which the folder should be sorted.</span></span>
| <span data-ttu-id="f2e7f-115">**sortOrder**</span><span class="sxs-lookup"><span data-stu-id="f2e7f-115">**sortOrder**</span></span>         | <span data-ttu-id="f2e7f-116">string</span><span class="sxs-lookup"><span data-stu-id="f2e7f-116">string</span></span> | <span data-ttu-id="f2e7f-117">Ist diese Eigenschaft auf „true“ gesetzt, sollen alle Elemente in absteigender Reihenfolge sortiert werden.</span><span class="sxs-lookup"><span data-stu-id="f2e7f-117">If true, indicates that items should be sorted in descending order.</span></span> <span data-ttu-id="f2e7f-118">Andernfalls sollen die Elemente in aufsteigender Reihenfolge sortiert werden.</span><span class="sxs-lookup"><span data-stu-id="f2e7f-118">Otherwise, items should be sorted ascending.</span></span>
| <span data-ttu-id="f2e7f-119">**viewType**</span><span class="sxs-lookup"><span data-stu-id="f2e7f-119">**viewType**</span></span>          | <span data-ttu-id="f2e7f-120">string</span><span class="sxs-lookup"><span data-stu-id="f2e7f-120">string</span></span> | <span data-ttu-id="f2e7f-121">Diese Eigenschaft legt die Ansicht fest, die zur Darstellung des Ordners verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="f2e7f-121">The type of view that should be used to represent the folder.</span></span>

<span data-ttu-id="f2e7f-122">Über die Eigenschaft _sortBy_ können Sie die Sortierreihenfolge von Elementen in allen Anwendungen steuern, die das Facet **viewType** berücksichtigen.</span><span class="sxs-lookup"><span data-stu-id="f2e7f-122">You can use the _sortBy_ property to control the sort order of the items in applications that respect the **viewType** facet.</span></span>

### <a name="sortby-values"></a><span data-ttu-id="f2e7f-123">Werte für „sortBy“</span><span class="sxs-lookup"><span data-stu-id="f2e7f-123">sortBy values</span></span>

<span data-ttu-id="f2e7f-124">Für die Eigenschaft **sortBy** sind die folgenden Werte definiert:</span><span class="sxs-lookup"><span data-stu-id="f2e7f-124">The following values are defined for the **sortBy** property.</span></span>

| <span data-ttu-id="f2e7f-125">Wert</span><span class="sxs-lookup"><span data-stu-id="f2e7f-125">Value</span></span>                    | <span data-ttu-id="f2e7f-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f2e7f-126">Description</span></span>
| ------------------------ | --------------------------------------------------
| `default`                | <span data-ttu-id="f2e7f-127">Dieser Wert steht für die Standardsortierreihenfolge der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="f2e7f-127">The default sort order of the application.</span></span>
| `name`                   | <span data-ttu-id="f2e7f-128">Elemente sollen auf Basis ihrer Eigenschaft **name** sortiert werden.</span><span class="sxs-lookup"><span data-stu-id="f2e7f-128">Items should be arranged by the **name** property of the items.</span></span>
| `type`                   | <span data-ttu-id="f2e7f-129">Elemente sollen auf Basis des Elementtyps sortiert werden.</span><span class="sxs-lookup"><span data-stu-id="f2e7f-129">Items should be arranged by the type of item.</span></span>
| `size`                   | <span data-ttu-id="f2e7f-130">Elemente sollen auf Basis ihrer Eigenschaft **size** sortiert werden.</span><span class="sxs-lookup"><span data-stu-id="f2e7f-130">Items should be arranged by the **size** property of the items.</span></span>
| `takenOrCreatedDateTime` | <span data-ttu-id="f2e7f-131">Elemente sollen auf Basis der Eigenschaft **takenDateTime** des Facet **photo** sortiert werden.</span><span class="sxs-lookup"><span data-stu-id="f2e7f-131">Items should be arranged by the **takenDateTime** property of the **photo** facet.</span></span> <span data-ttu-id="f2e7f-132">Ist diese nicht verfügbar, soll die Eigenschaft **createdDateTime** verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="f2e7f-132">If not available, the **createdDateTime** property should be used.</span></span>
| `lastModifiedDateTime`   | <span data-ttu-id="f2e7f-133">Elemente sollen auf Basis ihrer Eigenschaft **lastModifiedDateTime** sortiert werden.</span><span class="sxs-lookup"><span data-stu-id="f2e7f-133">Items should be arranged by the **lastModifiedDateTime** property of the items.</span></span>
| `sequence`               | <span data-ttu-id="f2e7f-134">Die Elemente folgen einer vom Benutzer angegebenen benutzerdefinierten Sequenz.</span><span class="sxs-lookup"><span data-stu-id="f2e7f-134">Items follow a custom sequence specified by the user.</span></span>


### <a name="sortorder-values"></a><span data-ttu-id="f2e7f-135">sortOrder-Werte</span><span class="sxs-lookup"><span data-stu-id="f2e7f-135">sortOrder values</span></span>

<span data-ttu-id="f2e7f-136">Für die Eigenschaft **sortOrder** sind die folgenden Werte definiert:</span><span class="sxs-lookup"><span data-stu-id="f2e7f-136">The following values are defined for the **sortOrder** property.</span></span>

| <span data-ttu-id="f2e7f-137">Wert</span><span class="sxs-lookup"><span data-stu-id="f2e7f-137">Value</span></span>        | <span data-ttu-id="f2e7f-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f2e7f-138">Description</span></span>
| ------------ | --------------------------------------------------------------
| `ascending`  | <span data-ttu-id="f2e7f-139">Elemente sollen in aufsteigender Reihenfolge sortiert werden.</span><span class="sxs-lookup"><span data-stu-id="f2e7f-139">Items should be arranged in ascending order.</span></span>
| `descending` | <span data-ttu-id="f2e7f-140">Elemente sollen in absteigender Reihenfolge sortiert werden.</span><span class="sxs-lookup"><span data-stu-id="f2e7f-140">Items should be arranged in descending order.</span></span>


### <a name="viewtype-values"></a><span data-ttu-id="f2e7f-141">Werte für „viewType“</span><span class="sxs-lookup"><span data-stu-id="f2e7f-141">viewType values</span></span>

<span data-ttu-id="f2e7f-142">Für die Eigenschaft **viewType** sind die folgenden Werte definiert:</span><span class="sxs-lookup"><span data-stu-id="f2e7f-142">The following values are defined for the **viewType** property.</span></span>

| <span data-ttu-id="f2e7f-143">Wert</span><span class="sxs-lookup"><span data-stu-id="f2e7f-143">Value</span></span>        | <span data-ttu-id="f2e7f-144">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f2e7f-144">Description</span></span>
| ------------ | --------------------------------------------------------------
| `default`    | <span data-ttu-id="f2e7f-145">Der Standardansichtstyp der Anwendung</span><span class="sxs-lookup"><span data-stu-id="f2e7f-145">The default view type for the application.</span></span>
| `icons`      | <span data-ttu-id="f2e7f-146">Eine Ansicht, die Ressourcen des Typs „driveItem“ als Symbole darstellt</span><span class="sxs-lookup"><span data-stu-id="f2e7f-146">A view that uses icons to represent driveItems.</span></span>
| `details`    | <span data-ttu-id="f2e7f-147">Eine Ansicht mit mehreren Spalten, die zusätzliche Details zu den einzelnen Elementen enthalten</span><span class="sxs-lookup"><span data-stu-id="f2e7f-147">A view with multiple columns that provide additional details about each item.</span></span>
| `thumbnails` | <span data-ttu-id="f2e7f-148">Eine Ansicht, die Elemente als größere Miniaturansichten von Ressourcen des Typs „driveItem“ darstellt</span><span class="sxs-lookup"><span data-stu-id="f2e7f-148">A view that uses larger thumbnails of driveItems to represent the items.</span></span>


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
