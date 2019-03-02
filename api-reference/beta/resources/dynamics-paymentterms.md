---
title: paymentTerms-Ressourcentyp
description: Ein Zahlungsbedingungen-Objekt in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 4ed1f3791474cf6e29038e75fcd3625e4da300a0
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365640"
---
# <a name="paymentterms-resource-type"></a><span data-ttu-id="dd761-103">paymentTerms-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="dd761-103">paymentTerms resource type</span></span>
<span data-ttu-id="dd761-104">Stellt eine Zahlungsbedingung in Dynamics 365 Business Central dar.</span><span class="sxs-lookup"><span data-stu-id="dd761-104">Represents a payment term in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="dd761-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="dd761-105">Methods</span></span>

| <span data-ttu-id="dd761-106">Methode</span><span class="sxs-lookup"><span data-stu-id="dd761-106">Method</span></span>                                                      | <span data-ttu-id="dd761-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="dd761-107">Return Type</span></span>|<span data-ttu-id="dd761-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dd761-108">Description</span></span>            |
|:------------------------------------------------------------|:-----------|:----------------------|
|[<span data-ttu-id="dd761-109">PaymentTerms abrufen</span><span class="sxs-lookup"><span data-stu-id="dd761-109">Get paymentTerms</span></span>](../api/dynamics-paymentterms-get.md)      |<span data-ttu-id="dd761-110">paymentTerms</span><span class="sxs-lookup"><span data-stu-id="dd761-110">paymentTerms</span></span>|<span data-ttu-id="dd761-111">Rufen Sie ein Zahlungsbedingungen-Objekt ab.</span><span class="sxs-lookup"><span data-stu-id="dd761-111">Get a payment terms object.</span></span>   |
|[<span data-ttu-id="dd761-112">Post paymentTerms</span><span class="sxs-lookup"><span data-stu-id="dd761-112">Post paymentTerms</span></span>](../api/dynamics-create-paymentterms.md)  |<span data-ttu-id="dd761-113">paymentTerms</span><span class="sxs-lookup"><span data-stu-id="dd761-113">paymentTerms</span></span>|<span data-ttu-id="dd761-114">Erstellen eines Zahlungs Begriffs-Objekts.</span><span class="sxs-lookup"><span data-stu-id="dd761-114">Create a payment terms object.</span></span>|
|[<span data-ttu-id="dd761-115">Patch-paymentTerms</span><span class="sxs-lookup"><span data-stu-id="dd761-115">Patch paymentTerms</span></span>](../api/dynamics-paymentterms-update.md) |<span data-ttu-id="dd761-116">paymentTerms</span><span class="sxs-lookup"><span data-stu-id="dd761-116">paymentTerms</span></span>|<span data-ttu-id="dd761-117">Aktualisieren eines Zahlungs Begriffs-Objekts.</span><span class="sxs-lookup"><span data-stu-id="dd761-117">Update a payment terms object.</span></span>|
|[<span data-ttu-id="dd761-118">PaymentTerms löschen</span><span class="sxs-lookup"><span data-stu-id="dd761-118">Delete paymentTerms</span></span>](../api/dynamics-paymentterms-delete.md)|<span data-ttu-id="dd761-119">Keine</span><span class="sxs-lookup"><span data-stu-id="dd761-119">none</span></span>        |<span data-ttu-id="dd761-120">Löschen eines Zahlungs Begriffs-Objekts.</span><span class="sxs-lookup"><span data-stu-id="dd761-120">Delete a payment terms object.</span></span>|

