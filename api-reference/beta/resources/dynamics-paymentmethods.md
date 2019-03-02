---
title: paymentMethods-Ressourcentyp
description: Ein Zahlungsmethoden Objekt in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 1e4cd044d4b552a9239b742efb302633524ce22b
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366648"
---
# <a name="paymentmethods-resource-type"></a><span data-ttu-id="c3ae4-103">paymentMethods-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c3ae4-103">paymentMethods resource type</span></span>
<span data-ttu-id="c3ae4-104">Stellt eine Zahlungsmethode in Dynamics 365 Business Central dar, beispielsweise PayPal, Kreditkarte und Bankkonto.</span><span class="sxs-lookup"><span data-stu-id="c3ae4-104">Represents a method of payment in Dynamics 365 Business Central, such as PayPal, credit card, and bank account.</span></span>

## <a name="methods"></a><span data-ttu-id="c3ae4-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="c3ae4-105">Methods</span></span>

| <span data-ttu-id="c3ae4-106">Methode</span><span class="sxs-lookup"><span data-stu-id="c3ae4-106">Method</span></span>                                                          | <span data-ttu-id="c3ae4-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="c3ae4-107">Return Type</span></span>  |<span data-ttu-id="c3ae4-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c3ae4-108">Description</span></span>             |
|:----------------------------------------------------------------|:-------------|:-----------------------|
|[<span data-ttu-id="c3ae4-109">PaymentMethods abrufen</span><span class="sxs-lookup"><span data-stu-id="c3ae4-109">Get paymentMethods</span></span>](../api/dynamics-paymentmethods-get.md)      |<span data-ttu-id="c3ae4-110">paymentMethods</span><span class="sxs-lookup"><span data-stu-id="c3ae4-110">paymentMethods</span></span>|<span data-ttu-id="c3ae4-111">Ruft ein Zahlungsmethoden Objekt ab.</span><span class="sxs-lookup"><span data-stu-id="c3ae4-111">Gets a payment method object.</span></span>   |
|[<span data-ttu-id="c3ae4-112">Post paymentMethods</span><span class="sxs-lookup"><span data-stu-id="c3ae4-112">Post paymentMethods</span></span>](../api/dynamics-create-paymentmethods.md)  |<span data-ttu-id="c3ae4-113">paymentMethods</span><span class="sxs-lookup"><span data-stu-id="c3ae4-113">paymentMethods</span></span>|<span data-ttu-id="c3ae4-114">Erstellt ein Zahlungsmethoden Objekt.</span><span class="sxs-lookup"><span data-stu-id="c3ae4-114">Creates a payment method object.</span></span>|
|[<span data-ttu-id="c3ae4-115">Patch-paymentMethods</span><span class="sxs-lookup"><span data-stu-id="c3ae4-115">Patch paymentMethods</span></span>](../api/dynamics-paymentmethods-update.md) |<span data-ttu-id="c3ae4-116">paymentMethods</span><span class="sxs-lookup"><span data-stu-id="c3ae4-116">paymentMethods</span></span>|<span data-ttu-id="c3ae4-117">Aktualisiert ein Zahlungsmethoden Objekt.</span><span class="sxs-lookup"><span data-stu-id="c3ae4-117">Updates a payment method object.</span></span>|
|[<span data-ttu-id="c3ae4-118">PaymentMethods löschen</span><span class="sxs-lookup"><span data-stu-id="c3ae4-118">Delete paymentMethods</span></span>](../api/dynamics-paymentmethods-delete.md)|<span data-ttu-id="c3ae4-119">Keine</span><span class="sxs-lookup"><span data-stu-id="c3ae4-119">none</span></span>          |<span data-ttu-id="c3ae4-120">Löscht ein Zahlungsmethoden Objekt.</span><span class="sxs-lookup"><span data-stu-id="c3ae4-120">Deletes a payment method object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c3ae4-121">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c3ae4-121">Properties</span></span>
| <span data-ttu-id="c3ae4-122">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c3ae4-122">Property</span></span>           | <span data-ttu-id="c3ae4-123">Typ</span><span class="sxs-lookup"><span data-stu-id="c3ae4-123">Type</span></span>   |<span data-ttu-id="c3ae4-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c3ae4-124">Description</span></span>                                                  |
|:-------------------|:-------|:------------------------------------------------------------|
|<span data-ttu-id="c3ae4-125">id</span><span class="sxs-lookup"><span data-stu-id="c3ae4-125">id</span></span>                  |<span data-ttu-id="c3ae4-126">GUID</span><span class="sxs-lookup"><span data-stu-id="c3ae4-126">GUID</span></span>    |<span data-ttu-id="c3ae4-127">Die eindeutige ID des paymentMethods.</span><span class="sxs-lookup"><span data-stu-id="c3ae4-127">The unique ID of the paymentMethods.</span></span> <span data-ttu-id="c3ae4-128">Nicht bearbeitbar.</span><span class="sxs-lookup"><span data-stu-id="c3ae4-128">Non-editable.</span></span>           |
|<span data-ttu-id="c3ae4-129">code</span><span class="sxs-lookup"><span data-stu-id="c3ae4-129">code</span></span>                |<span data-ttu-id="c3ae4-130">string</span><span class="sxs-lookup"><span data-stu-id="c3ae4-130">string</span></span>  |<span data-ttu-id="c3ae4-131">Gibt den Zahlungsmethoden Code an.</span><span class="sxs-lookup"><span data-stu-id="c3ae4-131">Specifies the payment method code.</span></span>                           |
|<span data-ttu-id="c3ae4-132">displayName</span><span class="sxs-lookup"><span data-stu-id="c3ae4-132">displayName</span></span>         |<span data-ttu-id="c3ae4-133">string</span><span class="sxs-lookup"><span data-stu-id="c3ae4-133">string</span></span>  |<span data-ttu-id="c3ae4-134">Gibt den Anzeigenamen der Zahlungsmethode an.</span><span class="sxs-lookup"><span data-stu-id="c3ae4-134">Specifies the payment method display name.</span></span>                   |
|<span data-ttu-id="c3ae4-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c3ae4-135">lastModifiedDateTime</span></span>|<span data-ttu-id="c3ae4-136">DateTime</span><span class="sxs-lookup"><span data-stu-id="c3ae4-136">datetime</span></span>|<span data-ttu-id="c3ae4-137">Die letzte DateTime, die die Zahlungsmethode geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="c3ae4-137">The last datetime the payment method was modified.</span></span> <span data-ttu-id="c3ae4-138">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c3ae4-138">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="c3ae4-139">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c3ae4-139">Relationships</span></span>
<span data-ttu-id="c3ae4-140">Keine</span><span class="sxs-lookup"><span data-stu-id="c3ae4-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c3ae4-141">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c3ae4-141">JSON representation</span></span>

<span data-ttu-id="c3ae4-142">Es folgt eine JSON-Darstellung des paymentMethods.</span><span class="sxs-lookup"><span data-stu-id="c3ae4-142">Here is a JSON representation of the paymentMethods.</span></span>


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}

```
