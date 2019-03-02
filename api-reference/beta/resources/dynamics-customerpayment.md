---
title: customerPayments-Ressourcentyp
description: Ein Kunden Zahlungs Objekt in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 9063a9066c51956596e4f0aa918a2e7a53bf2ab9
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365612"
---
# <a name="customerpayments-resource-type"></a><span data-ttu-id="d4ce8-103">customerPayments-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d4ce8-103">customerPayments resource type</span></span>
<span data-ttu-id="d4ce8-104">Stellt eine Kundenzahlung in Dynamics 365 Business Central dar.</span><span class="sxs-lookup"><span data-stu-id="d4ce8-104">Represents a customer payment in Dynamics 365 Business Central.</span></span> <span data-ttu-id="d4ce8-105">Eine Debitorenzahlung wird als Zeile in einer Debitoren Zahlungserfassung eingegeben.</span><span class="sxs-lookup"><span data-stu-id="d4ce8-105">A customer payment is entered as a line in a customer payment journal.</span></span>

## <a name="methods"></a><span data-ttu-id="d4ce8-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="d4ce8-106">Methods</span></span>

| <span data-ttu-id="d4ce8-107">Methode</span><span class="sxs-lookup"><span data-stu-id="d4ce8-107">Method</span></span>         | <span data-ttu-id="d4ce8-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="d4ce8-108">Return Type</span></span>  |<span data-ttu-id="d4ce8-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d4ce8-109">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="d4ce8-110">CustomerPayments abrufen</span><span class="sxs-lookup"><span data-stu-id="d4ce8-110">Get customerPayments</span></span>](../api/dynamics-customerpayment-get.md)|<span data-ttu-id="d4ce8-111">customerPayments</span><span class="sxs-lookup"><span data-stu-id="d4ce8-111">customerPayments</span></span>|<span data-ttu-id="d4ce8-112">Ruft eine Kundenzahlung ab.</span><span class="sxs-lookup"><span data-stu-id="d4ce8-112">Gets a customer payment.</span></span>|
|[<span data-ttu-id="d4ce8-113">Post customerPayments</span><span class="sxs-lookup"><span data-stu-id="d4ce8-113">Post customerPayments</span></span>](../api/dynamics-create-customerpayment.md)|<span data-ttu-id="d4ce8-114">customerPayments</span><span class="sxs-lookup"><span data-stu-id="d4ce8-114">customerPayments</span></span>|<span data-ttu-id="d4ce8-115">Erstellt eine Debitorenzahlung.</span><span class="sxs-lookup"><span data-stu-id="d4ce8-115">Creates a customer payment.</span></span>|
|[<span data-ttu-id="d4ce8-116">Patch-customerPayments</span><span class="sxs-lookup"><span data-stu-id="d4ce8-116">Patch customerPayments</span></span>](../api/dynamics-customerpayment-update.md)|<span data-ttu-id="d4ce8-117">customerPayments</span><span class="sxs-lookup"><span data-stu-id="d4ce8-117">customerPayments</span></span>|<span data-ttu-id="d4ce8-118">Aktualisiert eine Kundenzahlung.</span><span class="sxs-lookup"><span data-stu-id="d4ce8-118">Updates a customer payment.</span></span>|
|[<span data-ttu-id="d4ce8-119">CustomerPayments löschen</span><span class="sxs-lookup"><span data-stu-id="d4ce8-119">Delete customerPayments</span></span>](../api/dynamics-customerpayment-delete.md)|<span data-ttu-id="d4ce8-120">Keine</span><span class="sxs-lookup"><span data-stu-id="d4ce8-120">none</span></span>|<span data-ttu-id="d4ce8-121">Löscht eine Debitorenzahlung.</span><span class="sxs-lookup"><span data-stu-id="d4ce8-121">Deletes a customer payment.</span></span>|

