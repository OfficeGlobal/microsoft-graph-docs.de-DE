---
title: shipmentMethods-Ressourcentyp
description: Eine Sendungs Methode in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 2f7ef9611fc85c13ac24c79b292e06a6bdc5d587
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365500"
---
# <a name="shipmentmethods-resource-type"></a><span data-ttu-id="29b10-103">shipmentMethods-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="29b10-103">shipmentMethods resource type</span></span>
<span data-ttu-id="29b10-104">Stellt eine Versandmethode in Dynamics 365 Business Central dar, beispielsweise UPS, FedEx und DHL.</span><span class="sxs-lookup"><span data-stu-id="29b10-104">Represents a method of shipment in Dynamics 365 Business Central, such as UPS, Fedex, and DHL.</span></span>

## <a name="methods"></a><span data-ttu-id="29b10-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="29b10-105">Methods</span></span>

| <span data-ttu-id="29b10-106">Methode</span><span class="sxs-lookup"><span data-stu-id="29b10-106">Method</span></span>       | <span data-ttu-id="29b10-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="29b10-107">Return Type</span></span>  |<span data-ttu-id="29b10-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="29b10-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="29b10-109">ShipmentMethods abrufen</span><span class="sxs-lookup"><span data-stu-id="29b10-109">Get shipmentMethods</span></span>](../api/dynamics-shipmentmethods-get.md)|<span data-ttu-id="29b10-110">shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="29b10-110">shipmentMethods</span></span>|<span data-ttu-id="29b10-111">Ruft eine Sendungs Methode ab.</span><span class="sxs-lookup"><span data-stu-id="29b10-111">Gets a shipment method.</span></span>|
|[<span data-ttu-id="29b10-112">Post shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="29b10-112">Post shipmentMethods</span></span>](../api/dynamics-create-shipmentmethods.md)|<span data-ttu-id="29b10-113">shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="29b10-113">shipmentMethods</span></span>|<span data-ttu-id="29b10-114">Erstellt eine Transportmethode.</span><span class="sxs-lookup"><span data-stu-id="29b10-114">Creates a shipment method.</span></span>|
|[<span data-ttu-id="29b10-115">Patch-shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="29b10-115">Patch shipmentMethods</span></span>](../api/dynamics-shipmentmethods-update.md)|<span data-ttu-id="29b10-116">shipmentMethods</span><span class="sxs-lookup"><span data-stu-id="29b10-116">shipmentMethods</span></span>|<span data-ttu-id="29b10-117">Aktualisiert eine Transportmethode.</span><span class="sxs-lookup"><span data-stu-id="29b10-117">Updates a shipment method.</span></span>|
|[<span data-ttu-id="29b10-118">ShipmentMethods löschen</span><span class="sxs-lookup"><span data-stu-id="29b10-118">Delete shipmentMethods</span></span>](../api/dynamics-shipmentmethods-delete.md)|<span data-ttu-id="29b10-119">Keine</span><span class="sxs-lookup"><span data-stu-id="29b10-119">none</span></span>|<span data-ttu-id="29b10-120">Löscht eine Transportmethode.</span><span class="sxs-lookup"><span data-stu-id="29b10-120">Deletes a shipment method.</span></span>|

## <a name="properties"></a><span data-ttu-id="29b10-121">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="29b10-121">Properties</span></span>
| <span data-ttu-id="29b10-122">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="29b10-122">Property</span></span>     | <span data-ttu-id="29b10-123">Typ</span><span class="sxs-lookup"><span data-stu-id="29b10-123">Type</span></span>   |<span data-ttu-id="29b10-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="29b10-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="29b10-125">id</span><span class="sxs-lookup"><span data-stu-id="29b10-125">id</span></span>|<span data-ttu-id="29b10-126">GUID</span><span class="sxs-lookup"><span data-stu-id="29b10-126">GUID</span></span>|<span data-ttu-id="29b10-127">Die eindeutige ID des shipmentMethod.</span><span class="sxs-lookup"><span data-stu-id="29b10-127">The unique ID of the shipmentMethod.</span></span> <span data-ttu-id="29b10-128">Nicht bearbeitbar.</span><span class="sxs-lookup"><span data-stu-id="29b10-128">Non-editable.</span></span>|
|<span data-ttu-id="29b10-129">code</span><span class="sxs-lookup"><span data-stu-id="29b10-129">code</span></span>|<span data-ttu-id="29b10-130">string</span><span class="sxs-lookup"><span data-stu-id="29b10-130">string</span></span>|<span data-ttu-id="29b10-131">Gibt den Code der Transportmethode an.</span><span class="sxs-lookup"><span data-stu-id="29b10-131">Specifies the shipment method code.</span></span>|
|<span data-ttu-id="29b10-132">displayName</span><span class="sxs-lookup"><span data-stu-id="29b10-132">displayName</span></span>|<span data-ttu-id="29b10-133">string</span><span class="sxs-lookup"><span data-stu-id="29b10-133">string</span></span>|<span data-ttu-id="29b10-134">Gibt den Anzeigenamen der Sendungs Methode an.</span><span class="sxs-lookup"><span data-stu-id="29b10-134">Specifies the shipment method display name.</span></span>|
|<span data-ttu-id="29b10-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="29b10-135">lastModifiedDateTime</span></span>|<span data-ttu-id="29b10-136">DateTime</span><span class="sxs-lookup"><span data-stu-id="29b10-136">datetime</span></span>|<span data-ttu-id="29b10-137">Die letzte DateTime, die die Sendungs Methode geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="29b10-137">The last datetime the shipment method was modified.</span></span> <span data-ttu-id="29b10-138">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="29b10-138">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="29b10-139">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="29b10-139">Relationships</span></span>
<span data-ttu-id="29b10-140">Keine</span><span class="sxs-lookup"><span data-stu-id="29b10-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="29b10-141">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="29b10-141">JSON representation</span></span>

<span data-ttu-id="29b10-142">Es folgt eine JSON-Darstellung des shipmentMethod.</span><span class="sxs-lookup"><span data-stu-id="29b10-142">Here is a JSON representation of the shipmentMethod.</span></span>

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}

```


