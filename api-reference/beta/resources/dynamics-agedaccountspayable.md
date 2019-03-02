---
title: agedAccountsPayable-Ressourcentyp
description: Ein gealterte Kreditoren Objekte in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 679c24b7ef32ef59b34a5885ea745d8c244376b2
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365906"
---
# <a name="agedaccountspayable-resource-type"></a><span data-ttu-id="a1b2a-103">agedAccountsPayable-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a1b2a-103">agedAccountsPayable resource type</span></span>
<span data-ttu-id="a1b2a-104">Stellt ein agedAccountsPayable-Objekt in Dynamics 365 Business Central dar, das die Alterung eines Kreditorenkontos anzeigt.</span><span class="sxs-lookup"><span data-stu-id="a1b2a-104">Represents an agedAccountsPayable object in Dynamics 365 Business Central, which is showing the aging of a vendor account.</span></span>

## <a name="methods"></a><span data-ttu-id="a1b2a-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="a1b2a-105">Methods</span></span>

| <span data-ttu-id="a1b2a-106">Methode</span><span class="sxs-lookup"><span data-stu-id="a1b2a-106">Method</span></span>         | <span data-ttu-id="a1b2a-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="a1b2a-107">Return Type</span></span>  |<span data-ttu-id="a1b2a-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a1b2a-108">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="a1b2a-109">AgedAccountsPayable abrufen</span><span class="sxs-lookup"><span data-stu-id="a1b2a-109">Get agedAccountsPayable</span></span>](../api/dynamics-agedaccountspayable-get.md)|<span data-ttu-id="a1b2a-110">agedAccountsPayable</span><span class="sxs-lookup"><span data-stu-id="a1b2a-110">agedAccountsPayable</span></span>|<span data-ttu-id="a1b2a-111">AgedAccountsPayable-Objekt abrufen</span><span class="sxs-lookup"><span data-stu-id="a1b2a-111">Get agedAccountsPayable object</span></span>|

