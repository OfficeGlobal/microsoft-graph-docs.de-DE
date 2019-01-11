---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ContentType
localization_priority: Normal
ms.openlocfilehash: c7d4b3222ec64432d6a2c9921e53ce409de3f139
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876734"
---
# <a name="contenttype-resource-type"></a><span data-ttu-id="3890d-102">ContentType-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="3890d-102">ContentType resource type</span></span>

<span data-ttu-id="3890d-103">Die **ContentType**-Ressource stellt einen _Inhaltstyp_ in SharePoint dar.</span><span class="sxs-lookup"><span data-stu-id="3890d-103">The **contentType** resource represents a _content type_ in SharePoint.</span></span>
<span data-ttu-id="3890d-104">Mit Inhaltstypen können Sie eine Reihe von Spalten definieren, die auf jedem [ **ListItem** ] [ listItem] in einer [ **Liste** ] [list] vorhanden sein müssen.</span><span class="sxs-lookup"><span data-stu-id="3890d-104">Content types allow you to define a set of columns that must be present on every [**listItem**][listItem] in a [**list**][list].</span></span>

[list]: list.md
[listItem]: listitem.md

## <a name="json-representation"></a><span data-ttu-id="3890d-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3890d-105">JSON representation</span></span>

<span data-ttu-id="3890d-106">Es folgt eine JSON-Darstellung einer **contentType**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="3890d-106">Here is a JSON representation of a **contentType** resource.</span></span>
<!-- {
  "blockType": "resource",
 "baseType": "microsoft.graph.entity",
 "@odata.type": "microsoft.graph.contentType" } -->

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

## <a name="properties"></a><span data-ttu-id="3890d-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3890d-107">Properties</span></span>

