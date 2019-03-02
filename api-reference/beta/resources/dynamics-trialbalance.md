---
title: trialBalance-Ressourcentyp
description: Ein Test-Balance-Objekt in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 1a7e906e50ddf39e4c9e2d3d9dde11226c7ec662
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365325"
---
# <a name="trialbalance-resource-type"></a><span data-ttu-id="aa2ec-103">trialBalance-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="aa2ec-103">trialBalance resource type</span></span>
<span data-ttu-id="aa2ec-104">Stellt einen Test Saldo in Dynamics 365 Business Central dar.</span><span class="sxs-lookup"><span data-stu-id="aa2ec-104">Represents a trial balance in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="aa2ec-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="aa2ec-105">Methods</span></span>

| <span data-ttu-id="aa2ec-106">Methode</span><span class="sxs-lookup"><span data-stu-id="aa2ec-106">Method</span></span>       | <span data-ttu-id="aa2ec-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="aa2ec-107">Return Type</span></span>  |<span data-ttu-id="aa2ec-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aa2ec-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="aa2ec-109">TrialBalance abrufen</span><span class="sxs-lookup"><span data-stu-id="aa2ec-109">Get trialBalance</span></span>](../api/dynamics-trialbalance-get.md)|<span data-ttu-id="aa2ec-110">trialBalance</span><span class="sxs-lookup"><span data-stu-id="aa2ec-110">trialBalance</span></span>|<span data-ttu-id="aa2ec-111">Ruft ein Test Balance-Objekt ab.</span><span class="sxs-lookup"><span data-stu-id="aa2ec-111">Gets a trial balance object.</span></span>|

## <a name="properties"></a><span data-ttu-id="aa2ec-112">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="aa2ec-112">Properties</span></span>
| <span data-ttu-id="aa2ec-113">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="aa2ec-113">Property</span></span>     | <span data-ttu-id="aa2ec-114">Typ</span><span class="sxs-lookup"><span data-stu-id="aa2ec-114">Type</span></span>   |<span data-ttu-id="aa2ec-115">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aa2ec-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aa2ec-116">number</span><span class="sxs-lookup"><span data-stu-id="aa2ec-116">number</span></span>|<span data-ttu-id="aa2ec-117">string</span><span class="sxs-lookup"><span data-stu-id="aa2ec-117">string</span></span>|<span data-ttu-id="aa2ec-118">Die sachKontonummer für das trialBalance-Element</span><span class="sxs-lookup"><span data-stu-id="aa2ec-118">The G/L Account number for the trialBalance item</span></span>|
|<span data-ttu-id="aa2ec-119">accountId</span><span class="sxs-lookup"><span data-stu-id="aa2ec-119">accountId</span></span>|<span data-ttu-id="aa2ec-120">GUID</span><span class="sxs-lookup"><span data-stu-id="aa2ec-120">GUID</span></span>|<span data-ttu-id="aa2ec-121">Der eindeutige Bezeichner für das Sachkonto des Record-Elements.</span><span class="sxs-lookup"><span data-stu-id="aa2ec-121">The unique identifier for the G/L account of the record.</span></span>|
|<span data-ttu-id="aa2ec-122">accountType</span><span class="sxs-lookup"><span data-stu-id="aa2ec-122">accountType</span></span>|<span data-ttu-id="aa2ec-123">string</span><span class="sxs-lookup"><span data-stu-id="aa2ec-123">string</span></span>|<span data-ttu-id="aa2ec-124">Der Kontotyp des Sachkontos des Datensatzes.</span><span class="sxs-lookup"><span data-stu-id="aa2ec-124">The account type of the G/L account of the record.</span></span>|
|<span data-ttu-id="aa2ec-125">Anzeige</span><span class="sxs-lookup"><span data-stu-id="aa2ec-125">display</span></span>|<span data-ttu-id="aa2ec-126">string</span><span class="sxs-lookup"><span data-stu-id="aa2ec-126">string</span></span>|<span data-ttu-id="aa2ec-127">Der sachKontoname für das trialBalance-Element.</span><span class="sxs-lookup"><span data-stu-id="aa2ec-127">The G/L Account name for the trialBalance item.</span></span>|
|<span data-ttu-id="aa2ec-128">totalDebit</span><span class="sxs-lookup"><span data-stu-id="aa2ec-128">totalDebit</span></span>|<span data-ttu-id="aa2ec-129">string</span><span class="sxs-lookup"><span data-stu-id="aa2ec-129">string</span></span>|<span data-ttu-id="aa2ec-130">Stellt den gesamten Sollbetrag im sachKonto dar.</span><span class="sxs-lookup"><span data-stu-id="aa2ec-130">Represents total debit amount in G/L Account.</span></span>|
|<span data-ttu-id="aa2ec-131">totalCredit</span><span class="sxs-lookup"><span data-stu-id="aa2ec-131">totalCredit</span></span>|<span data-ttu-id="aa2ec-132">string</span><span class="sxs-lookup"><span data-stu-id="aa2ec-132">string</span></span>|<span data-ttu-id="aa2ec-133">Stellt den gesamten Guthabenbetrag im sachKonto dar.</span><span class="sxs-lookup"><span data-stu-id="aa2ec-133">Represents total credit amount in G/L Account.</span></span>|
|<span data-ttu-id="aa2ec-134">balanceAtDateDebit</span><span class="sxs-lookup"><span data-stu-id="aa2ec-134">balanceAtDateDebit</span></span>|<span data-ttu-id="aa2ec-135">string</span><span class="sxs-lookup"><span data-stu-id="aa2ec-135">string</span></span>|<span data-ttu-id="aa2ec-136">Stellt einen positiven Saldo in einem sachKonto dar.</span><span class="sxs-lookup"><span data-stu-id="aa2ec-136">Represents positive Balance at Date amount in G/L Account.</span></span>|
|<span data-ttu-id="aa2ec-137">balanceAtDateCredit</span><span class="sxs-lookup"><span data-stu-id="aa2ec-137">balanceAtDateCredit</span></span>|<span data-ttu-id="aa2ec-138">string</span><span class="sxs-lookup"><span data-stu-id="aa2ec-138">string</span></span>|<span data-ttu-id="aa2ec-139">Stellt einen negativen Saldo in einem sachKonto dar.</span><span class="sxs-lookup"><span data-stu-id="aa2ec-139">Represents negative Balance at Date amount in G/L Account.</span></span>|
|<span data-ttu-id="aa2ec-140">dateFilter</span><span class="sxs-lookup"><span data-stu-id="aa2ec-140">dateFilter</span></span>|<span data-ttu-id="aa2ec-141">date</span><span class="sxs-lookup"><span data-stu-id="aa2ec-141">date</span></span>|<span data-ttu-id="aa2ec-142">Der Datumsfilter, der zum Berechnen der trialBalance-Elemente verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="aa2ec-142">The date filter used to calculate the trialBalance items.</span></span>|


## <a name="relationships"></a><span data-ttu-id="aa2ec-143">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="aa2ec-143">Relationships</span></span>
<span data-ttu-id="aa2ec-144">Keine</span><span class="sxs-lookup"><span data-stu-id="aa2ec-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aa2ec-145">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="aa2ec-145">JSON representation</span></span>

<span data-ttu-id="aa2ec-146">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="aa2ec-146">Here is a JSON representation of the resource.</span></span>


```json
{
    "number": "string",
    "accountId": "GUID",
    "accountType": "string",
    "display": "string",
    "totalDebit": "string",
    "totalCredit": "string",
    "balanceAtDateDebit": "string",
    "balanceAtDateCredit": "string",
    "dateFilter": "date"
}

```