## <a name="properties"></a><span data-ttu-id="dd761-121">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="dd761-121">Properties</span></span>
| <span data-ttu-id="dd761-122">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="dd761-122">Property</span></span>                     | <span data-ttu-id="dd761-123">Typ</span><span class="sxs-lookup"><span data-stu-id="dd761-123">Type</span></span>     |<span data-ttu-id="dd761-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dd761-124">Description</span></span>                                                |
|:-----------------------------|:-------|:----------------------------------------------------------|
|<span data-ttu-id="dd761-125">id</span><span class="sxs-lookup"><span data-stu-id="dd761-125">id</span></span>                            |<span data-ttu-id="dd761-126">GUID</span><span class="sxs-lookup"><span data-stu-id="dd761-126">GUID</span></span>    |<span data-ttu-id="dd761-127">Die eindeutige ID des paymentTerms.</span><span class="sxs-lookup"><span data-stu-id="dd761-127">The unique ID of the paymentTerms.</span></span> <span data-ttu-id="dd761-128">Nicht bearbeitbar.</span><span class="sxs-lookup"><span data-stu-id="dd761-128">Non-editable.</span></span>           |
|<span data-ttu-id="dd761-129">code</span><span class="sxs-lookup"><span data-stu-id="dd761-129">code</span></span>                          |<span data-ttu-id="dd761-130">string</span><span class="sxs-lookup"><span data-stu-id="dd761-130">string</span></span>  |<span data-ttu-id="dd761-131">Gibt den Zahlungs Begriffs Code an.</span><span class="sxs-lookup"><span data-stu-id="dd761-131">Specifies the payment term code.</span></span>                           |
|<span data-ttu-id="dd761-132">displayName</span><span class="sxs-lookup"><span data-stu-id="dd761-132">displayName</span></span>                   |<span data-ttu-id="dd761-133">string</span><span class="sxs-lookup"><span data-stu-id="dd761-133">string</span></span>  |<span data-ttu-id="dd761-134">Gibt den Anzeigenamen für den Zahlungs Ausdruck an.</span><span class="sxs-lookup"><span data-stu-id="dd761-134">Specifies the payment term display name.</span></span>                   |
|<span data-ttu-id="dd761-135">dueDateCalculation</span><span class="sxs-lookup"><span data-stu-id="dd761-135">dueDateCalculation</span></span>            |<span data-ttu-id="dd761-136">string</span><span class="sxs-lookup"><span data-stu-id="dd761-136">string</span></span>  |<span data-ttu-id="dd761-137">Gibt die Formel an, die verwendet wird, um das Datum zu berechnen, an dem eine Zahlung getätigt werden muss.</span><span class="sxs-lookup"><span data-stu-id="dd761-137">Specifies the formula that is used to calculate the date that a payment must be made.</span></span>|
|<span data-ttu-id="dd761-138">discountDateCalculation</span><span class="sxs-lookup"><span data-stu-id="dd761-138">discountDateCalculation</span></span>       |<span data-ttu-id="dd761-139">string</span><span class="sxs-lookup"><span data-stu-id="dd761-139">string</span></span>  |<span data-ttu-id="dd761-140">Gibt die Formel an, die verwendet wird, um das Datum zu berechnen, an dem eine Zahlung getätigt werden muss, um einen Rabatt zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="dd761-140">Specifies the formula that is used to calculate the date that a payment must be made in order to obtain a discount.</span></span>|
|<span data-ttu-id="dd761-141">discountPercent</span><span class="sxs-lookup"><span data-stu-id="dd761-141">discountPercent</span></span>               |<span data-ttu-id="dd761-142">decimal</span><span class="sxs-lookup"><span data-stu-id="dd761-142">decimal</span></span> |<span data-ttu-id="dd761-143">Gibt den Rabattprozentsatz an, der für die vorzeitige Zahlung eines Rechnungsbetrags angewendet wird.</span><span class="sxs-lookup"><span data-stu-id="dd761-143">Specifies the discount percentage that is applied for early payment of an invoice amount.</span></span>|
|<span data-ttu-id="dd761-144">calculateDiscountOnCreditMemos</span><span class="sxs-lookup"><span data-stu-id="dd761-144">calculateDiscountOnCreditMemos</span></span>|<span data-ttu-id="dd761-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="dd761-145">boolean</span></span> |<span data-ttu-id="dd761-146">Gibt an, ob der Rabatt auf Gutschriften angewendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="dd761-146">Specifies if the discount should be applied to credit memos.</span></span> <span data-ttu-id="dd761-147">**True** gibt an, dass ein Rabatt gewährt wird, **false** gibt an, dass kein Preisnachlass gewährt wird.</span><span class="sxs-lookup"><span data-stu-id="dd761-147">**True** indicates a discount will be given, **false** indicates a discount will not be given.</span></span>|
|<span data-ttu-id="dd761-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dd761-148">lastModifiedDateTime</span></span>          |<span data-ttu-id="dd761-149">DateTime</span><span class="sxs-lookup"><span data-stu-id="dd761-149">datetime</span></span>|<span data-ttu-id="dd761-150">Die letzte DateTime, die der paymentTerms geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="dd761-150">The last datetime the paymentTerms was modified.</span></span> <span data-ttu-id="dd761-151">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="dd761-151">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="dd761-152">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="dd761-152">Relationships</span></span>
<span data-ttu-id="dd761-153">Keine</span><span class="sxs-lookup"><span data-stu-id="dd761-153">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dd761-154">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="dd761-154">JSON representation</span></span>

<span data-ttu-id="dd761-155">Es folgt eine JSON-Darstellung des paymentTerms.</span><span class="sxs-lookup"><span data-stu-id="dd761-155">Here is a JSON representation of the paymentTerms.</span></span>


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "dueDateCalculation": "string",
  "discountDateCalculation": "string",
  "discountPercent": "decimal",
  "calculateDiscountOnCreditMemos": "boolean",
  "lastModifiedDateTime": "datetime"
}

```
