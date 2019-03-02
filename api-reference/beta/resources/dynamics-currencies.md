---
title: Ressourcentyp "Währungen"
description: Ein Currency-Objekt in Dynamics 365 Business Central
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: c0d15b8d20e99537cb2f567a9f8fe12b45dbd389
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366627"
---
# <a name="currencies-resource-type"></a><span data-ttu-id="dbc0c-103">Ressourcentyp "Währungen"</span><span class="sxs-lookup"><span data-stu-id="dbc0c-103">currencies resource type</span></span>
<span data-ttu-id="dbc0c-104">Stellt eine Währung dar, die in Dynamics 365 Business Central verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="dbc0c-104">Represents a currency used in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="dbc0c-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="dbc0c-105">Methods</span></span>
| <span data-ttu-id="dbc0c-106">Methode</span><span class="sxs-lookup"><span data-stu-id="dbc0c-106">Method</span></span>                                                  |<span data-ttu-id="dbc0c-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="dbc0c-107">Return Type</span></span>|<span data-ttu-id="dbc0c-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dbc0c-108">Description</span></span>       |
|:--------------------------------------------------------|:----------|:-----------------|
|[<span data-ttu-id="dbc0c-109">Währungen abrufen</span><span class="sxs-lookup"><span data-stu-id="dbc0c-109">Get currencies</span></span>](../api/dynamics-currencies-get.md)      |<span data-ttu-id="dbc0c-110">Währungen</span><span class="sxs-lookup"><span data-stu-id="dbc0c-110">currencies</span></span> |<span data-ttu-id="dbc0c-111">Holen Sie sich eine Währung.</span><span class="sxs-lookup"><span data-stu-id="dbc0c-111">Get a Currency.</span></span>   |
|[<span data-ttu-id="dbc0c-112">Post Währungen</span><span class="sxs-lookup"><span data-stu-id="dbc0c-112">Post currencies</span></span>](../api/dynamics-create-currencies.md)  |<span data-ttu-id="dbc0c-113">Währungen</span><span class="sxs-lookup"><span data-stu-id="dbc0c-113">currencies</span></span> |<span data-ttu-id="dbc0c-114">Erstellen Sie eine Währung.</span><span class="sxs-lookup"><span data-stu-id="dbc0c-114">Create a Currency.</span></span>|
|[<span data-ttu-id="dbc0c-115">Patch-Währungen</span><span class="sxs-lookup"><span data-stu-id="dbc0c-115">Patch currencies</span></span>](../api/dynamics-currencies-update.md) |<span data-ttu-id="dbc0c-116">Währungen</span><span class="sxs-lookup"><span data-stu-id="dbc0c-116">currencies</span></span> |<span data-ttu-id="dbc0c-117">Aktualisieren einer Währung.</span><span class="sxs-lookup"><span data-stu-id="dbc0c-117">Update a Currency.</span></span>|
|[<span data-ttu-id="dbc0c-118">Währungen löschen</span><span class="sxs-lookup"><span data-stu-id="dbc0c-118">Delete currencies</span></span>](../api/dynamics-currencies-delete.md)|<span data-ttu-id="dbc0c-119">Keine</span><span class="sxs-lookup"><span data-stu-id="dbc0c-119">none</span></span>       |<span data-ttu-id="dbc0c-120">Eine Währung löschen.</span><span class="sxs-lookup"><span data-stu-id="dbc0c-120">Delete a Currency.</span></span>|

