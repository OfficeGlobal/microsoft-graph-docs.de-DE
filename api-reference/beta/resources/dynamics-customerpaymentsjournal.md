---
title: customerPaymentJournals-Ressourcentyp
description: Ein Kunden Zahlungsjournal in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: a8b01124db732866e1a7b971af57d7e0a2b692e1
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365738"
---
# <a name="customerpaymentsjournals-resource-type"></a><span data-ttu-id="7864f-103">customerPaymentsJournals-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="7864f-103">customerPaymentsJournals resource type</span></span>
<span data-ttu-id="7864f-104">Stellt ein Debitoren Zahlungsjournal in Dynamics 365 Business Central dar.</span><span class="sxs-lookup"><span data-stu-id="7864f-104">Represents a customer payment journal in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="7864f-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="7864f-105">Methods</span></span>

| <span data-ttu-id="7864f-106">Methode</span><span class="sxs-lookup"><span data-stu-id="7864f-106">Method</span></span>               | <span data-ttu-id="7864f-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="7864f-107">Return Type</span></span>             |<span data-ttu-id="7864f-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7864f-108">Description</span></span>                      |
|:---------------------|:------------------------|:--------------------------------|
|[<span data-ttu-id="7864f-109">CustomerPaymentJournals abrufen</span><span class="sxs-lookup"><span data-stu-id="7864f-109">Get customerPaymentJournals</span></span>](../api/dynamics-customerpaymentsjournal-get.md)      |<span data-ttu-id="7864f-110">customerPaymentJournals</span><span class="sxs-lookup"><span data-stu-id="7864f-110">customerPaymentJournals</span></span>|<span data-ttu-id="7864f-111">Ruft ein Debitoren Zahlungsjournal ab.</span><span class="sxs-lookup"><span data-stu-id="7864f-111">Gets a customer payment journal.</span></span>   |
|[<span data-ttu-id="7864f-112">Post customerPaymentJournals</span><span class="sxs-lookup"><span data-stu-id="7864f-112">Post customerPaymentJournals</span></span>](../api/dynamics-create-customerpaymentsjournal.md)  |<span data-ttu-id="7864f-113">customerPaymentJournals</span><span class="sxs-lookup"><span data-stu-id="7864f-113">customerPaymentJournals</span></span>|<span data-ttu-id="7864f-114">Erstellt ein Debitoren Zahlungsjournal.</span><span class="sxs-lookup"><span data-stu-id="7864f-114">Creates a customer payment journal.</span></span>|
|[<span data-ttu-id="7864f-115">Patch-customerPaymentJournals</span><span class="sxs-lookup"><span data-stu-id="7864f-115">Patch customerPaymentJournals</span></span>](../api/dynamics-customerpaymentsjournal-update.md) |<span data-ttu-id="7864f-116">customerPaymentJournals</span><span class="sxs-lookup"><span data-stu-id="7864f-116">customerPaymentJournals</span></span>|<span data-ttu-id="7864f-117">Aktualisiert ein Debitoren Zahlungsjournal.</span><span class="sxs-lookup"><span data-stu-id="7864f-117">Updates a customer payment journal.</span></span>|
|[<span data-ttu-id="7864f-118">CustomerPaymentJournals löschen</span><span class="sxs-lookup"><span data-stu-id="7864f-118">Delete customerPaymentJournals</span></span>](../api/dynamics-customerpaymentsjournal-delete.md)|<span data-ttu-id="7864f-119">Keine</span><span class="sxs-lookup"><span data-stu-id="7864f-119">none</span></span>                     |<span data-ttu-id="7864f-120">Löscht ein Debitoren-Zahlungs Blatt.</span><span class="sxs-lookup"><span data-stu-id="7864f-120">Deletes a customer payment journal.</span></span>|

## <a name="properties"></a><span data-ttu-id="7864f-121">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7864f-121">Properties</span></span>
| <span data-ttu-id="7864f-122">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7864f-122">Property</span></span>           | <span data-ttu-id="7864f-123">Typ</span><span class="sxs-lookup"><span data-stu-id="7864f-123">Type</span></span>                  |<span data-ttu-id="7864f-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7864f-124">Description</span></span>                                                             |
|:-------------------|:----------------------|:-----------------------------------------------------------------------|
|<span data-ttu-id="7864f-125">id</span><span class="sxs-lookup"><span data-stu-id="7864f-125">id</span></span>                  |<span data-ttu-id="7864f-126">GUID</span><span class="sxs-lookup"><span data-stu-id="7864f-126">GUID</span></span>                   |<span data-ttu-id="7864f-127">Die eindeutige ID des Debitoren-Zahlungs Blatts.</span><span class="sxs-lookup"><span data-stu-id="7864f-127">The unique ID of the customer payment journal.</span></span> <span data-ttu-id="7864f-128">Nicht bearbeitbar.</span><span class="sxs-lookup"><span data-stu-id="7864f-128">Non-editable.</span></span>           |
|<span data-ttu-id="7864f-129">code</span><span class="sxs-lookup"><span data-stu-id="7864f-129">code</span></span>                |<span data-ttu-id="7864f-130">Zeichenfolge, maximale Größe 10</span><span class="sxs-lookup"><span data-stu-id="7864f-130">string, maximum size 10</span></span>| <span data-ttu-id="7864f-131">Der Code des Debitoren-Zahlungs Blatts.</span><span class="sxs-lookup"><span data-stu-id="7864f-131">The code of the customer payment journal.</span></span>                             |
|<span data-ttu-id="7864f-132">displayName</span><span class="sxs-lookup"><span data-stu-id="7864f-132">displayName</span></span>         |<span data-ttu-id="7864f-133">Zeichenfolge, maximale Größe 50</span><span class="sxs-lookup"><span data-stu-id="7864f-133">string, maximum size 50</span></span>| <span data-ttu-id="7864f-134">Der Anzeigename des Debitoren-Zahlungs Blatts.</span><span class="sxs-lookup"><span data-stu-id="7864f-134">The display name of the customer payment journal.</span></span>                     |
|<span data-ttu-id="7864f-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7864f-135">lastModifiedDateTime</span></span>|<span data-ttu-id="7864f-136">DateTime</span><span class="sxs-lookup"><span data-stu-id="7864f-136">datetime</span></span>               |<span data-ttu-id="7864f-137">Die letzte Uhrzeit, zu der das Debitoren Zahlungsjournal geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="7864f-137">The last datetime the customer payment journal was modified.</span></span> <span data-ttu-id="7864f-138">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7864f-138">Read-Only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7864f-139">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="7864f-139">Relationships</span></span>

## <a name="json-representation"></a><span data-ttu-id="7864f-140">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7864f-140">JSON representation</span></span>

<span data-ttu-id="7864f-141">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7864f-141">Here is a JSON representation of the resource.</span></span>


```json
{
  "id": "GUID",
  "code": "String",
  "displayName": "String",
  "lastModifiedDateTime": "datetime"
}
```

