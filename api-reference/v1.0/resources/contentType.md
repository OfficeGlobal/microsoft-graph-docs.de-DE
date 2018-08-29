---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ContentType
ms.openlocfilehash: cb16559aa9da3a885be1977bbd1466265d0a72f0
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/21/2018
ms.locfileid: "23268333"
---
# <a name="contenttype-resource-type"></a><span data-ttu-id="bbe24-102">ContentType-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="bbe24-102">ContentType resource type</span></span>

<span data-ttu-id="bbe24-103">Die **ContentType**-Ressource stellt einen _Inhaltstyp_ in SharePoint dar.</span><span class="sxs-lookup"><span data-stu-id="bbe24-103">The **contentType** resource represents a _content type_ in SharePoint.</span></span>
<span data-ttu-id="bbe24-104">Mit Inhaltstypen können Sie eine Reihe von Spalten definieren, die auf jedem [ **ListItem** ] [ listItem] in einer [ **Liste** ] [list] vorhanden sein müssen.</span><span class="sxs-lookup"><span data-stu-id="bbe24-104">Content types allow you to define a set of columns that must be present on every [**listItem**][listItem] in a [**list**][list].</span></span>

[list]: list.md
[listItem]: listItem.md

## <a name="json-representation"></a><span data-ttu-id="bbe24-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bbe24-105">JSON representation</span></span>

<span data-ttu-id="bbe24-106">Es folgt eine JSON-Darstellung einer **contentType**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="bbe24-106">Here is a JSON representation of a **contentType** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="bbe24-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bbe24-107">Properties</span></span>

| <span data-ttu-id="bbe24-108">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="bbe24-108">Property name</span></span>     | <span data-ttu-id="bbe24-109">Typ</span><span class="sxs-lookup"><span data-stu-id="bbe24-109">Type</span></span>                 | <span data-ttu-id="bbe24-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bbe24-110">Description</span></span>
|:------------------|:---------------------|:----------------------------------
| <span data-ttu-id="bbe24-111">**description**</span><span class="sxs-lookup"><span data-stu-id="bbe24-111">**description**</span></span>   | <span data-ttu-id="bbe24-112">string</span><span class="sxs-lookup"><span data-stu-id="bbe24-112">string</span></span>               | <span data-ttu-id="bbe24-113">Der beschreibende Text für das Element.</span><span class="sxs-lookup"><span data-stu-id="bbe24-113">The descriptive text for the item.</span></span>
| <span data-ttu-id="bbe24-114">**group**</span><span class="sxs-lookup"><span data-stu-id="bbe24-114">**group**</span></span>         | <span data-ttu-id="bbe24-115">string</span><span class="sxs-lookup"><span data-stu-id="bbe24-115">string</span></span>               | <span data-ttu-id="bbe24-116">Der Name der Gruppe, der dieser Inhaltstyp angehört.</span><span class="sxs-lookup"><span data-stu-id="bbe24-116">The name of the group this content type belongs to.</span></span> <span data-ttu-id="bbe24-117">Dadurch können dazugehörige Inhaltstypen einfacher organisiert werden.</span><span class="sxs-lookup"><span data-stu-id="bbe24-117">Helps organize related content types.</span></span>
| <span data-ttu-id="bbe24-118">**hidden**</span><span class="sxs-lookup"><span data-stu-id="bbe24-118">**hidden**</span></span>        | <span data-ttu-id="bbe24-119">boolean</span><span class="sxs-lookup"><span data-stu-id="bbe24-119">boolean</span></span>              | <span data-ttu-id="bbe24-120">Gibt an, ob der Inhaltstyp im Menü 'Neu' der Liste ausgeblendet ist.</span><span class="sxs-lookup"><span data-stu-id="bbe24-120">Indicates whether the content type is hidden in the list's 'New' menu.</span></span>
| <span data-ttu-id="bbe24-121">**ID**</span><span class="sxs-lookup"><span data-stu-id="bbe24-121">**id**</span></span>            | <span data-ttu-id="bbe24-122">string</span><span class="sxs-lookup"><span data-stu-id="bbe24-122">string</span></span>               | <span data-ttu-id="bbe24-123">Der eindeutige Bezeichner des Inhaltstyps.</span><span class="sxs-lookup"><span data-stu-id="bbe24-123">The unique identifier of the content type.</span></span>
| <span data-ttu-id="bbe24-124">**inheritedFrom**</span><span class="sxs-lookup"><span data-stu-id="bbe24-124">**inheritedFrom**</span></span> | <span data-ttu-id="bbe24-125">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="bbe24-125">[itemReference][]</span></span>    | <span data-ttu-id="bbe24-126">Wenn dieses Inhaltstyps aus einem anderen Bereich (z. B. eine Website) übernommen wurde, wird ein Verweis auf das Element angezeigt, in dem der Inhaltstyp definiert ist.</span><span class="sxs-lookup"><span data-stu-id="bbe24-126">If this content type is inherited from another scope (like a site), provides a reference to the item where the content type is defined.</span></span>
| <span data-ttu-id="bbe24-127">**name**</span><span class="sxs-lookup"><span data-stu-id="bbe24-127">**name**</span></span>          | <span data-ttu-id="bbe24-128">string</span><span class="sxs-lookup"><span data-stu-id="bbe24-128">string</span></span>               | <span data-ttu-id="bbe24-129">Der Name des Inhaltstyps.</span><span class="sxs-lookup"><span data-stu-id="bbe24-129">The name of the content type.</span></span>
| <span data-ttu-id="bbe24-130">**order**</span><span class="sxs-lookup"><span data-stu-id="bbe24-130">**order**</span></span>         | <span data-ttu-id="bbe24-131">[contentTypeOrder][]</span><span class="sxs-lookup"><span data-stu-id="bbe24-131">[contentTypeOrder][]</span></span> | <span data-ttu-id="bbe24-132">Gibt die Reihenfolge, in welcher der Inhaltstyp in der Auswahl-Benutzeroberfläche angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="bbe24-132">Specifies the order in which the content type appears in the selection UI.</span></span>
| <span data-ttu-id="bbe24-133">**parentId**</span><span class="sxs-lookup"><span data-stu-id="bbe24-133">**parentId**</span></span>      | <span data-ttu-id="bbe24-134">string</span><span class="sxs-lookup"><span data-stu-id="bbe24-134">string</span></span>               | <span data-ttu-id="bbe24-135">Der eindeutige Bezeichner des Inhaltstyps.</span><span class="sxs-lookup"><span data-stu-id="bbe24-135">The unique identifier of the content type.</span></span>
| <span data-ttu-id="bbe24-136">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="bbe24-136">**readOnly**</span></span>      | <span data-ttu-id="bbe24-137">boolean</span><span class="sxs-lookup"><span data-stu-id="bbe24-137">boolean</span></span>              | <span data-ttu-id="bbe24-138">gibt an, dass der Inhaltstyp erst geändert werden kann, nachdem der Wert auf `false` festgelegt wurde.`true`</span><span class="sxs-lookup"><span data-stu-id="bbe24-138">If `true`, the content type cannot be modified unless this value is first set to `false`.</span></span>
| <span data-ttu-id="bbe24-139">**sealed**</span><span class="sxs-lookup"><span data-stu-id="bbe24-139">**sealed**</span></span>        | <span data-ttu-id="bbe24-140">boolean</span><span class="sxs-lookup"><span data-stu-id="bbe24-140">boolean</span></span>              | <span data-ttu-id="bbe24-141">gibt an, dass der Inhaltstyp nicht von Benutzern oder über Push-Down-Vorgänge geändert werden kann.`true`</span><span class="sxs-lookup"><span data-stu-id="bbe24-141">If `true`, the content type cannot be modified by users or through push-down operations.</span></span> <span data-ttu-id="bbe24-142">Nur Websitesammlungsadministratoren können Inhaltstypen versiegeln oder entsiegeln.</span><span class="sxs-lookup"><span data-stu-id="bbe24-142">Only site collection administrators can seal or unseal content types.</span></span>