| <span data-ttu-id="3890d-108">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="3890d-108">Property name</span></span>     | <span data-ttu-id="3890d-109">Typ</span><span class="sxs-lookup"><span data-stu-id="3890d-109">Type</span></span>                 | <span data-ttu-id="3890d-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3890d-110">Description</span></span>
|:------------------|:---------------------|:----------------------------------
| <span data-ttu-id="3890d-111">**description**</span><span class="sxs-lookup"><span data-stu-id="3890d-111">**description**</span></span>   | <span data-ttu-id="3890d-112">string</span><span class="sxs-lookup"><span data-stu-id="3890d-112">string</span></span>               | <span data-ttu-id="3890d-113">Der beschreibende Text für das Element.</span><span class="sxs-lookup"><span data-stu-id="3890d-113">The descriptive text for the item.</span></span>
| <span data-ttu-id="3890d-114">**group**</span><span class="sxs-lookup"><span data-stu-id="3890d-114">**group**</span></span>         | <span data-ttu-id="3890d-115">string</span><span class="sxs-lookup"><span data-stu-id="3890d-115">string</span></span>               | <span data-ttu-id="3890d-116">Der Name der Gruppe, der dieser Inhaltstyp angehört.</span><span class="sxs-lookup"><span data-stu-id="3890d-116">The name of the group this content type belongs to.</span></span> <span data-ttu-id="3890d-117">Dadurch können dazugehörige Inhaltstypen einfacher organisiert werden.</span><span class="sxs-lookup"><span data-stu-id="3890d-117">Helps organize related content types.</span></span>
| <span data-ttu-id="3890d-118">**hidden**</span><span class="sxs-lookup"><span data-stu-id="3890d-118">**hidden**</span></span>        | <span data-ttu-id="3890d-119">boolean</span><span class="sxs-lookup"><span data-stu-id="3890d-119">boolean</span></span>              | <span data-ttu-id="3890d-120">Gibt an, ob der Inhaltstyp im Menü 'Neu' der Liste ausgeblendet ist.</span><span class="sxs-lookup"><span data-stu-id="3890d-120">Indicates whether the content type is hidden in the list's 'New' menu.</span></span>
| <span data-ttu-id="3890d-121">**id**</span><span class="sxs-lookup"><span data-stu-id="3890d-121">**id**</span></span>            | <span data-ttu-id="3890d-122">string</span><span class="sxs-lookup"><span data-stu-id="3890d-122">string</span></span>               | <span data-ttu-id="3890d-123">Der eindeutige Bezeichner des Inhaltstyps.</span><span class="sxs-lookup"><span data-stu-id="3890d-123">The unique identifier of the content type.</span></span>
| <span data-ttu-id="3890d-124">**inheritedFrom**</span><span class="sxs-lookup"><span data-stu-id="3890d-124">**inheritedFrom**</span></span> | <span data-ttu-id="3890d-125">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="3890d-125">[itemReference][]</span></span>    | <span data-ttu-id="3890d-126">Wenn dieses Inhaltstyps aus einem anderen Bereich (z. B. eine Website) übernommen wurde, wird ein Verweis auf das Element angezeigt, in dem der Inhaltstyp definiert ist.</span><span class="sxs-lookup"><span data-stu-id="3890d-126">If this content type is inherited from another scope (like a site), provides a reference to the item where the content type is defined.</span></span>
| <span data-ttu-id="3890d-127">**name**</span><span class="sxs-lookup"><span data-stu-id="3890d-127">**name**</span></span>          | <span data-ttu-id="3890d-128">string</span><span class="sxs-lookup"><span data-stu-id="3890d-128">string</span></span>               | <span data-ttu-id="3890d-129">Der Name des Inhaltstyps.</span><span class="sxs-lookup"><span data-stu-id="3890d-129">The name of the content type.</span></span>
| <span data-ttu-id="3890d-130">**order**</span><span class="sxs-lookup"><span data-stu-id="3890d-130">**order**</span></span>         | <span data-ttu-id="3890d-131">[contentTypeOrder][]</span><span class="sxs-lookup"><span data-stu-id="3890d-131">[contentTypeOrder][]</span></span> | <span data-ttu-id="3890d-132">Gibt die Reihenfolge, in welcher der Inhaltstyp in der Auswahl-Benutzeroberfläche angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="3890d-132">Specifies the order in which the content type appears in the selection UI.</span></span>
| <span data-ttu-id="3890d-133">**parentId**</span><span class="sxs-lookup"><span data-stu-id="3890d-133">**parentId**</span></span>      | <span data-ttu-id="3890d-134">string</span><span class="sxs-lookup"><span data-stu-id="3890d-134">string</span></span>               | <span data-ttu-id="3890d-135">Der eindeutige Bezeichner des Inhaltstyps.</span><span class="sxs-lookup"><span data-stu-id="3890d-135">The unique identifier of the content type.</span></span>
| <span data-ttu-id="3890d-136">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="3890d-136">**readOnly**</span></span>      | <span data-ttu-id="3890d-137">boolean</span><span class="sxs-lookup"><span data-stu-id="3890d-137">boolean</span></span>              | <span data-ttu-id="3890d-138">`true` gibt an, dass der Inhaltstyp erst geändert werden kann, nachdem der Wert auf `false` festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="3890d-138">If `true`, the content type cannot be modified unless this value is first set to `false`.</span></span>
| <span data-ttu-id="3890d-139">**sealed**</span><span class="sxs-lookup"><span data-stu-id="3890d-139">**sealed**</span></span>        | <span data-ttu-id="3890d-140">boolean</span><span class="sxs-lookup"><span data-stu-id="3890d-140">boolean</span></span>              | <span data-ttu-id="3890d-141">`true` gibt an, dass der Inhaltstyp nicht von Benutzern oder über Push-Down-Vorgänge geändert werden kann.</span><span class="sxs-lookup"><span data-stu-id="3890d-141">If `true`, the content type cannot be modified by users or through push-down operations.</span></span> <span data-ttu-id="3890d-142">Nur Websitesammlungsadministratoren können Inhaltstypen versiegeln oder entsiegeln.</span><span class="sxs-lookup"><span data-stu-id="3890d-142">Only site collection administrators can seal or unseal content types.</span></span>

## <a name="relationships"></a><span data-ttu-id="3890d-143">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="3890d-143">Relationships</span></span>

| <span data-ttu-id="3890d-144">Eigenschaftsname</span><span class="sxs-lookup"><span data-stu-id="3890d-144">Property name</span></span>   | <span data-ttu-id="3890d-145">Typ</span><span class="sxs-lookup"><span data-stu-id="3890d-145">Type</span></span>                      | <span data-ttu-id="3890d-146">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3890d-146">Description</span></span>
|:----------------|:--------------------------|:-------------------------------
| <span data-ttu-id="3890d-147">**columnLinks**</span><span class="sxs-lookup"><span data-stu-id="3890d-147">**columnLinks**</span></span> | <span data-ttu-id="3890d-148">[columnLink][]-Sammlung</span><span class="sxs-lookup"><span data-stu-id="3890d-148">[columnLink][] collection</span></span> | <span data-ttu-id="3890d-149">Die Sammlung von Spalten, die für diesen Inhaltstyp erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="3890d-149">The collection of columns that are required by this content type</span></span>

<span data-ttu-id="3890d-150">Weitere Informationen finden Sie unter [Einführung in Inhaltstypen und die Inhaltstypveröffentlichung][contentTypeIntro].</span><span class="sxs-lookup"><span data-stu-id="3890d-150">See [Introduction to content types and content type publishing][contentTypeIntro] for more information.</span></span>

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