## <a name="properties"></a><span data-ttu-id="dbc0c-121">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="dbc0c-121">Properties</span></span>
| <span data-ttu-id="dbc0c-122">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="dbc0c-122">Property</span></span>              | <span data-ttu-id="dbc0c-123">Typ</span><span class="sxs-lookup"><span data-stu-id="dbc0c-123">Type</span></span>   |<span data-ttu-id="dbc0c-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dbc0c-124">Description</span></span>                                                   |
|:----------------------|:-------|:-------------------------------------------------------------|
|<span data-ttu-id="dbc0c-125">id</span><span class="sxs-lookup"><span data-stu-id="dbc0c-125">id</span></span>                     |<span data-ttu-id="dbc0c-126">GUID</span><span class="sxs-lookup"><span data-stu-id="dbc0c-126">GUID</span></span>    |<span data-ttu-id="dbc0c-127">Die eindeutige ID der Währung.</span><span class="sxs-lookup"><span data-stu-id="dbc0c-127">The unique ID of the currency.</span></span> <span data-ttu-id="dbc0c-128">Nicht bearbeitbar.</span><span class="sxs-lookup"><span data-stu-id="dbc0c-128">Non-editable.</span></span>                  |
|<span data-ttu-id="dbc0c-129">code</span><span class="sxs-lookup"><span data-stu-id="dbc0c-129">code</span></span>                   |<span data-ttu-id="dbc0c-130">string</span><span class="sxs-lookup"><span data-stu-id="dbc0c-130">string</span></span>  |<span data-ttu-id="dbc0c-131">Gibt den Währungscode an.</span><span class="sxs-lookup"><span data-stu-id="dbc0c-131">Specifies the currency code.</span></span>                                  |
|<span data-ttu-id="dbc0c-132">displayName</span><span class="sxs-lookup"><span data-stu-id="dbc0c-132">displayName</span></span>            |<span data-ttu-id="dbc0c-133">string</span><span class="sxs-lookup"><span data-stu-id="dbc0c-133">string</span></span>  |<span data-ttu-id="dbc0c-134">Gibt den Anzeigenamen der Währung an.</span><span class="sxs-lookup"><span data-stu-id="dbc0c-134">Specifies the currency display name.</span></span>                          |
|<span data-ttu-id="dbc0c-135">Symbol</span><span class="sxs-lookup"><span data-stu-id="dbc0c-135">symbol</span></span>                 |<span data-ttu-id="dbc0c-136">string</span><span class="sxs-lookup"><span data-stu-id="dbc0c-136">string</span></span>  |<span data-ttu-id="dbc0c-137">Gibt das Symbol für diese Währung an, das in Schecks angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="dbc0c-137">Specifies the symbol for this currency that appears on checks.</span></span>|
|<span data-ttu-id="dbc0c-138">amountDecimalPlaces</span><span class="sxs-lookup"><span data-stu-id="dbc0c-138">amountDecimalPlaces</span></span>    |<span data-ttu-id="dbc0c-139">string</span><span class="sxs-lookup"><span data-stu-id="dbc0c-139">string</span></span>  |<span data-ttu-id="dbc0c-140">Gibt die Anzahl der Dezimalstellen an, die vom System für Beträge für diese Währung angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="dbc0c-140">Specifies the number of decimal places the system will display on amounts for this currency.</span></span>|
|<span data-ttu-id="dbc0c-141">amountRoundingPrecision</span><span class="sxs-lookup"><span data-stu-id="dbc0c-141">amountRoundingPrecision</span></span>|<span data-ttu-id="dbc0c-142">decimal</span><span class="sxs-lookup"><span data-stu-id="dbc0c-142">decimal</span></span> |<span data-ttu-id="dbc0c-143">Gibt die Größe des Intervalls an, das beim Runden von Beträgen für diese Währung verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="dbc0c-143">Specifies the size of the interval to be used when rounding amounts for this currency.</span></span>|
|<span data-ttu-id="dbc0c-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dbc0c-144">lastModifiedDateTime</span></span>   |<span data-ttu-id="dbc0c-145">DateTime</span><span class="sxs-lookup"><span data-stu-id="dbc0c-145">datetime</span></span>|<span data-ttu-id="dbc0c-146">Die letzte Uhrzeit, zu der die Währung geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="dbc0c-146">The last datetime the currency was modified.</span></span> <span data-ttu-id="dbc0c-147">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="dbc0c-147">Read-Only.</span></span>       |  


## <a name="relationships"></a><span data-ttu-id="dbc0c-148">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="dbc0c-148">Relationships</span></span>
<span data-ttu-id="dbc0c-149">Keine</span><span class="sxs-lookup"><span data-stu-id="dbc0c-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dbc0c-150">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="dbc0c-150">JSON representation</span></span>

<span data-ttu-id="dbc0c-151">Es folgt eine JSON-Darstellung der Währungen.</span><span class="sxs-lookup"><span data-stu-id="dbc0c-151">Here is a JSON representation of the currencies.</span></span>


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "symbol": "string",
  "amountDecimalPlaces": "string",
  "amountRoundingPrecision": "decimal",
  "lastModifiedDateTime": "datetime"
}

```