## <a name="relationships"></a><span data-ttu-id="bbe24-143">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="bbe24-143">Relationships</span></span>

| <span data-ttu-id="bbe24-144">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="bbe24-144">Property name</span></span>   | <span data-ttu-id="bbe24-145">Typ</span><span class="sxs-lookup"><span data-stu-id="bbe24-145">Type</span></span>                      | <span data-ttu-id="bbe24-146">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bbe24-146">Description</span></span>
|:----------------|:--------------------------|:-------------------------------
| <span data-ttu-id="bbe24-147">**columnLinks**</span><span class="sxs-lookup"><span data-stu-id="bbe24-147">**columnLinks**</span></span> | <span data-ttu-id="bbe24-148">[columnLink][]-Sammlung</span><span class="sxs-lookup"><span data-stu-id="bbe24-148">[columnLink][] collection</span></span> | <span data-ttu-id="bbe24-149">Die Sammlung von Spalten, die für diesen Inhaltstyp erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="bbe24-149">The collection of columns that are required by this content type</span></span>

<span data-ttu-id="bbe24-150">Weitere Informationen finden Sie unter [Einführung in Inhaltstypen und die Inhaltstypveröffentlichung][contentTypeIntro].</span><span class="sxs-lookup"><span data-stu-id="bbe24-150">See [Introduction to content types and content type publishing][contentTypeIntro] for more information.</span></span>

[columnLink]: columnLink.md
[contentTypeIntro]: https://support.office.com/en-us/article/Introduction-to-content-types-and-content-type-publishing-e1277a2e-a1e8-4473-9126-91a0647766e5
[itemReference]: itemReference.md
[contentTypeOrder]: contentTypeOrder.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentType"
} -->
