---
title: Journal-Ressourcentyp
description: Ein Journal in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: bef5008bbacb1729f48758b228e55a3f6adc2af0
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365472"
---
# <a name="journal-resource-type"></a><span data-ttu-id="70d90-103">Journal-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="70d90-103">journal resource type</span></span>
<span data-ttu-id="70d90-104">Stellt ein Journal in Dynamics 365 Business Central dar.</span><span class="sxs-lookup"><span data-stu-id="70d90-104">Represents a journal in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="70d90-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="70d90-105">Methods</span></span>

| <span data-ttu-id="70d90-106">Methode</span><span class="sxs-lookup"><span data-stu-id="70d90-106">Method</span></span>                                            |<span data-ttu-id="70d90-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="70d90-107">Return Type</span></span>|<span data-ttu-id="70d90-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="70d90-108">Description</span></span>    |
|:--------------------------------------------------|:----------|:--------------|
|[<span data-ttu-id="70d90-109">Journal abrufen</span><span class="sxs-lookup"><span data-stu-id="70d90-109">Get journal</span></span>](../api/dynamics-journal-get.md)      |<span data-ttu-id="70d90-110">Journal</span><span class="sxs-lookup"><span data-stu-id="70d90-110">journal</span></span>    |<span data-ttu-id="70d90-111">Ruft ein Journal ab.</span><span class="sxs-lookup"><span data-stu-id="70d90-111">Gets a journal.</span></span>   |
|[<span data-ttu-id="70d90-112">Post Journal</span><span class="sxs-lookup"><span data-stu-id="70d90-112">Post journal</span></span>](../api/dynamics-create-journal.md)  |<span data-ttu-id="70d90-113">Journal</span><span class="sxs-lookup"><span data-stu-id="70d90-113">journal</span></span>    |<span data-ttu-id="70d90-114">Erstellt ein Journal.</span><span class="sxs-lookup"><span data-stu-id="70d90-114">Creates a journal.</span></span>|
|[<span data-ttu-id="70d90-115">Patch-Journal</span><span class="sxs-lookup"><span data-stu-id="70d90-115">Patch journal</span></span>](../api/dynamics-journal-update.md) |<span data-ttu-id="70d90-116">Journal</span><span class="sxs-lookup"><span data-stu-id="70d90-116">journal</span></span>    |<span data-ttu-id="70d90-117">Aktualisiert ein Journal.</span><span class="sxs-lookup"><span data-stu-id="70d90-117">Updates a journal.</span></span>|
|[<span data-ttu-id="70d90-118">Journal löschen</span><span class="sxs-lookup"><span data-stu-id="70d90-118">Delete journal</span></span>](../api/dynamics-journal-delete.md)|<span data-ttu-id="70d90-119">Keine</span><span class="sxs-lookup"><span data-stu-id="70d90-119">none</span></span>       |<span data-ttu-id="70d90-120">Löscht ein Journal.</span><span class="sxs-lookup"><span data-stu-id="70d90-120">Deletes a journal.</span></span>|

## <a name="properties"></a><span data-ttu-id="70d90-121">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="70d90-121">Properties</span></span>
| <span data-ttu-id="70d90-122">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="70d90-122">Property</span></span>           | <span data-ttu-id="70d90-123">Typ</span><span class="sxs-lookup"><span data-stu-id="70d90-123">Type</span></span>                  |<span data-ttu-id="70d90-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="70d90-124">Description</span></span>                                           |
|:-------------------|:----------------------|:-----------------------------------------------------|
|<span data-ttu-id="70d90-125">id</span><span class="sxs-lookup"><span data-stu-id="70d90-125">id</span></span>                  |<span data-ttu-id="70d90-126">GUID</span><span class="sxs-lookup"><span data-stu-id="70d90-126">GUID</span></span>                   |<span data-ttu-id="70d90-127">Die eindeutige ID des Journals.</span><span class="sxs-lookup"><span data-stu-id="70d90-127">The unique ID of the journal.</span></span> <span data-ttu-id="70d90-128">Nicht bearbeitbar.</span><span class="sxs-lookup"><span data-stu-id="70d90-128">Non-editable.</span></span>           |
|<span data-ttu-id="70d90-129">code</span><span class="sxs-lookup"><span data-stu-id="70d90-129">code</span></span>                |<span data-ttu-id="70d90-130">Zeichenfolge, maximale Größe 10</span><span class="sxs-lookup"><span data-stu-id="70d90-130">string, maximum size 10</span></span>| <span data-ttu-id="70d90-131">Der Code des Journals.</span><span class="sxs-lookup"><span data-stu-id="70d90-131">The code of the journal.</span></span>                             |
|<span data-ttu-id="70d90-132">displayName</span><span class="sxs-lookup"><span data-stu-id="70d90-132">displayName</span></span>         |<span data-ttu-id="70d90-133">Zeichenfolge, maximale Größe 50</span><span class="sxs-lookup"><span data-stu-id="70d90-133">string, maximum size 50</span></span>| <span data-ttu-id="70d90-134">Der Anzeigename des Journals.</span><span class="sxs-lookup"><span data-stu-id="70d90-134">The display name of the journal.</span></span>                     |
|<span data-ttu-id="70d90-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="70d90-135">lastModifiedDateTime</span></span>|<span data-ttu-id="70d90-136">DateTime</span><span class="sxs-lookup"><span data-stu-id="70d90-136">datetime</span></span>               |<span data-ttu-id="70d90-137">Die letzte DateTime, die das Journal geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="70d90-137">The last datetime the journal was modified.</span></span> <span data-ttu-id="70d90-138">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="70d90-138">Read-Only.</span></span>|

## <a name="bound-actions"></a><span data-ttu-id="70d90-139">Gebundene Aktionen</span><span class="sxs-lookup"><span data-stu-id="70d90-139">Bound actions</span></span>
<span data-ttu-id="70d90-140">Der Ressourcentyp Journal bietet eine gebundene Aktion `post` , die den entsprechenden allgemeinen Journal Batch bereitstellt.</span><span class="sxs-lookup"><span data-stu-id="70d90-140">The journal resource type offers a bound action called `post` which posts the corresponding general journal batch.</span></span>

<span data-ttu-id="70d90-141">Die Buchung des Fibu Buch.-Blatts wird im folgenden Beispiel veranschaulicht:</span><span class="sxs-lookup"><span data-stu-id="70d90-141">Posting the general journal batch is illustrated in the following example:</span></span>  
<span data-ttu-id="70d90-142">`POST https://graph.microsoft.com/beta/financials/companies{id}/journals{id}/post`.</span><span class="sxs-lookup"><span data-stu-id="70d90-142"></span></span>

<span data-ttu-id="70d90-143">Die Antwort hat keinen Inhalt; der Antwortcode lautet 204.</span><span class="sxs-lookup"><span data-stu-id="70d90-143">The response has no content; the response code is 204.</span></span>

## <a name="json-representation"></a><span data-ttu-id="70d90-144">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="70d90-144">JSON representation</span></span>

<span data-ttu-id="70d90-145">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="70d90-145">Here is a JSON representation of the resource.</span></span>


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}
```