## <a name="properties"></a><span data-ttu-id="d4ce8-122">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d4ce8-122">Properties</span></span>
| <span data-ttu-id="d4ce8-123">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d4ce8-123">Property</span></span>     | <span data-ttu-id="d4ce8-124">Typ</span><span class="sxs-lookup"><span data-stu-id="d4ce8-124">Type</span></span>    |<span data-ttu-id="d4ce8-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d4ce8-125">Description</span></span>|
|:-------------|:--------|:----------|
|<span data-ttu-id="d4ce8-126">id</span><span class="sxs-lookup"><span data-stu-id="d4ce8-126">id</span></span>|<span data-ttu-id="d4ce8-127">GUID</span><span class="sxs-lookup"><span data-stu-id="d4ce8-127">GUID</span></span>|<span data-ttu-id="d4ce8-128">Die eindeutige ID der Debitorenzahlung.</span><span class="sxs-lookup"><span data-stu-id="d4ce8-128">The unique ID of the customer payment.</span></span> <span data-ttu-id="d4ce8-129">Nicht bearbeitbar.</span><span class="sxs-lookup"><span data-stu-id="d4ce8-129">Non-editable.</span></span>|
|<span data-ttu-id="d4ce8-130">journalDisplayName</span><span class="sxs-lookup"><span data-stu-id="d4ce8-130">journalDisplayName</span></span>|<span data-ttu-id="d4ce8-131">string</span><span class="sxs-lookup"><span data-stu-id="d4ce8-131">string</span></span>|<span data-ttu-id="d4ce8-132">Das Debitoren-Zahlungs Blatt, in dem der Zahlungsdatensatz eine Zeile ist.</span><span class="sxs-lookup"><span data-stu-id="d4ce8-132">The customer payment journal in which the payment record is a line.</span></span>|
|<span data-ttu-id="d4ce8-133">lineNumber</span><span class="sxs-lookup"><span data-stu-id="d4ce8-133">lineNumber</span></span>|<span data-ttu-id="d4ce8-134">integer</span><span class="sxs-lookup"><span data-stu-id="d4ce8-134">integer</span></span>|<span data-ttu-id="d4ce8-135">Die Anzahl der Debitorenzahlung.</span><span class="sxs-lookup"><span data-stu-id="d4ce8-135">The number of the customer payment.</span></span>|
|<span data-ttu-id="d4ce8-136">customerId</span><span class="sxs-lookup"><span data-stu-id="d4ce8-136">customerId</span></span>|<span data-ttu-id="d4ce8-137">GUID</span><span class="sxs-lookup"><span data-stu-id="d4ce8-137">GUID</span></span>|<span data-ttu-id="d4ce8-138">Die eindeutige ID des Debitors, mit dem die Zahlung verbunden ist.</span><span class="sxs-lookup"><span data-stu-id="d4ce8-138">The unique ID of the customer that the payment is related to.</span></span>|
|<span data-ttu-id="d4ce8-139">customerNumber</span><span class="sxs-lookup"><span data-stu-id="d4ce8-139">customerNumber</span></span>|<span data-ttu-id="d4ce8-140">Zeichenfolge, maximale Größe 20</span><span class="sxs-lookup"><span data-stu-id="d4ce8-140">string, maximum size 20</span></span>|<span data-ttu-id="d4ce8-141">Die Nummer des Debitors, mit dem die Zahlung verbunden ist.</span><span class="sxs-lookup"><span data-stu-id="d4ce8-141">The number of the customer that the payment is related to.</span></span>|
|<span data-ttu-id="d4ce8-142">contactId</span><span class="sxs-lookup"><span data-stu-id="d4ce8-142">contactId</span></span>|<span data-ttu-id="d4ce8-143">Zeichenfolge, maximale Größe 250</span><span class="sxs-lookup"><span data-stu-id="d4ce8-143">string, maximum size 250</span></span>|<span data-ttu-id="d4ce8-144">Die Exchange-Kontakt-ID für den angegebenen Kunden.</span><span class="sxs-lookup"><span data-stu-id="d4ce8-144">The exchange contact id for the given customer.</span></span> <span data-ttu-id="d4ce8-145">Wenn keine Kunden-ID angegeben wird, verwenden wir die Kontakt-ID, um Sie zu finden.</span><span class="sxs-lookup"><span data-stu-id="d4ce8-145">If a customer id is not specified, we will use the contact id to find it.</span></span>|
|<span data-ttu-id="d4ce8-146">postingDate</span><span class="sxs-lookup"><span data-stu-id="d4ce8-146">postingDate</span></span>|<span data-ttu-id="d4ce8-147">date</span><span class="sxs-lookup"><span data-stu-id="d4ce8-147">date</span></span>|<span data-ttu-id="d4ce8-148">Das Datum, an dem die Debitorenzahlung gebucht wird.</span><span class="sxs-lookup"><span data-stu-id="d4ce8-148">The date that the customer payment is posted.</span></span>|
|<span data-ttu-id="d4ce8-149">documentNumber</span><span class="sxs-lookup"><span data-stu-id="d4ce8-149">documentNumber</span></span>|<span data-ttu-id="d4ce8-150">Zeichenfolge, maximale Größe 20</span><span class="sxs-lookup"><span data-stu-id="d4ce8-150">string, maximum size 20</span></span>|<span data-ttu-id="d4ce8-151">Gibt eine Dokumentnummer für die Debitorenzahlung an.</span><span class="sxs-lookup"><span data-stu-id="d4ce8-151">Specifies a document number for the customer payment.</span></span>|
|<span data-ttu-id="d4ce8-152">externalDocumentNumber</span><span class="sxs-lookup"><span data-stu-id="d4ce8-152">externalDocumentNumber</span></span>|<span data-ttu-id="d4ce8-153">Zeichenfolge, maximale Größe 20</span><span class="sxs-lookup"><span data-stu-id="d4ce8-153">string, maximum size 20</span></span>|<span data-ttu-id="d4ce8-154">Gibt eine externe Belegnummer für die Debitorenzahlung an.</span><span class="sxs-lookup"><span data-stu-id="d4ce8-154">Specifies an external document number for the customer payment.</span></span>|
|<span data-ttu-id="d4ce8-155">Menge</span><span class="sxs-lookup"><span data-stu-id="d4ce8-155">amount</span></span>|<span data-ttu-id="d4ce8-156">decimal</span><span class="sxs-lookup"><span data-stu-id="d4ce8-156">decimal</span></span>|<span data-ttu-id="d4ce8-157">Gibt den Gesamtbetrag (einschließlich Mehrwertsteuer) an, aus dem die Debitorenzahlung besteht.</span><span class="sxs-lookup"><span data-stu-id="d4ce8-157">Specifies the total amount (including VAT) that the customer payment consists of.</span></span>|
|<span data-ttu-id="d4ce8-158">appliesToInvoiceId</span><span class="sxs-lookup"><span data-stu-id="d4ce8-158">appliesToInvoiceId</span></span>|<span data-ttu-id="d4ce8-159">GUID</span><span class="sxs-lookup"><span data-stu-id="d4ce8-159">GUID</span></span>|<span data-ttu-id="d4ce8-160">Die eindeutige ID der Rechnung, mit der die Zahlung verbunden ist.</span><span class="sxs-lookup"><span data-stu-id="d4ce8-160">The unique ID of the invoice that the payment is related to.</span></span>|
|<span data-ttu-id="d4ce8-161">appliesToInvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="d4ce8-161">appliesToInvoiceNumber</span></span>|<span data-ttu-id="d4ce8-162">Zeichenfolge, maximale Größe 20</span><span class="sxs-lookup"><span data-stu-id="d4ce8-162">string, maximum size 20</span></span>|<span data-ttu-id="d4ce8-163">Die Nummer der Rechnung, mit der die Zahlung verbunden ist.</span><span class="sxs-lookup"><span data-stu-id="d4ce8-163">The number of the invoice that the payment is related to.</span></span>|
|<span data-ttu-id="d4ce8-164">description</span><span class="sxs-lookup"><span data-stu-id="d4ce8-164">description</span></span>|<span data-ttu-id="d4ce8-165">Zeichenfolge, maximale Größe 50</span><span class="sxs-lookup"><span data-stu-id="d4ce8-165">string, maximum size 50</span></span>|<span data-ttu-id="d4ce8-166">Die Beschreibung der Debitorenzahlung, die vom Benutzer bereitgestellt oder selbst erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="d4ce8-166">The description of the customer payment, provided by the user or autocreated.</span></span>|
|<span data-ttu-id="d4ce8-167">Kommentar</span><span class="sxs-lookup"><span data-stu-id="d4ce8-167">comment</span></span>|<span data-ttu-id="d4ce8-168">Zeichenfolge, maximale Größe 250</span><span class="sxs-lookup"><span data-stu-id="d4ce8-168">string, maximum size 250</span></span>|<span data-ttu-id="d4ce8-169">Ein benutzerdefinierter Kommentar zur Debitorenzahlung.</span><span class="sxs-lookup"><span data-stu-id="d4ce8-169">A user specified comment on the customer payment.</span></span>|
|<span data-ttu-id="d4ce8-170">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d4ce8-170">lastModifiedDateTime</span></span>|<span data-ttu-id="d4ce8-171">DateTime</span><span class="sxs-lookup"><span data-stu-id="d4ce8-171">datetime</span></span>|<span data-ttu-id="d4ce8-172">Die letzte DateTime, für die die Debitorenzahlung geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="d4ce8-172">The last datetime the customer payment was modified.</span></span> <span data-ttu-id="d4ce8-173">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d4ce8-173">Read-Only.</span></span>|


