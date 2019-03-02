---
title: generalLedgerEntries-Ressourcentyp
description: Ein Hauptbuch-Eintrag in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 0a5701451bf96773428b12b6bb715320e2ba81b5
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365759"
---
# <a name="generalledgerentries-resource-type"></a><span data-ttu-id="daad3-103">generalLedgerEntries-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="daad3-103">generalLedgerEntries resource type</span></span>
<span data-ttu-id="daad3-104">Stellt ein generalLedgerEntry-Objekt in Dynamics 365 Business Central dar.</span><span class="sxs-lookup"><span data-stu-id="daad3-104">Represents a generalLedgerEntry object in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="daad3-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="daad3-105">Methods</span></span>

| <span data-ttu-id="daad3-106">Methode</span><span class="sxs-lookup"><span data-stu-id="daad3-106">Method</span></span>       | <span data-ttu-id="daad3-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="daad3-107">Return Type</span></span>  |<span data-ttu-id="daad3-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="daad3-108">Description</span></span>|
|:-------------|:-------------|:----------|
|[<span data-ttu-id="daad3-109">GeneralLedgerEntries abrufen</span><span class="sxs-lookup"><span data-stu-id="daad3-109">Get generalLedgerEntries</span></span>](../api/dynamics-generalledgerentries-get.md)|<span data-ttu-id="daad3-110">generalLedgerEntries</span><span class="sxs-lookup"><span data-stu-id="daad3-110">generalLedgerEntries</span></span>|<span data-ttu-id="daad3-111">Ein G/L-Eintrags Objekt abrufen.</span><span class="sxs-lookup"><span data-stu-id="daad3-111">Get a G/L entry object.</span></span>|