## <a name="properties"></a><span data-ttu-id="a1b2a-112">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a1b2a-112">Properties</span></span>
| <span data-ttu-id="a1b2a-113">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a1b2a-113">Property</span></span>      | <span data-ttu-id="a1b2a-114">Typ</span><span class="sxs-lookup"><span data-stu-id="a1b2a-114">Type</span></span>     |<span data-ttu-id="a1b2a-115">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a1b2a-115">Description</span></span>                                 |
|:--------------|:---------|:-------------------------------------------|
|<span data-ttu-id="a1b2a-116">vendorId</span><span class="sxs-lookup"><span data-stu-id="a1b2a-116">vendorId</span></span>       |<span data-ttu-id="a1b2a-117">GUID</span><span class="sxs-lookup"><span data-stu-id="a1b2a-117">GUID</span></span>      |<span data-ttu-id="a1b2a-118">Die eindeutige ID des Anbieters.</span><span class="sxs-lookup"><span data-stu-id="a1b2a-118">The unique ID of vendor.</span></span>                    |
|<span data-ttu-id="a1b2a-119">vendorNumber</span><span class="sxs-lookup"><span data-stu-id="a1b2a-119">vendorNumber</span></span>   |<span data-ttu-id="a1b2a-120">string</span><span class="sxs-lookup"><span data-stu-id="a1b2a-120">string</span></span>    |<span data-ttu-id="a1b2a-121">Gibt die Nummer des Kreditors an.</span><span class="sxs-lookup"><span data-stu-id="a1b2a-121">Specifies vendor's number.</span></span>                  |
|<span data-ttu-id="a1b2a-122">name</span><span class="sxs-lookup"><span data-stu-id="a1b2a-122">name</span></span>           |<span data-ttu-id="a1b2a-123">string</span><span class="sxs-lookup"><span data-stu-id="a1b2a-123">string</span></span>    |<span data-ttu-id="a1b2a-124">Gibt den Namen des Anbieters an.</span><span class="sxs-lookup"><span data-stu-id="a1b2a-124">Specifies vendor's name.</span></span>                    |
|<span data-ttu-id="a1b2a-125">currencyCode</span><span class="sxs-lookup"><span data-stu-id="a1b2a-125">currencyCode</span></span>   |<span data-ttu-id="a1b2a-126">string</span><span class="sxs-lookup"><span data-stu-id="a1b2a-126">string</span></span>    |<span data-ttu-id="a1b2a-127">Gibt die Währung an.</span><span class="sxs-lookup"><span data-stu-id="a1b2a-127">Specifies the currency.</span></span>                     |
|<span data-ttu-id="a1b2a-128">balanceDue</span><span class="sxs-lookup"><span data-stu-id="a1b2a-128">balanceDue</span></span>     |<span data-ttu-id="a1b2a-129">numerischen</span><span class="sxs-lookup"><span data-stu-id="a1b2a-129">numeric</span></span>   |<span data-ttu-id="a1b2a-130">Gibt den Gesamtsaldo des Kreditors an.</span><span class="sxs-lookup"><span data-stu-id="a1b2a-130">Specifies the total balance due to the vendor.</span></span>|
|<span data-ttu-id="a1b2a-131">currentAmount</span><span class="sxs-lookup"><span data-stu-id="a1b2a-131">currentAmount</span></span>  |<span data-ttu-id="a1b2a-132">numerischen</span><span class="sxs-lookup"><span data-stu-id="a1b2a-132">numeric</span></span>   |<span data-ttu-id="a1b2a-133">Gibt den Saldo vor dem ersten Fälligkeits Zeitraum an.</span><span class="sxs-lookup"><span data-stu-id="a1b2a-133">Specifies balance before first aging period.</span></span>|
|<span data-ttu-id="a1b2a-134">period1Amount</span><span class="sxs-lookup"><span data-stu-id="a1b2a-134">period1Amount</span></span>  |<span data-ttu-id="a1b2a-135">numerischen</span><span class="sxs-lookup"><span data-stu-id="a1b2a-135">numeric</span></span>   |<span data-ttu-id="a1b2a-136">Gibt den Saldo im ersten Alterungszeitraum an.</span><span class="sxs-lookup"><span data-stu-id="a1b2a-136">Specifies balance in the first aging period.</span></span>|
|<span data-ttu-id="a1b2a-137">period2Amount</span><span class="sxs-lookup"><span data-stu-id="a1b2a-137">period2Amount</span></span>  |<span data-ttu-id="a1b2a-138">numerischen</span><span class="sxs-lookup"><span data-stu-id="a1b2a-138">numeric</span></span>   |<span data-ttu-id="a1b2a-139">Gibt den Saldo im zweiten Alterungszeitraum an.</span><span class="sxs-lookup"><span data-stu-id="a1b2a-139">Specifies balance in the second aging period.</span></span>|
|<span data-ttu-id="a1b2a-140">period3Amount</span><span class="sxs-lookup"><span data-stu-id="a1b2a-140">period3Amount</span></span>  |<span data-ttu-id="a1b2a-141">numerischen</span><span class="sxs-lookup"><span data-stu-id="a1b2a-141">numeric</span></span>   |<span data-ttu-id="a1b2a-142">Gibt den Saldo im dritten Alterungszeitraum an.</span><span class="sxs-lookup"><span data-stu-id="a1b2a-142">Specifies balance in the third aging period.</span></span>|
|<span data-ttu-id="a1b2a-143">agedAsOfDate</span><span class="sxs-lookup"><span data-stu-id="a1b2a-143">agedAsOfDate</span></span>   |<span data-ttu-id="a1b2a-144">date</span><span class="sxs-lookup"><span data-stu-id="a1b2a-144">date</span></span>|<span data-ttu-id="a1b2a-145">Gibt den Zeitraum an, der zum Berechnen von Alterungs Perioden verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="a1b2a-145">Specifies period start date used to calculate aging periods.</span></span>|
|<span data-ttu-id="a1b2a-146">periodLengthFilter</span><span class="sxs-lookup"><span data-stu-id="a1b2a-146">periodLengthFilter</span></span>|<span data-ttu-id="a1b2a-147">string</span><span class="sxs-lookup"><span data-stu-id="a1b2a-147">string</span></span> |<span data-ttu-id="a1b2a-148">Gibt die Länge der Punkte an.</span><span class="sxs-lookup"><span data-stu-id="a1b2a-148">Specifies the length of the periods.</span></span> <span data-ttu-id="a1b2a-149">Zulässige Werte für die Zeiteinheiten sind: D, WD, W, M, Q oder Y. C, was bedeutet, dass die aktuelle Zeiteinheit auf dem Datum basiert, als Präfix für die Zeiteinheit angegeben werden kann.</span><span class="sxs-lookup"><span data-stu-id="a1b2a-149">Acceptable values for the time units are: D, WD, W, M, Q, or Y. C, meaning current time unit based on date, can be specified as a prefix to the time unit.</span></span>|


## <a name="relationships"></a><span data-ttu-id="a1b2a-150">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a1b2a-150">Relationships</span></span>
<span data-ttu-id="a1b2a-151">Keine</span><span class="sxs-lookup"><span data-stu-id="a1b2a-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a1b2a-152">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a1b2a-152">JSON representation</span></span>

<span data-ttu-id="a1b2a-153">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a1b2a-153">Here is a JSON representation of the resource.</span></span>


```json
{
    "vendorId": "GUID",
    "vendorNumber": "string",
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
