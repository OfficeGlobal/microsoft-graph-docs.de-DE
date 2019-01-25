---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: FolderView
localization_priority: Normal
ms.openlocfilehash: e57e74a0dbcb785d88fb7ccdd3aa3c0e62dc882a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517568"
---
# <a name="folderview-resource-type"></a><span data-ttu-id="36dc8-102">FolderView-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="36dc8-102">FolderView resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36dc8-103">Die **FolderView**-Ressource gibt Empfehlungen zur Benutzerfreundlichkeit eines Ordners oder legt sie fest.</span><span class="sxs-lookup"><span data-stu-id="36dc8-103">The **FolderView** resource provides or sets recommendations on the user-experience of a folder.</span></span>

<span data-ttu-id="36dc8-104">Es ist verfügbar über die Eigenschaft [folder][folder-facet] von Ressourcen des Typs [driveItem][item-resource].</span><span class="sxs-lookup"><span data-stu-id="36dc8-104">It is available from the [folder][folder-facet] property of [driveItem][item-resource] resources.</span></span>

## <a name="json-representation"></a><span data-ttu-id="36dc8-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="36dc8-105">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.folderView" } -->

```json
{
  "sortBy": "default | name | type | size | takenOrCreatedDateTime | lastModifiedDateTime | sequence",
  "sortDescending": "ascending | descending",
  "viewType": "default | icons | details | thumbnails"
}
```

## <a name="properties"></a><span data-ttu-id="36dc8-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="36dc8-106">Properties</span></span>

| <span data-ttu-id="36dc8-107">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="36dc8-107">Property name</span></span>         | <span data-ttu-id="36dc8-108">Typ</span><span class="sxs-lookup"><span data-stu-id="36dc8-108">Type</span></span>   | <span data-ttu-id="36dc8-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="36dc8-109">Description</span></span>
|:----------------------|:-------|:--------------------------------------------
| <span data-ttu-id="36dc8-110">**sortBy**</span><span class="sxs-lookup"><span data-stu-id="36dc8-110">**sortBy**</span></span>            | <span data-ttu-id="36dc8-111">string</span><span class="sxs-lookup"><span data-stu-id="36dc8-111">string</span></span> | <span data-ttu-id="36dc8-112">Diese Eigenschaft legt die Methode fest, auf deren Basis der Ordner sortiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="36dc8-112">The method by which the folder should be sorted.</span></span>
| <span data-ttu-id="36dc8-113">**sortOrder**</span><span class="sxs-lookup"><span data-stu-id="36dc8-113">**sortOrder**</span></span>         | <span data-ttu-id="36dc8-114">string</span><span class="sxs-lookup"><span data-stu-id="36dc8-114">string</span></span> | <span data-ttu-id="36dc8-115">Ist diese Eigenschaft auf „true“ gesetzt, sollen alle Elemente in absteigender Reihenfolge sortiert werden.</span><span class="sxs-lookup"><span data-stu-id="36dc8-115">If true, indicates that items should be sorted in descending order.</span></span> <span data-ttu-id="36dc8-116">Andernfalls sollen die Elemente in aufsteigender Reihenfolge sortiert werden.</span><span class="sxs-lookup"><span data-stu-id="36dc8-116">Otherwise, items should be sorted ascending.</span></span>
| <span data-ttu-id="36dc8-117">**viewType**</span><span class="sxs-lookup"><span data-stu-id="36dc8-117">**viewType**</span></span>          | <span data-ttu-id="36dc8-118">string</span><span class="sxs-lookup"><span data-stu-id="36dc8-118">string</span></span> | <span data-ttu-id="36dc8-119">Diese Eigenschaft legt die Ansicht fest, die zur Darstellung des Ordners verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="36dc8-119">The type of view that should be used to represent the folder.</span></span>

<span data-ttu-id="36dc8-120">Über die Eigenschaft _sortBy_ können Sie die Sortierreihenfolge von Elementen in allen Anwendungen steuern, die das Facet **viewType** berücksichtigen.</span><span class="sxs-lookup"><span data-stu-id="36dc8-120">You can use the _sortBy_ property to control the sort order of the items in applications that respect the **viewType** facet.</span></span>

### <a name="sortby-values"></a><span data-ttu-id="36dc8-121">Werte für „sortBy“</span><span class="sxs-lookup"><span data-stu-id="36dc8-121">sortBy values</span></span>

<span data-ttu-id="36dc8-122">Für die Eigenschaft **sortBy** sind die folgenden Werte definiert:</span><span class="sxs-lookup"><span data-stu-id="36dc8-122">The following values are defined for the **sortBy** property.</span></span>

