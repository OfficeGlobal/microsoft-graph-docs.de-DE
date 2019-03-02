---
title: Ressourcentyp "vendors"
description: Ein Vendor-Objekt in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 1cec20dee4a124bb704d60ceb8229ea820aa55b0
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365661"
---
# <a name="vendors-resource-type"></a><span data-ttu-id="2ce42-103">Ressourcentyp "vendors"</span><span class="sxs-lookup"><span data-stu-id="2ce42-103">vendors resource type</span></span>
<span data-ttu-id="2ce42-104">Stellt einen Anbieter in Dynamics 365 Business Central dar.</span><span class="sxs-lookup"><span data-stu-id="2ce42-104">Represents a vendor in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="2ce42-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="2ce42-105">Methods</span></span>

| <span data-ttu-id="2ce42-106">Methode</span><span class="sxs-lookup"><span data-stu-id="2ce42-106">Method</span></span>       | <span data-ttu-id="2ce42-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="2ce42-107">Return Type</span></span>  |<span data-ttu-id="2ce42-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2ce42-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2ce42-109">Kreditoren abrufen</span><span class="sxs-lookup"><span data-stu-id="2ce42-109">Get vendors</span></span>](../api/dynamics-vendor-get.md)|<span data-ttu-id="2ce42-110">Anbieter</span><span class="sxs-lookup"><span data-stu-id="2ce42-110">vendors</span></span>|<span data-ttu-id="2ce42-111">Ruft ein Vendor-Objekt ab.</span><span class="sxs-lookup"><span data-stu-id="2ce42-111">Gets a vendor object.</span></span>|
|[<span data-ttu-id="2ce42-112">Post-Kreditoren</span><span class="sxs-lookup"><span data-stu-id="2ce42-112">Post vendors</span></span>](../api/dynamics-create-vendor.md)|<span data-ttu-id="2ce42-113">Anbieter</span><span class="sxs-lookup"><span data-stu-id="2ce42-113">vendors</span></span>|<span data-ttu-id="2ce42-114">Erstellt ein Vendor-Objekt.</span><span class="sxs-lookup"><span data-stu-id="2ce42-114">Creates a vendor object.</span></span>|
|[<span data-ttu-id="2ce42-115">Patch-Anbieter</span><span class="sxs-lookup"><span data-stu-id="2ce42-115">Patch vendors</span></span>](../api/dynamics-vendor-update.md)|<span data-ttu-id="2ce42-116">Anbieter</span><span class="sxs-lookup"><span data-stu-id="2ce42-116">vendors</span></span>|<span data-ttu-id="2ce42-117">Aktualisiert ein Vendor-Objekt.</span><span class="sxs-lookup"><span data-stu-id="2ce42-117">Updates a vendor object.</span></span>|
|[<span data-ttu-id="2ce42-118">Kreditor löschen</span><span class="sxs-lookup"><span data-stu-id="2ce42-118">Delete vendor</span></span>](../api/dynamics-vendor-delete.md)|<span data-ttu-id="2ce42-119">Keine</span><span class="sxs-lookup"><span data-stu-id="2ce42-119">none</span></span>|<span data-ttu-id="2ce42-120">Löscht ein Vendor-Objekt.</span><span class="sxs-lookup"><span data-stu-id="2ce42-120">Deletes a vendor object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2ce42-121">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2ce42-121">Properties</span></span>
| <span data-ttu-id="2ce42-122">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2ce42-122">Property</span></span>     | <span data-ttu-id="2ce42-123">Typ</span><span class="sxs-lookup"><span data-stu-id="2ce42-123">Type</span></span>   |<span data-ttu-id="2ce42-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2ce42-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2ce42-125">id</span><span class="sxs-lookup"><span data-stu-id="2ce42-125">id</span></span>|<span data-ttu-id="2ce42-126">GUID</span><span class="sxs-lookup"><span data-stu-id="2ce42-126">GUID</span></span>|<span data-ttu-id="2ce42-127">Die eindeutige ID des Kreditors.</span><span class="sxs-lookup"><span data-stu-id="2ce42-127">The unique ID of the vendor.</span></span> <span data-ttu-id="2ce42-128">Nicht bearbeitbar.</span><span class="sxs-lookup"><span data-stu-id="2ce42-128">Non-editable.</span></span>|
|<span data-ttu-id="2ce42-129">number</span><span class="sxs-lookup"><span data-stu-id="2ce42-129">number</span></span>|<span data-ttu-id="2ce42-130">string</span><span class="sxs-lookup"><span data-stu-id="2ce42-130">string</span></span>|<span data-ttu-id="2ce42-131">Die Kreditornummer.</span><span class="sxs-lookup"><span data-stu-id="2ce42-131">The vendor number.</span></span>|
|<span data-ttu-id="2ce42-132">displayName</span><span class="sxs-lookup"><span data-stu-id="2ce42-132">displayName</span></span>|<span data-ttu-id="2ce42-133">string</span><span class="sxs-lookup"><span data-stu-id="2ce42-133">string</span></span>|<span data-ttu-id="2ce42-134">Der Anzeigename des Anbieters.</span><span class="sxs-lookup"><span data-stu-id="2ce42-134">The vendor's display name.</span></span>|
|<span data-ttu-id="2ce42-135">address</span><span class="sxs-lookup"><span data-stu-id="2ce42-135">address</span></span>|[<span data-ttu-id="2ce42-136">Navigations. PostalAddress</span><span class="sxs-lookup"><span data-stu-id="2ce42-136">NAV.PostalAddress</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="2ce42-137">Die Adresse des Kreditors.</span><span class="sxs-lookup"><span data-stu-id="2ce42-137">The vendor's address.</span></span>|
|<span data-ttu-id="2ce42-138">PhoneNumber</span><span class="sxs-lookup"><span data-stu-id="2ce42-138">phoneNumber</span></span>|<span data-ttu-id="2ce42-139">string</span><span class="sxs-lookup"><span data-stu-id="2ce42-139">string</span></span>|<span data-ttu-id="2ce42-140">Die Telefonnummer des Kreditors.</span><span class="sxs-lookup"><span data-stu-id="2ce42-140">The vendor's telephone number.</span></span>|
|<span data-ttu-id="2ce42-141">email</span><span class="sxs-lookup"><span data-stu-id="2ce42-141">email</span></span>|<span data-ttu-id="2ce42-142">string</span><span class="sxs-lookup"><span data-stu-id="2ce42-142">string</span></span>|<span data-ttu-id="2ce42-143">Die e-Mail-Adresse des Anbieters.</span><span class="sxs-lookup"><span data-stu-id="2ce42-143">The vendor's email address.</span></span>|
|<span data-ttu-id="2ce42-144">Website</span><span class="sxs-lookup"><span data-stu-id="2ce42-144">website</span></span>|<span data-ttu-id="2ce42-145">string</span><span class="sxs-lookup"><span data-stu-id="2ce42-145">string</span></span>|<span data-ttu-id="2ce42-146">Die Websiteadresse des Anbieters.</span><span class="sxs-lookup"><span data-stu-id="2ce42-146">The vendor's website address.</span></span>|
|<span data-ttu-id="2ce42-147">taxRegistrationNumber</span><span class="sxs-lookup"><span data-stu-id="2ce42-147">taxRegistrationNumber</span></span>|<span data-ttu-id="2ce42-148">string</span><span class="sxs-lookup"><span data-stu-id="2ce42-148">string</span></span>|<span data-ttu-id="2ce42-149">Die Steuernummer des Kreditors.</span><span class="sxs-lookup"><span data-stu-id="2ce42-149">The vendor's tax registration number.</span></span>|
|<span data-ttu-id="2ce42-150">currencyId</span><span class="sxs-lookup"><span data-stu-id="2ce42-150">currencyId</span></span>|<span data-ttu-id="2ce42-151">GUID</span><span class="sxs-lookup"><span data-stu-id="2ce42-151">GUID</span></span>|<span data-ttu-id="2ce42-152">Die Standard-Währungscode-ID für den Kreditor.</span><span class="sxs-lookup"><span data-stu-id="2ce42-152">The default currency code ID for the vendor.</span></span>|
|<span data-ttu-id="2ce42-153">currencyCode</span><span class="sxs-lookup"><span data-stu-id="2ce42-153">currencyCode</span></span>|<span data-ttu-id="2ce42-154">string</span><span class="sxs-lookup"><span data-stu-id="2ce42-154">string</span></span>|<span data-ttu-id="2ce42-155">Der Standardwährungscode für den Kreditor.</span><span class="sxs-lookup"><span data-stu-id="2ce42-155">The default currency code for the vendor.</span></span>|
|<span data-ttu-id="2ce42-156">irs1099Code</span><span class="sxs-lookup"><span data-stu-id="2ce42-156">irs1099Code</span></span>|<span data-ttu-id="2ce42-157">string</span><span class="sxs-lookup"><span data-stu-id="2ce42-157">string</span></span>|<span data-ttu-id="2ce42-158">Gibt einen 1099-Code für den Kreditor an.</span><span class="sxs-lookup"><span data-stu-id="2ce42-158">Specifies a 1099 code for the vendor.</span></span> <span data-ttu-id="2ce42-159">Nur uns.</span><span class="sxs-lookup"><span data-stu-id="2ce42-159">US only.</span></span>|
|<span data-ttu-id="2ce42-160">paymentTermsId</span><span class="sxs-lookup"><span data-stu-id="2ce42-160">paymentTermsId</span></span>|<span data-ttu-id="2ce42-161">GUID</span><span class="sxs-lookup"><span data-stu-id="2ce42-161">GUID</span></span>|<span data-ttu-id="2ce42-162">Die Standard-Zahlungs Bedingungs-ID für den Kreditor.</span><span class="sxs-lookup"><span data-stu-id="2ce42-162">The default payment terms ID for the vendor.</span></span>|
|<span data-ttu-id="2ce42-163">paymentMethodId</span><span class="sxs-lookup"><span data-stu-id="2ce42-163">paymentMethodId</span></span>|<span data-ttu-id="2ce42-164">GUID</span><span class="sxs-lookup"><span data-stu-id="2ce42-164">GUID</span></span>|<span data-ttu-id="2ce42-165">Die Standard-Zahlungsmethoden-ID für den Kreditor.</span><span class="sxs-lookup"><span data-stu-id="2ce42-165">The default payment method ID for the vendor.</span></span>|
|<span data-ttu-id="2ce42-166">taxLiable</span><span class="sxs-lookup"><span data-stu-id="2ce42-166">taxLiable</span></span>|<span data-ttu-id="2ce42-167">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="2ce42-167">boolean</span></span>|<span data-ttu-id="2ce42-168">Gibt an, ob der Verkäufer steuerpflichtig ist.</span><span class="sxs-lookup"><span data-stu-id="2ce42-168">Specifies if the vendor is liable for tax.</span></span>|
|<span data-ttu-id="2ce42-169">gesperrt</span><span class="sxs-lookup"><span data-stu-id="2ce42-169">blocked</span></span>|<span data-ttu-id="2ce42-170">string</span><span class="sxs-lookup"><span data-stu-id="2ce42-170">string</span></span>|<span data-ttu-id="2ce42-171">Gibt an, welche Transaktionen mit dem Kreditor, der nicht gebucht werden kann.</span><span class="sxs-lookup"><span data-stu-id="2ce42-171">Specifies which transactions with the vendor that cannot be posted.</span></span> <span data-ttu-id="2ce42-172">Akzeptierte Werte sind leer, Zahlung oder alle</span><span class="sxs-lookup"><span data-stu-id="2ce42-172">Accepted values are blank, Payment or All</span></span>|
|<span data-ttu-id="2ce42-173">Ausgleich</span><span class="sxs-lookup"><span data-stu-id="2ce42-173">balance</span></span>|<span data-ttu-id="2ce42-174">decimal</span><span class="sxs-lookup"><span data-stu-id="2ce42-174">decimal</span></span>|<span data-ttu-id="2ce42-175">Der Saldo des Kreditors.</span><span class="sxs-lookup"><span data-stu-id="2ce42-175">The vendor's balance.</span></span> <span data-ttu-id="2ce42-176">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2ce42-176">Read-Only.</span></span>|
|<span data-ttu-id="2ce42-177">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2ce42-177">lastModifiedDateTime</span></span>|<span data-ttu-id="2ce42-178">DateTime</span><span class="sxs-lookup"><span data-stu-id="2ce42-178">datetime</span></span>|<span data-ttu-id="2ce42-179">Die letzte DateTime, die der Kreditor geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="2ce42-179">The last datetime the vendor was modified.</span></span> <span data-ttu-id="2ce42-180">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2ce42-180">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="2ce42-181">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="2ce42-181">Relationships</span></span>
<span data-ttu-id="2ce42-182">Keine</span><span class="sxs-lookup"><span data-stu-id="2ce42-182">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2ce42-183">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2ce42-183">JSON representation</span></span>

<span data-ttu-id="2ce42-184">Es folgt eine JSON-Darstellung des Anbieters.</span><span class="sxs-lookup"><span data-stu-id="2ce42-184">Here is a JSON representation of the vendor.</span></span>

```json
{
  "id": "GUID",
  "number": "string",
  "displayName": "string",
  "address": "NAV.PostalAddress",
  "phoneNumber": "string",
  "email": "string",
  "website": "string",
  "taxRegistrationNumber": "string",
  "currencyId": "GUID",
  "currencyCode": "string",
  "irs1099Code": "string",
  "paymentTermsId": "GUID",
  "paymentMethodId": "GUID",
  "taxLiable": "boolean",
  "blocked": "string",
  "balance": "decimal",
  "lastModifiedDateTime": "datetime"
}

```

