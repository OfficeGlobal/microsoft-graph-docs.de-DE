---
title: Ressourcentyp "Accounts"
description: Ein Account-Objekt in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 4252c20e9d11f67a6de40871b1649a165cbd787c
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365458"
---
# <a name="accounts-resource-type"></a><span data-ttu-id="f6d4c-103">Ressourcentyp "Accounts"</span><span class="sxs-lookup"><span data-stu-id="f6d4c-103">accounts resource type</span></span>
<span data-ttu-id="f6d4c-104">Stellt ein Account-Objekt in Dynamics 365 Business Central dar.</span><span class="sxs-lookup"><span data-stu-id="f6d4c-104">Represents an account object in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="f6d4c-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="f6d4c-105">Methods</span></span>

| <span data-ttu-id="f6d4c-106">Methode</span><span class="sxs-lookup"><span data-stu-id="f6d4c-106">Method</span></span>       | <span data-ttu-id="f6d4c-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="f6d4c-107">Return Type</span></span>  |<span data-ttu-id="f6d4c-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f6d4c-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f6d4c-109">Konten abrufen</span><span class="sxs-lookup"><span data-stu-id="f6d4c-109">Get accounts</span></span>](../api/dynamics-account-get.md)|<span data-ttu-id="f6d4c-110">Konten</span><span class="sxs-lookup"><span data-stu-id="f6d4c-110">accounts</span></span>|<span data-ttu-id="f6d4c-111">Get Accounts-Objekt.</span><span class="sxs-lookup"><span data-stu-id="f6d4c-111">Get accounts object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f6d4c-112">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f6d4c-112">Properties</span></span>
| <span data-ttu-id="f6d4c-113">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f6d4c-113">Property</span></span>     | <span data-ttu-id="f6d4c-114">Typ</span><span class="sxs-lookup"><span data-stu-id="f6d4c-114">Type</span></span>   |<span data-ttu-id="f6d4c-115">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f6d4c-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f6d4c-116">id</span><span class="sxs-lookup"><span data-stu-id="f6d4c-116">id</span></span>|<span data-ttu-id="f6d4c-117">GUID</span><span class="sxs-lookup"><span data-stu-id="f6d4c-117">GUID</span></span>|<span data-ttu-id="f6d4c-118">Die eindeutige ID des Kontos.</span><span class="sxs-lookup"><span data-stu-id="f6d4c-118">The unique ID of the account.</span></span>|
|<span data-ttu-id="f6d4c-119">number</span><span class="sxs-lookup"><span data-stu-id="f6d4c-119">number</span></span>|<span data-ttu-id="f6d4c-120">Zeichenfolge, maximale Größe 20</span><span class="sxs-lookup"><span data-stu-id="f6d4c-120">string, maximum size 20</span></span>|<span data-ttu-id="f6d4c-121">Gibt die Nummer des Sachkontos an.</span><span class="sxs-lookup"><span data-stu-id="f6d4c-121">Specifies the number of the G/L account.</span></span>|
|<span data-ttu-id="f6d4c-122">displayName</span><span class="sxs-lookup"><span data-stu-id="f6d4c-122">displayName</span></span>|<span data-ttu-id="f6d4c-123">Zeichenfolge, maximale Größe 50</span><span class="sxs-lookup"><span data-stu-id="f6d4c-123">string, maximum size 50</span></span>|<span data-ttu-id="f6d4c-124">Gibt den Namen des Sachkontos an.</span><span class="sxs-lookup"><span data-stu-id="f6d4c-124">Specifies the name of the G/L account.</span></span>|
|<span data-ttu-id="f6d4c-125">category</span><span class="sxs-lookup"><span data-stu-id="f6d4c-125">category</span></span>|<span data-ttu-id="f6d4c-126">Zeichenfolge, maximale Größe 20</span><span class="sxs-lookup"><span data-stu-id="f6d4c-126">string, maximum size 20</span></span>|<span data-ttu-id="f6d4c-127">Gibt die Kategorie des Sachkontos an.</span><span class="sxs-lookup"><span data-stu-id="f6d4c-127">Specifies the category of the G/L account.</span></span>|
|<span data-ttu-id="f6d4c-128">subCategory</span><span class="sxs-lookup"><span data-stu-id="f6d4c-128">subCategory</span></span>|<span data-ttu-id="f6d4c-129">Zeichenfolge, maximale Größe 80</span><span class="sxs-lookup"><span data-stu-id="f6d4c-129">string, maximum size 80</span></span>|<span data-ttu-id="f6d4c-130">Gibt die Unterkategorie der Kontokategorie des Sachkontos an.</span><span class="sxs-lookup"><span data-stu-id="f6d4c-130">Specifies the subcategory of the account category of the G/L account.</span></span>|
|<span data-ttu-id="f6d4c-131">gesperrt</span><span class="sxs-lookup"><span data-stu-id="f6d4c-131">blocked</span></span>|<span data-ttu-id="f6d4c-132">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f6d4c-132">boolean</span></span>|<span data-ttu-id="f6d4c-133">Gibt an, dass Posten nicht in das Sachkonto gebucht werden können.</span><span class="sxs-lookup"><span data-stu-id="f6d4c-133">Specifies that entries cannot be posted to the G/L account.</span></span> <span data-ttu-id="f6d4c-134">**True** gibt an, dass das Konto gesperrt ist und das Veröffentlichen nicht zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="f6d4c-134">**True** indicates account is blocked and posting is not allowed.</span></span>|
|<span data-ttu-id="f6d4c-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f6d4c-135">lastModifiedDateTime</span></span>|<span data-ttu-id="f6d4c-136">DateTime</span><span class="sxs-lookup"><span data-stu-id="f6d4c-136">datetime</span></span>|<span data-ttu-id="f6d4c-137">Die letzte Uhrzeit, zu der das Konto geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="f6d4c-137">The last datetime the account was modified.</span></span>|


## <a name="relationships"></a><span data-ttu-id="f6d4c-138">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f6d4c-138">Relationships</span></span>
<span data-ttu-id="f6d4c-139">Keine</span><span class="sxs-lookup"><span data-stu-id="f6d4c-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f6d4c-140">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f6d4c-140">JSON representation</span></span>

<span data-ttu-id="f6d4c-141">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f6d4c-141">Here is a JSON representation of the resource.</span></span>


```json
{
  "id": "GUID",
  "number": "string",
  "displayName": "string",
  "category": "string",
  "subCategory": "string",
  "blocked": "boolean",
  "lastModifiedDateTime": "datetime"
}

```
