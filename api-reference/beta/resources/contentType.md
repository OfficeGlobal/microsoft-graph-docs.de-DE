---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ContentType
ms.openlocfilehash: cda50c2f20df14c733d3bf71e1b84d5b0df225a0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064610"
---
# <a name="contenttype-resource-type"></a><span data-ttu-id="34759-102">ContentType-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="34759-102">ContentType resource type</span></span>

> <span data-ttu-id="34759-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="34759-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="34759-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="34759-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="34759-105">Die **ContentType**-Ressource stellt einen _Inhaltstyp_ in SharePoint dar.</span><span class="sxs-lookup"><span data-stu-id="34759-105">The **contentType** resource represents a _content type_ in SharePoint.</span></span>
<span data-ttu-id="34759-106">Mit Inhaltstypen können Sie eine Reihe von Spalten definieren, die auf jedem [ **ListItem** ] [ listItem] in einer [ **Liste** ] [list] vorhanden sein müssen.</span><span class="sxs-lookup"><span data-stu-id="34759-106">Content types allow you to define a set of columns that must be present on every [**listItem**][listItem] in a [**list**][list].</span></span>

[list]: list.md
[listItem]: listitem.md

## <a name="json-representation"></a><span data-ttu-id="34759-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="34759-107">JSON representation</span></span>

<span data-ttu-id="34759-108">Es folgt eine JSON-Darstellung einer **contentType**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="34759-108">Here is a JSON representation of a **contentType** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.contentType" } -->

```json
{
  "description": "string",
  "group": "string",
  "hidden": false,
  "id": "string",
  "inheritedFrom": { "@type": "microsoft.graph.itemReference" },
  "name": "string",
  "order": { "@type": "microsoft.graph.contentTypeOrder" },
  "parentId": "string",
  "readOnly": false,
  "sealed": false,

  "columnLinks": [{ "@type": "microsoft.graph.columnLink" }]
}
```

## <a name="properties"></a><span data-ttu-id="34759-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="34759-109">Properties</span></span>

