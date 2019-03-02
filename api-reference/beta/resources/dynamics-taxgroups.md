---
title: taxGroups-Ressourcentyp
description: Ein Steuergruppen Objekt in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: bdfbec8f5373637924262388dab0e9c74c363af9
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366690"
---
# <a name="taxgroups-resource-type"></a><span data-ttu-id="bc296-103">taxGroups-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="bc296-103">taxGroups resource type</span></span>
<span data-ttu-id="bc296-104">Stellt einen taxGroups-Ressourcentyp in Dynamics 365 Business Central dar.</span><span class="sxs-lookup"><span data-stu-id="bc296-104">Represents a taxGroups resource type in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="bc296-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="bc296-105">Methods</span></span>
| <span data-ttu-id="bc296-106">Methode</span><span class="sxs-lookup"><span data-stu-id="bc296-106">Method</span></span>       | <span data-ttu-id="bc296-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="bc296-107">Return Type</span></span>  |<span data-ttu-id="bc296-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bc296-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bc296-109">TaxGroups abrufen</span><span class="sxs-lookup"><span data-stu-id="bc296-109">Get taxGroups</span></span>](../api/dynamics-taxgroups-get.md)|<span data-ttu-id="bc296-110">taxGroups</span><span class="sxs-lookup"><span data-stu-id="bc296-110">taxGroups</span></span>|<span data-ttu-id="bc296-111">Ruft ein Steuergruppen Objekt ab.</span><span class="sxs-lookup"><span data-stu-id="bc296-111">Gets a tax group object.</span></span>|
|[<span data-ttu-id="bc296-112">Post taxGroups</span><span class="sxs-lookup"><span data-stu-id="bc296-112">Post taxGroups</span></span>](../api/dynamics-create-taxgroups.md)|<span data-ttu-id="bc296-113">taxGroups</span><span class="sxs-lookup"><span data-stu-id="bc296-113">taxGroups</span></span>|<span data-ttu-id="bc296-114">Erstellt ein Steuergruppen Objekt.</span><span class="sxs-lookup"><span data-stu-id="bc296-114">Creates a tax group object.</span></span>|
|[<span data-ttu-id="bc296-115">Patch-taxGroups</span><span class="sxs-lookup"><span data-stu-id="bc296-115">Patch taxGroups</span></span>](../api/dynamics-taxgroups-update.md)|<span data-ttu-id="bc296-116">taxGroups</span><span class="sxs-lookup"><span data-stu-id="bc296-116">taxGroups</span></span>|<span data-ttu-id="bc296-117">Aktualisiert ein Steuergruppen Objekt.</span><span class="sxs-lookup"><span data-stu-id="bc296-117">Updates a tax group object.</span></span>|
|[<span data-ttu-id="bc296-118">TaxGroups löschen</span><span class="sxs-lookup"><span data-stu-id="bc296-118">Delete taxGroups</span></span>](../api/dynamics-taxgroups-delete.md)|<span data-ttu-id="bc296-119">Keine</span><span class="sxs-lookup"><span data-stu-id="bc296-119">none</span></span>|<span data-ttu-id="bc296-120">Löscht ein Steuergruppen Objekt.</span><span class="sxs-lookup"><span data-stu-id="bc296-120">Deletes a tax group object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bc296-121">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bc296-121">Properties</span></span>
| <span data-ttu-id="bc296-122">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bc296-122">Property</span></span>     | <span data-ttu-id="bc296-123">Typ</span><span class="sxs-lookup"><span data-stu-id="bc296-123">Type</span></span>   |<span data-ttu-id="bc296-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bc296-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bc296-125">id</span><span class="sxs-lookup"><span data-stu-id="bc296-125">id</span></span>|<span data-ttu-id="bc296-126">GUID</span><span class="sxs-lookup"><span data-stu-id="bc296-126">GUID</span></span>|<span data-ttu-id="bc296-127">Die eindeutige ID des taxGroup.</span><span class="sxs-lookup"><span data-stu-id="bc296-127">The unique ID of the taxGroup.</span></span> <span data-ttu-id="bc296-128">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="bc296-128">Read-Only.</span></span>|
|<span data-ttu-id="bc296-129">code</span><span class="sxs-lookup"><span data-stu-id="bc296-129">code</span></span>|<span data-ttu-id="bc296-130">string</span><span class="sxs-lookup"><span data-stu-id="bc296-130">string</span></span>|<span data-ttu-id="bc296-131">Gibt die Steuergruppe an.</span><span class="sxs-lookup"><span data-stu-id="bc296-131">Specifies the tax group.</span></span>|
|<span data-ttu-id="bc296-132">displayName</span><span class="sxs-lookup"><span data-stu-id="bc296-132">displayName</span></span>|<span data-ttu-id="bc296-133">string</span><span class="sxs-lookup"><span data-stu-id="bc296-133">string</span></span>|<span data-ttu-id="bc296-134">Gibt den Anzeigenamen der Steuergruppe an.</span><span class="sxs-lookup"><span data-stu-id="bc296-134">Specifies the tax group display name.</span></span>|
|<span data-ttu-id="bc296-135">taxType</span><span class="sxs-lookup"><span data-stu-id="bc296-135">taxType</span></span>|<span data-ttu-id="bc296-136">string</span><span class="sxs-lookup"><span data-stu-id="bc296-136">string</span></span>|<span data-ttu-id="bc296-137">Gibt den Steuertyp für die Gruppe an.</span><span class="sxs-lookup"><span data-stu-id="bc296-137">Specifies the tax type for the group.</span></span>|
|<span data-ttu-id="bc296-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bc296-138">lastModifiedDateTime</span></span>|<span data-ttu-id="bc296-139">DateTime</span><span class="sxs-lookup"><span data-stu-id="bc296-139">datetime</span></span>|<span data-ttu-id="bc296-140">Die letzte DateTime, die die Steuergruppe geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="bc296-140">The last datetime the tax group was modified.</span></span> <span data-ttu-id="bc296-141">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="bc296-141">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="bc296-142">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="bc296-142">Relationships</span></span>
<span data-ttu-id="bc296-143">Keine</span><span class="sxs-lookup"><span data-stu-id="bc296-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bc296-144">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bc296-144">JSON representation</span></span>

<span data-ttu-id="bc296-145">Es folgt eine JSON-Darstellung des taxGroup.</span><span class="sxs-lookup"><span data-stu-id="bc296-145">Here is a JSON representation of the taxGroup.</span></span>

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "taxType": "string",
  "lastModifiedDateTime": "datetime"
}

```


