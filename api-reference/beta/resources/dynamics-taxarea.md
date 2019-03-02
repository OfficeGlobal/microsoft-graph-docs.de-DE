---
title: taxAreas-Ressourcentyp
description: Ein Steuerbereich.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: aeda0ca136c178355a8a8f9589eb7410399ef62a
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365451"
---
# <a name="taxareas-resource-type"></a><span data-ttu-id="c819d-103">taxAreas-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c819d-103">taxAreas resource type</span></span>
<span data-ttu-id="c819d-104">Stellt einen Ressourcentyp für Steuerbereiche in Dynamics 365 Business Central dar.</span><span class="sxs-lookup"><span data-stu-id="c819d-104">Represents a tax area resource type in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="c819d-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="c819d-105">Methods</span></span>
| <span data-ttu-id="c819d-106">Methode</span><span class="sxs-lookup"><span data-stu-id="c819d-106">Method</span></span>       | <span data-ttu-id="c819d-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="c819d-107">Return Type</span></span>  |<span data-ttu-id="c819d-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c819d-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c819d-109">TaxAreas abrufen</span><span class="sxs-lookup"><span data-stu-id="c819d-109">Get taxAreas</span></span>](../api/dynamics-taxarea-get.md)|<span data-ttu-id="c819d-110">taxAreas</span><span class="sxs-lookup"><span data-stu-id="c819d-110">taxAreas</span></span>|<span data-ttu-id="c819d-111">Ruft ein Steuerbereichs Objekt ab.</span><span class="sxs-lookup"><span data-stu-id="c819d-111">Gets a tax area object.</span></span>|
|[<span data-ttu-id="c819d-112">Post taxAreas</span><span class="sxs-lookup"><span data-stu-id="c819d-112">Post taxAreas</span></span>](../api/dynamics-create-taxarea.md)|<span data-ttu-id="c819d-113">taxAreas</span><span class="sxs-lookup"><span data-stu-id="c819d-113">taxAreas</span></span>|<span data-ttu-id="c819d-114">Erstellt ein Steuerbereich-Objekt.</span><span class="sxs-lookup"><span data-stu-id="c819d-114">Creates a tax area object.</span></span>|
|[<span data-ttu-id="c819d-115">Patch-taxAreas</span><span class="sxs-lookup"><span data-stu-id="c819d-115">Patch taxAreas</span></span>](../api/dynamics-taxarea-update.md)|<span data-ttu-id="c819d-116">taxAreas</span><span class="sxs-lookup"><span data-stu-id="c819d-116">taxAreas</span></span>|<span data-ttu-id="c819d-117">Aktualisiert ein Steuerbereichs Objekt.</span><span class="sxs-lookup"><span data-stu-id="c819d-117">Updates a tax area object.</span></span>|
|[<span data-ttu-id="c819d-118">TaxAreas löschen</span><span class="sxs-lookup"><span data-stu-id="c819d-118">Delete taxAreas</span></span>](../api/dynamics-taxarea-delete.md)|<span data-ttu-id="c819d-119">Keine</span><span class="sxs-lookup"><span data-stu-id="c819d-119">none</span></span>|<span data-ttu-id="c819d-120">Löscht ein Steuerbereichs Objekt.</span><span class="sxs-lookup"><span data-stu-id="c819d-120">Deletes a tax area object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c819d-121">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c819d-121">Properties</span></span>
| <span data-ttu-id="c819d-122">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c819d-122">Property</span></span>     | <span data-ttu-id="c819d-123">Typ</span><span class="sxs-lookup"><span data-stu-id="c819d-123">Type</span></span>   |<span data-ttu-id="c819d-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c819d-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c819d-125">id</span><span class="sxs-lookup"><span data-stu-id="c819d-125">id</span></span>|<span data-ttu-id="c819d-126">GUID</span><span class="sxs-lookup"><span data-stu-id="c819d-126">GUID</span></span>|<span data-ttu-id="c819d-127">Die eindeutige ID des Steuerbereichs.</span><span class="sxs-lookup"><span data-stu-id="c819d-127">The unique ID of the tax area.</span></span> <span data-ttu-id="c819d-128">Nicht bearbeitbar.</span><span class="sxs-lookup"><span data-stu-id="c819d-128">Non-editable.</span></span>|
|<span data-ttu-id="c819d-129">code</span><span class="sxs-lookup"><span data-stu-id="c819d-129">code</span></span>|<span data-ttu-id="c819d-130">Zeichenfolge, maximale Größe 20</span><span class="sxs-lookup"><span data-stu-id="c819d-130">string, maximum size 20</span></span>| <span data-ttu-id="c819d-131">Der Code des Steuerbereichs.</span><span class="sxs-lookup"><span data-stu-id="c819d-131">The code of the tax area.</span></span>|
|<span data-ttu-id="c819d-132">displayName</span><span class="sxs-lookup"><span data-stu-id="c819d-132">displayName</span></span>|<span data-ttu-id="c819d-133">Zeichenfolge, maximale Größe 50</span><span class="sxs-lookup"><span data-stu-id="c819d-133">string, maximum size 50</span></span>| <span data-ttu-id="c819d-134">Der Anzeigename des Steuerbereichs.</span><span class="sxs-lookup"><span data-stu-id="c819d-134">The display name of the tax area.</span></span>|
|<span data-ttu-id="c819d-135">taxType</span><span class="sxs-lookup"><span data-stu-id="c819d-135">taxType</span></span>|<span data-ttu-id="c819d-136">string</span><span class="sxs-lookup"><span data-stu-id="c819d-136">string</span></span>|<span data-ttu-id="c819d-137">Der Steuertyp des Steuerbereichs.</span><span class="sxs-lookup"><span data-stu-id="c819d-137">The tax type of the tax area.</span></span>|
|<span data-ttu-id="c819d-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c819d-138">lastModifiedDateTime</span></span>|<span data-ttu-id="c819d-139">DateTime</span><span class="sxs-lookup"><span data-stu-id="c819d-139">datetime</span></span>|<span data-ttu-id="c819d-140">Der letzte DateTime-Steuerbereich wurde geändert.</span><span class="sxs-lookup"><span data-stu-id="c819d-140">The last datetime the tax area was modified.</span></span> <span data-ttu-id="c819d-141">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c819d-141">Read-Only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c819d-142">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c819d-142">Relationships</span></span>

## <a name="json-representation"></a><span data-ttu-id="c819d-143">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c819d-143">JSON representation</span></span>

<span data-ttu-id="c819d-144">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c819d-144">Here is a JSON representation of the resource.</span></span>


```json
{
  "id": "GUID",
  "code": "String",
  "displayName": "String",
  "taxType": "String",
  "lastModifiedDateTime": "datetime"
}
```