## <a name="relationships"></a><span data-ttu-id="d4ce8-174">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d4ce8-174">Relationships</span></span>
<span data-ttu-id="d4ce8-175">Bei einer Debitorenzahlung handelt es sich um eine Unterseite einer Debitoren Zahlungserfassung.</span><span class="sxs-lookup"><span data-stu-id="d4ce8-175">A customer payment is a subpage of a customer payment journal.</span></span> <span data-ttu-id="d4ce8-176">Er kann nicht direkt zugegriffen werden.</span><span class="sxs-lookup"><span data-stu-id="d4ce8-176">It cannot be accessed directly.</span></span>

<span data-ttu-id="d4ce8-177">Eine Debitorenzahlung kann eine "übergeordnete Entität" der Dimensionszeilen sein.</span><span class="sxs-lookup"><span data-stu-id="d4ce8-177">A customer payment can be a "Parent Entity" of the dimension lines.</span></span>

<span data-ttu-id="d4ce8-178">Ein Kunde (customerId) muss in der Customers-Tabelle vorhanden sein.</span><span class="sxs-lookup"><span data-stu-id="d4ce8-178">A Customer (customerId) must exist in the Customers table.</span></span>

<span data-ttu-id="d4ce8-179">In der Tabelle "Verkaufsrechnungen" muss eine Rechnung (appliesToInvoiceId) vorhanden sein.</span><span class="sxs-lookup"><span data-stu-id="d4ce8-179">An Invoice (appliesToInvoiceId) must exist in the Sales Invoices Table.</span></span>


## <a name="json-representation"></a><span data-ttu-id="d4ce8-180">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d4ce8-180">JSON representation</span></span>

<span data-ttu-id="d4ce8-181">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d4ce8-181">Here is a JSON representation of the resource.</span></span>

```json
{
    "id": "GUID",
    "journalDisplayName": "string",
    "lineNumber": "integer",
    "customerId": "GUID",
    "customerNumber": "string",
    "contactId": "string",
    "postingDate": "date",
    "documentNumber": "string",
    "externalDocumentNumber": "string",
    "amount": "decimal",
    "appliesToInvoiceId": "GUID",
    "appliesToInvoiceNumber": "string",
    "description": "string",
    "comment": "string",
    "lastModifiedDateTime": "datetime"
}
```

