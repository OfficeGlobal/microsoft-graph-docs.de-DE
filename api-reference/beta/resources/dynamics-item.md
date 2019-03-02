---
title: Ressourcentyp "Items"
description: Ein Item-Objekt in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 42ec7720e2e858f319beab8576fbe57542dd470c
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365962"
---
# <a name="items-resource-type"></a><span data-ttu-id="7c02c-103">Ressourcentyp "Items"</span><span class="sxs-lookup"><span data-stu-id="7c02c-103">items resource type</span></span>
<span data-ttu-id="7c02c-104">Stellt ein Element in Dynamics 365 Business Central dar.</span><span class="sxs-lookup"><span data-stu-id="7c02c-104">Represents an item in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="7c02c-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="7c02c-105">Methods</span></span>

| <span data-ttu-id="7c02c-106">Methode</span><span class="sxs-lookup"><span data-stu-id="7c02c-106">Method</span></span>                                      |<span data-ttu-id="7c02c-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="7c02c-107">Return Type</span></span>|<span data-ttu-id="7c02c-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7c02c-108">Description</span></span> |
|:--------------------------------------------|:----------|:-----------|
|[<span data-ttu-id="7c02c-109">Elemente abrufen</span><span class="sxs-lookup"><span data-stu-id="7c02c-109">Get items</span></span>](../api/dynamics-item-get.md)      |<span data-ttu-id="7c02c-110">Elemente</span><span class="sxs-lookup"><span data-stu-id="7c02c-110">items</span></span>     |<span data-ttu-id="7c02c-111">Ruft ein Item-Objekt ab.</span><span class="sxs-lookup"><span data-stu-id="7c02c-111">Gets an item object.</span></span>   |
|[<span data-ttu-id="7c02c-112">Bereitstellungselemente</span><span class="sxs-lookup"><span data-stu-id="7c02c-112">Post items</span></span>](../api/dynamics-create-item.md)  |<span data-ttu-id="7c02c-113">Elemente</span><span class="sxs-lookup"><span data-stu-id="7c02c-113">items</span></span>     |<span data-ttu-id="7c02c-114">Erstellt ein Item-Objekt.</span><span class="sxs-lookup"><span data-stu-id="7c02c-114">Creates an item object.</span></span>|
|[<span data-ttu-id="7c02c-115">Patchelement</span><span class="sxs-lookup"><span data-stu-id="7c02c-115">Patch item</span></span>](../api/dynamics-item-update.md)  |<span data-ttu-id="7c02c-116">Elemente</span><span class="sxs-lookup"><span data-stu-id="7c02c-116">items</span></span>     |<span data-ttu-id="7c02c-117">Aktualisiert ein Item-Objekt.</span><span class="sxs-lookup"><span data-stu-id="7c02c-117">Updates an item object.</span></span>|
|[<span data-ttu-id="7c02c-118">Löschen von Elementen</span><span class="sxs-lookup"><span data-stu-id="7c02c-118">Delete items</span></span>](../api/dynamics-item-delete.md)|<span data-ttu-id="7c02c-119">Keine</span><span class="sxs-lookup"><span data-stu-id="7c02c-119">none</span></span>      |<span data-ttu-id="7c02c-120">Löscht ein Item-Objekt.</span><span class="sxs-lookup"><span data-stu-id="7c02c-120">Deletes an item object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7c02c-121">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7c02c-121">Properties</span></span>
| <span data-ttu-id="7c02c-122">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7c02c-122">Property</span></span>           | <span data-ttu-id="7c02c-123">Typ</span><span class="sxs-lookup"><span data-stu-id="7c02c-123">Type</span></span> |<span data-ttu-id="7c02c-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7c02c-124">Description</span></span>                                          |
|:-------------------|:-------|:----------------------------------------------------|
|<span data-ttu-id="7c02c-125">id</span><span class="sxs-lookup"><span data-stu-id="7c02c-125">id</span></span>                  |<span data-ttu-id="7c02c-126">GUID</span><span class="sxs-lookup"><span data-stu-id="7c02c-126">GUID</span></span>    |<span data-ttu-id="7c02c-127">Die eindeutige ID des Elements.</span><span class="sxs-lookup"><span data-stu-id="7c02c-127">The unique ID of the item.</span></span> <span data-ttu-id="7c02c-128">Nicht bearbeitbar.</span><span class="sxs-lookup"><span data-stu-id="7c02c-128">Non-editable.</span></span>             |
|<span data-ttu-id="7c02c-129">number</span><span class="sxs-lookup"><span data-stu-id="7c02c-129">number</span></span>              |<span data-ttu-id="7c02c-130">string</span><span class="sxs-lookup"><span data-stu-id="7c02c-130">string</span></span>  |<span data-ttu-id="7c02c-131">Die Artikelnummer.</span><span class="sxs-lookup"><span data-stu-id="7c02c-131">The item number.</span></span>                                     |
|<span data-ttu-id="7c02c-132">displayName</span><span class="sxs-lookup"><span data-stu-id="7c02c-132">displayName</span></span>         |<span data-ttu-id="7c02c-133">string</span><span class="sxs-lookup"><span data-stu-id="7c02c-133">string</span></span>  |<span data-ttu-id="7c02c-134">Gibt eine Beschreibung des Elements an.</span><span class="sxs-lookup"><span data-stu-id="7c02c-134">Specifies a description of the item.</span></span>                 |
|<span data-ttu-id="7c02c-135">type</span><span class="sxs-lookup"><span data-stu-id="7c02c-135">type</span></span>                |<span data-ttu-id="7c02c-136">numerischen</span><span class="sxs-lookup"><span data-stu-id="7c02c-136">numeric</span></span> |<span data-ttu-id="7c02c-137">Der inventurtyp für das Element.</span><span class="sxs-lookup"><span data-stu-id="7c02c-137">The inventory type for the item.</span></span> <span data-ttu-id="7c02c-138">1 = Inventarelement, 2 = Service Element.</span><span class="sxs-lookup"><span data-stu-id="7c02c-138">1 = inventory item, 2 = service item.</span></span> <span data-ttu-id="7c02c-139">Dies ist eine erforderliche Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="7c02c-139">This is a required property.</span></span>|
|<span data-ttu-id="7c02c-140">gesperrt</span><span class="sxs-lookup"><span data-stu-id="7c02c-140">blocked</span></span>             |<span data-ttu-id="7c02c-141">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="7c02c-141">boolean</span></span> |<span data-ttu-id="7c02c-142">Gibt an, dass Transaktionen mit dem Element nicht gebucht werden können, da sich das Element in der Quarantäne befindet.</span><span class="sxs-lookup"><span data-stu-id="7c02c-142">Specifies that transactions with the item cannot be posted, for example, because the item is in quarantine.</span></span> <span data-ttu-id="7c02c-143">Wird auf **true**festgelegt, wenn item blockiert ist.</span><span class="sxs-lookup"><span data-stu-id="7c02c-143">Set to **true**, if item is blocked.</span></span>|
|<span data-ttu-id="7c02c-144">baseUnitOfMeasureId</span><span class="sxs-lookup"><span data-stu-id="7c02c-144">baseUnitOfMeasureId</span></span> |<span data-ttu-id="7c02c-145">GUID</span><span class="sxs-lookup"><span data-stu-id="7c02c-145">GUID</span></span>    |<span data-ttu-id="7c02c-146">Gibt die ID der Maßeinheit an.</span><span class="sxs-lookup"><span data-stu-id="7c02c-146">Specifies the ID of the unit of measure.</span></span>             |
|<span data-ttu-id="7c02c-147">baseUnitOfMeasure</span><span class="sxs-lookup"><span data-stu-id="7c02c-147">baseUnitOfMeasure</span></span>   |[<span data-ttu-id="7c02c-148">Navigations. UnitOfMeasure</span><span class="sxs-lookup"><span data-stu-id="7c02c-148">NAV.UnitOfMeasure</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="7c02c-149">Gibt die Einheit an, in der das Element im Bestand aufbewahrt wird.</span><span class="sxs-lookup"><span data-stu-id="7c02c-149">Specifies the unit in which the item is held in inventory.</span></span>|
|<span data-ttu-id="7c02c-150">GTIN</span><span class="sxs-lookup"><span data-stu-id="7c02c-150">gtin</span></span>                |<span data-ttu-id="7c02c-151">numerischen</span><span class="sxs-lookup"><span data-stu-id="7c02c-151">numeric</span></span> |<span data-ttu-id="7c02c-152">Dies ist die Nummer des globalen Handels Artikels.</span><span class="sxs-lookup"><span data-stu-id="7c02c-152">This is the Global Trade Item Number.</span></span>                |
|<span data-ttu-id="7c02c-153">itemCategoryId</span><span class="sxs-lookup"><span data-stu-id="7c02c-153">itemCategoryId</span></span>      |<span data-ttu-id="7c02c-154">GUID</span><span class="sxs-lookup"><span data-stu-id="7c02c-154">GUID</span></span> |<span data-ttu-id="7c02c-155">Gibt die Kategorie an, zu der das Element gehört.</span><span class="sxs-lookup"><span data-stu-id="7c02c-155">Specifies the category that the item belongs to.</span></span> <span data-ttu-id="7c02c-156">Elementkategorien enthalten auch alle zugewiesenen Element Attribute.</span><span class="sxs-lookup"><span data-stu-id="7c02c-156">Item categories also contain any assigned item attributes.</span></span>|
|<span data-ttu-id="7c02c-157">inventory</span><span class="sxs-lookup"><span data-stu-id="7c02c-157">inventory</span></span>           |<span data-ttu-id="7c02c-158">decimal</span><span class="sxs-lookup"><span data-stu-id="7c02c-158">decimal</span></span> |<span data-ttu-id="7c02c-159">Gibt an, wie viele Einheiten, wie Teile, Kisten oder Dosen, des Elements im Inventar sind.</span><span class="sxs-lookup"><span data-stu-id="7c02c-159">Specifies how many units, such as pieces, boxes, or cans, of the item are in inventory.</span></span> <span data-ttu-id="7c02c-160">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7c02c-160">Read-Only.</span></span>|
|<span data-ttu-id="7c02c-161">unitPrice</span><span class="sxs-lookup"><span data-stu-id="7c02c-161">unitPrice</span></span>           |<span data-ttu-id="7c02c-162">decimal</span><span class="sxs-lookup"><span data-stu-id="7c02c-162">decimal</span></span> |<span data-ttu-id="7c02c-163">Gibt den Preis für eine Einheit des Elements in der angegebenen Währung an.</span><span class="sxs-lookup"><span data-stu-id="7c02c-163">Specifies the price for one unit of the item in the specified currency.</span></span>|
|<span data-ttu-id="7c02c-164">priceIncludesTax</span><span class="sxs-lookup"><span data-stu-id="7c02c-164">priceIncludesTax</span></span>    |<span data-ttu-id="7c02c-165">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="7c02c-165">boolean</span></span> |<span data-ttu-id="7c02c-166">Gibt an, dass der Einzelpreis Steuern enthält.</span><span class="sxs-lookup"><span data-stu-id="7c02c-166">Specifies that the unitPrice includes tax.</span></span> <span data-ttu-id="7c02c-167">Auf **true**festgelegt, wenn Einzelpreis Steuer enthält.</span><span class="sxs-lookup"><span data-stu-id="7c02c-167">Set to **true**, if unitPrice includes tax.</span></span>|
|<span data-ttu-id="7c02c-168">unitCost</span><span class="sxs-lookup"><span data-stu-id="7c02c-168">unitCost</span></span>            |<span data-ttu-id="7c02c-169">decimal</span><span class="sxs-lookup"><span data-stu-id="7c02c-169">decimal</span></span> |<span data-ttu-id="7c02c-170">Gibt die Kosten pro Einheit des Elements an.</span><span class="sxs-lookup"><span data-stu-id="7c02c-170">Specifies the cost per unit of the item.</span></span>             |
|<span data-ttu-id="7c02c-171">taxGroupId</span><span class="sxs-lookup"><span data-stu-id="7c02c-171">taxGroupId</span></span>          |<span data-ttu-id="7c02c-172">GUID</span><span class="sxs-lookup"><span data-stu-id="7c02c-172">GUID</span></span>    |<span data-ttu-id="7c02c-173">Gibt die ID der Steuergruppe für das Element an.</span><span class="sxs-lookup"><span data-stu-id="7c02c-173">Specifies the ID of the Tax Group for the item.</span></span>      |
|<span data-ttu-id="7c02c-174">taxGroupCode</span><span class="sxs-lookup"><span data-stu-id="7c02c-174">taxGroupCode</span></span>        |<span data-ttu-id="7c02c-175">numerischen</span><span class="sxs-lookup"><span data-stu-id="7c02c-175">numeric</span></span> |<span data-ttu-id="7c02c-176">Eine Steuergruppe stellt eine Gruppe von Inventar Elementen oder Ressourcen dar, die identischen Steuerbedingungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7c02c-176">A Tax Group represents a group of inventory items or resources that are subject to identical tax terms.</span></span>|
|<span data-ttu-id="7c02c-177">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7c02c-177">lastModifiedDateTime</span></span>|<span data-ttu-id="7c02c-178">DateTime</span><span class="sxs-lookup"><span data-stu-id="7c02c-178">datetime</span></span>|<span data-ttu-id="7c02c-179">Die letzte DateTime, die das Element geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="7c02c-179">The last datetime the item was modified.</span></span> <span data-ttu-id="7c02c-180">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7c02c-180">Read-Only.</span></span>  |  


## <a name="relationships"></a><span data-ttu-id="7c02c-181">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="7c02c-181">Relationships</span></span>
<span data-ttu-id="7c02c-182">In der Tabelle "Steuergruppe" muss eine Steuergruppe (taxGroupCode) vorhanden sein.</span><span class="sxs-lookup"><span data-stu-id="7c02c-182">A Tax Group(taxGroupCode) must exist in the Tax Group table.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7c02c-183">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7c02c-183">JSON representation</span></span>

<span data-ttu-id="7c02c-184">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7c02c-184">Here is a JSON representation of the resource.</span></span>


```json
{
      "id": "GUID",
      "number": "string",
      "displayName": "string",
      "type": "string",
      "blocked": "boolean",
      "baseUnitOfMeasureId": "GUID",
      "baseUnitOfMeasure": "NAV.UnitOfMeasure",
      "gtin": "numeric",
      "itemCategoryId": "GUID",
      "inventory": "decimal",
      "unitPrice": "decimal",
      "priceIncludesTax": "boolean",
      "unitCost": "decimal",
      "taxGroupId": "GUID",
      "taxGroupCode": "string",
      "lastModifiedDateTime": "datetime"
}

```


