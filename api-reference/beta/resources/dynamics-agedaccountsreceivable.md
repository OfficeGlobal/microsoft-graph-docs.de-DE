---
title: agedAccountsReceivable-Ressourcentyp
description: Ein gealterte Forderungen Objekt in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: ce5d010c08f956468398082821040e30b4ef2ace
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365577"
---
# <a name="agedaccountsreceivable-resource-type"></a><span data-ttu-id="b48b4-103">agedAccountsReceivable-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b48b4-103">agedAccountsReceivable resource type</span></span>
<span data-ttu-id="b48b4-104">Stellt ein agedAccountsReceivable-Objekt in Dynamics 365 Business Central dar, das die Alterung eines Kundenkontos anzeigt.</span><span class="sxs-lookup"><span data-stu-id="b48b4-104">Represents an agedAccountsReceivable object in Dynamics 365 Business Central, which is showing the aging of a customer account.</span></span>

## <a name="methods"></a><span data-ttu-id="b48b4-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="b48b4-105">Methods</span></span>

| <span data-ttu-id="b48b4-106">Methode</span><span class="sxs-lookup"><span data-stu-id="b48b4-106">Method</span></span>         | <span data-ttu-id="b48b4-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="b48b4-107">Return Type</span></span>  |<span data-ttu-id="b48b4-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b48b4-108">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="b48b4-109">AgedAccountsReceivable abrufen</span><span class="sxs-lookup"><span data-stu-id="b48b4-109">Get agedAccountsReceivable</span></span>](../api/dynamics-agedaccountsreceivable-get.md)|<span data-ttu-id="b48b4-110">agedAccountsReceivable</span><span class="sxs-lookup"><span data-stu-id="b48b4-110">agedAccountsReceivable</span></span>|<span data-ttu-id="b48b4-111">AgedAccountsReceivable-Objekt abrufen</span><span class="sxs-lookup"><span data-stu-id="b48b4-111">Get agedAccountsReceivable object</span></span>|