| <span data-ttu-id="36dc8-123">Wert</span><span class="sxs-lookup"><span data-stu-id="36dc8-123">Value</span></span>                    | <span data-ttu-id="36dc8-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="36dc8-124">Description</span></span>
| ------------------------ | --------------------------------------------------
| `default`                | <span data-ttu-id="36dc8-125">Dieser Wert steht für die Standardsortierreihenfolge der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="36dc8-125">The default sort order of the application.</span></span>
| `name`                   | <span data-ttu-id="36dc8-126">Elemente sollen auf Basis ihrer Eigenschaft **name** sortiert werden.</span><span class="sxs-lookup"><span data-stu-id="36dc8-126">Items should be arranged by the **name** property of the items.</span></span>
| `type`                   | <span data-ttu-id="36dc8-127">Elemente sollen auf Basis des Elementtyps sortiert werden.</span><span class="sxs-lookup"><span data-stu-id="36dc8-127">Items should be arranged by the type of item.</span></span>
| `size`                   | <span data-ttu-id="36dc8-128">Elemente sollen auf Basis ihrer Eigenschaft **size** sortiert werden.</span><span class="sxs-lookup"><span data-stu-id="36dc8-128">Items should be arranged by the **size** property of the items.</span></span>
| `takenOrCreatedDateTime` | <span data-ttu-id="36dc8-129">Elemente sollen auf Basis der Eigenschaft **takenDateTime** des Facet **photo** sortiert werden.</span><span class="sxs-lookup"><span data-stu-id="36dc8-129">Items should be arranged by the **takenDateTime** property of the **photo** facet.</span></span> <span data-ttu-id="36dc8-130">Ist diese nicht verfügbar, soll die Eigenschaft **createdDateTime** verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="36dc8-130">If not available, the **createdDateTime** property should be used.</span></span>
| `lastModifiedDateTime`   | <span data-ttu-id="36dc8-131">Elemente sollen auf Basis ihrer Eigenschaft **lastModifiedDateTime** sortiert werden.</span><span class="sxs-lookup"><span data-stu-id="36dc8-131">Items should be arranged by the **lastModifiedDateTime** property of the items.</span></span>
| `sequence`               | <span data-ttu-id="36dc8-132">Die Elemente folgen einer vom Benutzer angegebenen benutzerdefinierten Sequenz.</span><span class="sxs-lookup"><span data-stu-id="36dc8-132">Items follow a custom sequence specified by the user.</span></span>


### <a name="sortorder-values"></a><span data-ttu-id="36dc8-133">sortOrder-Werte</span><span class="sxs-lookup"><span data-stu-id="36dc8-133">sortOrder values</span></span>

<span data-ttu-id="36dc8-134">Für die Eigenschaft **sortOrder** sind die folgenden Werte definiert:</span><span class="sxs-lookup"><span data-stu-id="36dc8-134">The following values are defined for the **sortOrder** property.</span></span>

| <span data-ttu-id="36dc8-135">Wert</span><span class="sxs-lookup"><span data-stu-id="36dc8-135">Value</span></span>        | <span data-ttu-id="36dc8-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="36dc8-136">Description</span></span>
| ------------ | --------------------------------------------------------------
| `ascending`  | <span data-ttu-id="36dc8-137">Elemente sollen in aufsteigender Reihenfolge sortiert werden.</span><span class="sxs-lookup"><span data-stu-id="36dc8-137">Items should be arranged in ascending order.</span></span>
| `descending` | <span data-ttu-id="36dc8-138">Elemente sollen in absteigender Reihenfolge sortiert werden.</span><span class="sxs-lookup"><span data-stu-id="36dc8-138">Items should be arranged in descending order.</span></span>


### <a name="viewtype-values"></a><span data-ttu-id="36dc8-139">Werte für „viewType“</span><span class="sxs-lookup"><span data-stu-id="36dc8-139">viewType values</span></span>

<span data-ttu-id="36dc8-140">Für die Eigenschaft **viewType** sind die folgenden Werte definiert:</span><span class="sxs-lookup"><span data-stu-id="36dc8-140">The following values are defined for the **viewType** property.</span></span>

| <span data-ttu-id="36dc8-141">Wert</span><span class="sxs-lookup"><span data-stu-id="36dc8-141">Value</span></span>        | <span data-ttu-id="36dc8-142">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="36dc8-142">Description</span></span>
| ------------ | --------------------------------------------------------------
| `default`    | <span data-ttu-id="36dc8-143">Der Standardansichtstyp der Anwendung</span><span class="sxs-lookup"><span data-stu-id="36dc8-143">The default view type for the application.</span></span>
| `icons`      | <span data-ttu-id="36dc8-144">Eine Ansicht, die Ressourcen des Typs „driveItem“ als Symbole darstellt</span><span class="sxs-lookup"><span data-stu-id="36dc8-144">A view that uses icons to represent driveItems.</span></span>
| `details`    | <span data-ttu-id="36dc8-145">Eine Ansicht mit mehreren Spalten, die zusätzliche Details zu den einzelnen Elementen enthalten</span><span class="sxs-lookup"><span data-stu-id="36dc8-145">A view with multiple columns that provide additional details about each item.</span></span>
| `thumbnails` | <span data-ttu-id="36dc8-146">Eine Ansicht, die Elemente als größere Miniaturansichten von Ressourcen des Typs „driveItem“ darstellt</span><span class="sxs-lookup"><span data-stu-id="36dc8-146">A view that uses larger thumbnails of driveItems to represent the items.</span></span>


[item-resource]: driveitem.md
[folder-facet]: folder.md

<!-- uuid: f9e446fd-190b-4692-a605-bb60e78f1f19
2017-05-03 02:34:40 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "folderView resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/folderview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