| <span data-ttu-id="34759-110">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="34759-110">Property name</span></span>     | <span data-ttu-id="34759-111">Typ</span><span class="sxs-lookup"><span data-stu-id="34759-111">Type</span></span>                 | <span data-ttu-id="34759-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="34759-112">Description</span></span>
|:------------------|:---------------------|:----------------------------------
| <span data-ttu-id="34759-113">**description**</span><span class="sxs-lookup"><span data-stu-id="34759-113">**description**</span></span>   | <span data-ttu-id="34759-114">string</span><span class="sxs-lookup"><span data-stu-id="34759-114">string</span></span>               | <span data-ttu-id="34759-115">Der beschreibende Text für das Element.</span><span class="sxs-lookup"><span data-stu-id="34759-115">The descriptive text for the item.</span></span>
| <span data-ttu-id="34759-116">**group**</span><span class="sxs-lookup"><span data-stu-id="34759-116">**group**</span></span>         | <span data-ttu-id="34759-117">string</span><span class="sxs-lookup"><span data-stu-id="34759-117">string</span></span>               | <span data-ttu-id="34759-118">Der Name der Gruppe, der dieser Inhaltstyp angehört.</span><span class="sxs-lookup"><span data-stu-id="34759-118">The name of the group this content type belongs to.</span></span> <span data-ttu-id="34759-119">Dadurch können dazugehörige Inhaltstypen einfacher organisiert werden.</span><span class="sxs-lookup"><span data-stu-id="34759-119">Helps organize related content types.</span></span>
| <span data-ttu-id="34759-120">**hidden**</span><span class="sxs-lookup"><span data-stu-id="34759-120">**hidden**</span></span>        | <span data-ttu-id="34759-121">boolean</span><span class="sxs-lookup"><span data-stu-id="34759-121">boolean</span></span>              | <span data-ttu-id="34759-122">Gibt an, ob der Inhaltstyp im Menü 'Neu' der Liste ausgeblendet ist.</span><span class="sxs-lookup"><span data-stu-id="34759-122">Indicates whether the content type is hidden in the list's 'New' menu.</span></span>
| <span data-ttu-id="34759-123">**id**</span><span class="sxs-lookup"><span data-stu-id="34759-123">**id**</span></span>            | <span data-ttu-id="34759-124">string</span><span class="sxs-lookup"><span data-stu-id="34759-124">string</span></span>               | <span data-ttu-id="34759-125">Der eindeutige Bezeichner des Inhaltstyps.</span><span class="sxs-lookup"><span data-stu-id="34759-125">The unique identifier of the content type.</span></span>
| <span data-ttu-id="34759-126">**inheritedFrom**</span><span class="sxs-lookup"><span data-stu-id="34759-126">**inheritedFrom**</span></span> | <span data-ttu-id="34759-127">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="34759-127">[itemReference][]</span></span>    | <span data-ttu-id="34759-128">Wenn dieses Inhaltstyps aus einem anderen Bereich (z. B. eine Website) übernommen wurde, wird ein Verweis auf das Element angezeigt, in dem der Inhaltstyp definiert ist.</span><span class="sxs-lookup"><span data-stu-id="34759-128">If this content type is inherited from another scope (like a site), provides a reference to the item where the content type is defined.</span></span>
| <span data-ttu-id="34759-129">**name**</span><span class="sxs-lookup"><span data-stu-id="34759-129">**name**</span></span>          | <span data-ttu-id="34759-130">string</span><span class="sxs-lookup"><span data-stu-id="34759-130">string</span></span>               | <span data-ttu-id="34759-131">Der Name des Inhaltstyps.</span><span class="sxs-lookup"><span data-stu-id="34759-131">The name of the content type.</span></span>
| <span data-ttu-id="34759-132">**order**</span><span class="sxs-lookup"><span data-stu-id="34759-132">**order**</span></span>         | <span data-ttu-id="34759-133">[contentTypeOrder][]</span><span class="sxs-lookup"><span data-stu-id="34759-133">[contentTypeOrder][]</span></span> | <span data-ttu-id="34759-134">Gibt die Reihenfolge, in welcher der Inhaltstyp in der Auswahl-Benutzeroberfläche angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="34759-134">Specifies the order in which the content type appears in the selection UI.</span></span>
| <span data-ttu-id="34759-135">**parentId**</span><span class="sxs-lookup"><span data-stu-id="34759-135">**parentId**</span></span>      | <span data-ttu-id="34759-136">string</span><span class="sxs-lookup"><span data-stu-id="34759-136">string</span></span>               | <span data-ttu-id="34759-137">Der eindeutige Bezeichner des Inhaltstyps.</span><span class="sxs-lookup"><span data-stu-id="34759-137">The unique identifier of the content type.</span></span>
| <span data-ttu-id="34759-138">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="34759-138">**readOnly**</span></span>      | <span data-ttu-id="34759-139">boolean</span><span class="sxs-lookup"><span data-stu-id="34759-139">boolean</span></span>              | <span data-ttu-id="34759-140">`true` gibt an, dass der Inhaltstyp erst geändert werden kann, nachdem der Wert auf `false` festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="34759-140">If `true`, the content type cannot be modified unless this value is first set to `false`.</span></span>
| <span data-ttu-id="34759-141">**sealed**</span><span class="sxs-lookup"><span data-stu-id="34759-141">**sealed**</span></span>        | <span data-ttu-id="34759-142">boolean</span><span class="sxs-lookup"><span data-stu-id="34759-142">boolean</span></span>              | <span data-ttu-id="34759-143">`true` gibt an, dass der Inhaltstyp nicht von Benutzern oder über Push-Down-Vorgänge geändert werden kann.</span><span class="sxs-lookup"><span data-stu-id="34759-143">If `true`, the content type cannot be modified by users or through push-down operations.</span></span> <span data-ttu-id="34759-144">Nur Websitesammlungsadministratoren können Inhaltstypen versiegeln oder entsiegeln.</span><span class="sxs-lookup"><span data-stu-id="34759-144">Only site collection administrators can seal or unseal content types.</span></span>

## <a name="relationships"></a><span data-ttu-id="34759-145">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="34759-145">Relationships</span></span>

| <span data-ttu-id="34759-146">Eigenschaftsname</span><span class="sxs-lookup"><span data-stu-id="34759-146">Property name</span></span>   | <span data-ttu-id="34759-147">Typ</span><span class="sxs-lookup"><span data-stu-id="34759-147">Type</span></span>                      | <span data-ttu-id="34759-148">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="34759-148">Description</span></span>
|:----------------|:--------------------------|:-------------------------------
| <span data-ttu-id="34759-149">**columnLinks**</span><span class="sxs-lookup"><span data-stu-id="34759-149">**columnLinks**</span></span> | <span data-ttu-id="34759-150">[columnLink][]-Sammlung</span><span class="sxs-lookup"><span data-stu-id="34759-150">[columnLink][] collection</span></span> | <span data-ttu-id="34759-151">Die Sammlung von Spalten, die für diesen Inhaltstyp erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="34759-151">The collection of columns that are required by this content type</span></span>

<span data-ttu-id="34759-152">Weitere Informationen finden Sie unter [Einführung in Inhaltstypen und die Inhaltstypveröffentlichung][contentTypeIntro].</span><span class="sxs-lookup"><span data-stu-id="34759-152">See [Introduction to content types and content type publishing][contentTypeIntro] for more information.</span></span>

[columnLink]: columnlink.md
[contentTypeIntro]: https://support.office.com/en-us/article/Introduction-to-content-types-and-content-type-publishing-e1277a2e-a1e8-4473-9126-91a0647766e5
[itemReference]: itemreference.md
[contentTypeOrder]: contenttypeorder.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentType"
} -->