## <a name="properties"></a><span data-ttu-id="b48b4-112">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b48b4-112">Properties</span></span>
| <span data-ttu-id="b48b4-113">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b48b4-113">Property</span></span>       | <span data-ttu-id="b48b4-114">Typ</span><span class="sxs-lookup"><span data-stu-id="b48b4-114">Type</span></span>    |<span data-ttu-id="b48b4-115">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b48b4-115">Description</span></span>                                  |
|:---------------|:--------|:--------------------------------------------|
|<span data-ttu-id="b48b4-116">customerId</span><span class="sxs-lookup"><span data-stu-id="b48b4-116">customerId</span></span>      |<span data-ttu-id="b48b4-117">GUID</span><span class="sxs-lookup"><span data-stu-id="b48b4-117">GUID</span></span>     |<span data-ttu-id="b48b4-118">Die eindeutige ID des Kunden.</span><span class="sxs-lookup"><span data-stu-id="b48b4-118">The unique ID of customer.</span></span>                   |
|<span data-ttu-id="b48b4-119">customerNumber</span><span class="sxs-lookup"><span data-stu-id="b48b4-119">customerNumber</span></span>  |<span data-ttu-id="b48b4-120">string</span><span class="sxs-lookup"><span data-stu-id="b48b4-120">string</span></span>   |<span data-ttu-id="b48b4-121">Gibt die Nummer des Kunden an.</span><span class="sxs-lookup"><span data-stu-id="b48b4-121">Specifies customer's number.</span></span>                 |
|<span data-ttu-id="b48b4-122">name</span><span class="sxs-lookup"><span data-stu-id="b48b4-122">name</span></span>            |<span data-ttu-id="b48b4-123">string</span><span class="sxs-lookup"><span data-stu-id="b48b4-123">string</span></span>   |<span data-ttu-id="b48b4-124">Gibt den Namen des Kunden an.</span><span class="sxs-lookup"><span data-stu-id="b48b4-124">Specifies customer's name.</span></span>                   |
|<span data-ttu-id="b48b4-125">currencyCode</span><span class="sxs-lookup"><span data-stu-id="b48b4-125">currencyCode</span></span>    |<span data-ttu-id="b48b4-126">string</span><span class="sxs-lookup"><span data-stu-id="b48b4-126">string</span></span>   |<span data-ttu-id="b48b4-127">Gibt die Währung an.</span><span class="sxs-lookup"><span data-stu-id="b48b4-127">Specifies the currency.</span></span>                      |
|<span data-ttu-id="b48b4-128">balanceDue</span><span class="sxs-lookup"><span data-stu-id="b48b4-128">balanceDue</span></span>      |<span data-ttu-id="b48b4-129">numerischen</span><span class="sxs-lookup"><span data-stu-id="b48b4-129">numeric</span></span>  |<span data-ttu-id="b48b4-130">Gibt den Gesamtsaldo des Kunden an.</span><span class="sxs-lookup"><span data-stu-id="b48b4-130">Specifies the customer's total balance.</span></span>      |
|<span data-ttu-id="b48b4-131">currentAmount</span><span class="sxs-lookup"><span data-stu-id="b48b4-131">currentAmount</span></span>   |<span data-ttu-id="b48b4-132">numerischen</span><span class="sxs-lookup"><span data-stu-id="b48b4-132">numeric</span></span>  |<span data-ttu-id="b48b4-133">Gibt den Saldo für die aktuelle Alterungsperiode an.</span><span class="sxs-lookup"><span data-stu-id="b48b4-133">Specifies balance for the current aging period.</span></span>|
|<span data-ttu-id="b48b4-134">period1Amount</span><span class="sxs-lookup"><span data-stu-id="b48b4-134">period1Amount</span></span>   |<span data-ttu-id="b48b4-135">numerischen</span><span class="sxs-lookup"><span data-stu-id="b48b4-135">numeric</span></span>  |<span data-ttu-id="b48b4-136">Gibt den Saldo im ersten Alterungszeitraum an.</span><span class="sxs-lookup"><span data-stu-id="b48b4-136">Specifies balance in the first aging period.</span></span> |
|<span data-ttu-id="b48b4-137">period2Amount</span><span class="sxs-lookup"><span data-stu-id="b48b4-137">period2Amount</span></span>   |<span data-ttu-id="b48b4-138">numerischen</span><span class="sxs-lookup"><span data-stu-id="b48b4-138">numeric</span></span>  |<span data-ttu-id="b48b4-139">Gibt den Saldo im zweiten Alterungszeitraum an.</span><span class="sxs-lookup"><span data-stu-id="b48b4-139">Specifies balance in the second aging period.</span></span>|
|<span data-ttu-id="b48b4-140">period3Amount</span><span class="sxs-lookup"><span data-stu-id="b48b4-140">period3Amount</span></span>   |<span data-ttu-id="b48b4-141">numerischen</span><span class="sxs-lookup"><span data-stu-id="b48b4-141">numeric</span></span>  |<span data-ttu-id="b48b4-142">Gibt den Saldo im dritten Alterungszeitraum an.</span><span class="sxs-lookup"><span data-stu-id="b48b4-142">Specifies balance in the third aging period.</span></span> |
|<span data-ttu-id="b48b4-143">agedAsOfDate</span><span class="sxs-lookup"><span data-stu-id="b48b4-143">agedAsOfDate</span></span>    |<span data-ttu-id="b48b4-144">date</span><span class="sxs-lookup"><span data-stu-id="b48b4-144">date</span></span>     |<span data-ttu-id="b48b4-145">Gibt den Zeitraum an, der zum Berechnen von Alterungs Perioden verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="b48b4-145">Specifies period start date used to calculate aging periods.</span></span>|
|<span data-ttu-id="b48b4-146">periodLengthFilter</span><span class="sxs-lookup"><span data-stu-id="b48b4-146">periodLengthFilter</span></span>|<span data-ttu-id="b48b4-147">string</span><span class="sxs-lookup"><span data-stu-id="b48b4-147">string</span></span> |<span data-ttu-id="b48b4-148">Gibt die Länge der Punkte an.</span><span class="sxs-lookup"><span data-stu-id="b48b4-148">Specifies the length of the periods.</span></span> <span data-ttu-id="b48b4-149">Zulässige Zeiteinheiten sind: D, WD, W, M, Q und Y. C, was bedeutet, dass die aktuelle Zeiteinheit auf dem Datum basiert, als Präfix für die Zeiteinheit angegeben werden kann.</span><span class="sxs-lookup"><span data-stu-id="b48b4-149">Acceptable time units include: D, WD, W, M, Q, and Y. C, meaning current time unit based on date, can be specified as a prefix to the time unit.</span></span>|


## <a name="relationships"></a><span data-ttu-id="b48b4-150">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b48b4-150">Relationships</span></span>
<span data-ttu-id="b48b4-151">Keine</span><span class="sxs-lookup"><span data-stu-id="b48b4-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b48b4-152">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b48b4-152">JSON representation</span></span>

<span data-ttu-id="b48b4-153">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b48b4-153">Here is a JSON representation of the resource.</span></span>


```json
{
    "customerId": "GUID",
    "customerNumber": "string",
    "name": "string",
    "currencyCode": "string",
    "balanceDue": "decimal",
    "currentAmount": "decimal",
    "period1Amount": "decimal",
    "period2Amount": "decimal",
    "period3Amount": "decimal",
    "agedAsOfDate": "date",
    "periodLengthFilter": "string"
}

```