## <a name="properties"></a><span data-ttu-id="daad3-112">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="daad3-112">Properties</span></span>
| <span data-ttu-id="daad3-113">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="daad3-113">Property</span></span>           | <span data-ttu-id="daad3-114">Typ</span><span class="sxs-lookup"><span data-stu-id="daad3-114">Type</span></span>                  |<span data-ttu-id="daad3-115">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="daad3-115">Description</span></span>                                  |
|:-------------------|:----------------------|:--------------------------------------------|
|<span data-ttu-id="daad3-116">id</span><span class="sxs-lookup"><span data-stu-id="daad3-116">id</span></span>                  |<span data-ttu-id="daad3-117">numerischen</span><span class="sxs-lookup"><span data-stu-id="daad3-117">numeric</span></span>                |<span data-ttu-id="daad3-118">Die eindeutige ID des G/L-Eintrags.</span><span class="sxs-lookup"><span data-stu-id="daad3-118">The unique ID of the G/L Entry.</span></span>              |
|<span data-ttu-id="daad3-119">postingDate</span><span class="sxs-lookup"><span data-stu-id="daad3-119">postingDate</span></span>         |<span data-ttu-id="daad3-120">date</span><span class="sxs-lookup"><span data-stu-id="daad3-120">date</span></span>                   |<span data-ttu-id="daad3-121">Gibt das Buchungsdatum des Fibu-Eintrags an.</span><span class="sxs-lookup"><span data-stu-id="daad3-121">Specifies the posting date of the G/L Entry.</span></span> |
|<span data-ttu-id="daad3-122">documentNumber</span><span class="sxs-lookup"><span data-stu-id="daad3-122">documentNumber</span></span>      |<span data-ttu-id="daad3-123">Zeichenfolge, maximale Größe 20</span><span class="sxs-lookup"><span data-stu-id="daad3-123">string, maximum size 20</span></span>|<span data-ttu-id="daad3-124">Gibt die Dokumentnummer des G/L-Eintrags an.</span><span class="sxs-lookup"><span data-stu-id="daad3-124">Specifies the document number of the G/L Entry.</span></span>|
|<span data-ttu-id="daad3-125">documentType</span><span class="sxs-lookup"><span data-stu-id="daad3-125">documentType</span></span>        |<span data-ttu-id="daad3-126">string</span><span class="sxs-lookup"><span data-stu-id="daad3-126">string</span></span>                 |<span data-ttu-id="daad3-127">Gibt den Dokumenttyp des G/L-Eintrags an.</span><span class="sxs-lookup"><span data-stu-id="daad3-127">Specifies the document type of the G/L Entry.</span></span>|
|<span data-ttu-id="daad3-128">accountId</span><span class="sxs-lookup"><span data-stu-id="daad3-128">accountId</span></span>           |<span data-ttu-id="daad3-129">GUID</span><span class="sxs-lookup"><span data-stu-id="daad3-129">GUID</span></span>                   |<span data-ttu-id="daad3-130">Gibt die Konto-Nr. des G/L-Eintrags an.</span><span class="sxs-lookup"><span data-stu-id="daad3-130">Specifies the accountId of the G/L Entry.</span></span>    |
|<span data-ttu-id="daad3-131">accountNumber</span><span class="sxs-lookup"><span data-stu-id="daad3-131">accountNumber</span></span>       |<span data-ttu-id="daad3-132">Zeichenfolge, maximale Größe 20</span><span class="sxs-lookup"><span data-stu-id="daad3-132">string, maximum size 20</span></span>|<span data-ttu-id="daad3-133">Gibt die accountNumber des G/L-Eintrags an.</span><span class="sxs-lookup"><span data-stu-id="daad3-133">Specifies the accountNumber of the G/L Entry.</span></span>|
|<span data-ttu-id="daad3-134">description</span><span class="sxs-lookup"><span data-stu-id="daad3-134">description</span></span>         |<span data-ttu-id="daad3-135">Zeichenfolge, maximale Größe 50</span><span class="sxs-lookup"><span data-stu-id="daad3-135">string, maximum size 50</span></span>|<span data-ttu-id="daad3-136">Gibt die Beschreibung des G/L-Eintrags an.</span><span class="sxs-lookup"><span data-stu-id="daad3-136">Specifies the description of the G/L Entry.</span></span>  |
|<span data-ttu-id="daad3-137">debitAmount</span><span class="sxs-lookup"><span data-stu-id="daad3-137">debitAmount</span></span>         |<span data-ttu-id="daad3-138">numerischen</span><span class="sxs-lookup"><span data-stu-id="daad3-138">numeric</span></span>                |<span data-ttu-id="daad3-139">Gibt die debitAmount des G/L-Eintrags an.</span><span class="sxs-lookup"><span data-stu-id="daad3-139">Specifies the debitAmount of the G/L Entry.</span></span>  |
|<span data-ttu-id="daad3-140">creditAmount</span><span class="sxs-lookup"><span data-stu-id="daad3-140">creditAmount</span></span>        |<span data-ttu-id="daad3-141">numerischen</span><span class="sxs-lookup"><span data-stu-id="daad3-141">numeric</span></span>                |<span data-ttu-id="daad3-142">Gibt die creditAmount des G/L-Eintrags an.</span><span class="sxs-lookup"><span data-stu-id="daad3-142">Specifies the creditAmount of the G/L Entry.</span></span> |
|<span data-ttu-id="daad3-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="daad3-143">lastModifiedDateTime</span></span>|<span data-ttu-id="daad3-144">DateTime</span><span class="sxs-lookup"><span data-stu-id="daad3-144">datetime</span></span>               |<span data-ttu-id="daad3-145">Die letzte DateTime, die der G/L-Eintrag geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="daad3-145">The last datetime the G/L Entry was modified.</span></span>|


## <a name="relationships"></a><span data-ttu-id="daad3-146">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="daad3-146">Relationships</span></span>
<span data-ttu-id="daad3-147">Keine</span><span class="sxs-lookup"><span data-stu-id="daad3-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="daad3-148">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="daad3-148">JSON representation</span></span>

<span data-ttu-id="daad3-149">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="daad3-149">Here is a JSON representation of the resource.</span></span>


```json
{
  "id": "int",
  "postingDate": "Date",
  "documentNumber": "string",
  "documentType": "string",
  "accountId": "GUID",
  "accountNumber": "string",
  "description": "string",
  "debitAmount": "decimal",
  "creditAmount": "decimal",
  "lastModifiedDateTime": "datetime"
}

```

