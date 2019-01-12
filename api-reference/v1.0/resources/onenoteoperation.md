---
title: onenoteOperation-Ressourcentyp
description: Der Status bestimmter lange dauernder OneNote-Vorgänge.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: eaab313e9399e6e8724d5096b7ac29ec315889ad
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977465"
---
# <a name="onenoteoperation-resource-type"></a><span data-ttu-id="1deff-103">onenoteOperation-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="1deff-103">onenoteOperation resource type</span></span>

<span data-ttu-id="1deff-104">Der Status bestimmter lange dauernder OneNote-Vorgänge.</span><span class="sxs-lookup"><span data-stu-id="1deff-104">The status of certain long-running OneNote operations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1deff-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1deff-105">JSON representation</span></span>

<span data-ttu-id="1deff-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1deff-106">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.operation",
  "@odata.type": "microsoft.graph.onenoteOperation"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "error": {"@odata.type": "microsoft.graph.onenoteOperationError"},
  "id": "string (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "resourceId": "string",
  "resourceLocation": "string",
  "status": "string",
  "percentComplete": "string"
}

```
## <a name="properties"></a><span data-ttu-id="1deff-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1deff-107">Properties</span></span>
| <span data-ttu-id="1deff-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1deff-108">Property</span></span>     | <span data-ttu-id="1deff-109">Typ</span><span class="sxs-lookup"><span data-stu-id="1deff-109">Type</span></span>   |<span data-ttu-id="1deff-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1deff-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1deff-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1deff-111">createdDateTime</span></span>| <span data-ttu-id="1deff-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1deff-112">DateTimeOffset</span></span> |<span data-ttu-id="1deff-113">Die Startzeit des Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="1deff-113">The start time of the operation.</span></span>|
|<span data-ttu-id="1deff-114">error</span><span class="sxs-lookup"><span data-stu-id="1deff-114">error</span></span>|[<span data-ttu-id="1deff-115">onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="1deff-115">onenoteOperationError</span></span>](onenoteoperationerror.md)|<span data-ttu-id="1deff-116">Der Fehler, der vom Vorgang zurückgegeben wird.</span><span class="sxs-lookup"><span data-stu-id="1deff-116">The error returned by the operation.</span></span>|
|<span data-ttu-id="1deff-117">id</span><span class="sxs-lookup"><span data-stu-id="1deff-117">id</span></span>|<span data-ttu-id="1deff-118">string</span><span class="sxs-lookup"><span data-stu-id="1deff-118">string</span></span>|<span data-ttu-id="1deff-119">Die Vorgangs-ID. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="1deff-119">The operation id. Read-only.</span></span>|
|<span data-ttu-id="1deff-120">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="1deff-120">lastActionDateTime</span></span>| <span data-ttu-id="1deff-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1deff-121">DateTimeOffset</span></span> |<span data-ttu-id="1deff-122">Der Zeitpunkt der letzten Aktion des Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="1deff-122">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="1deff-123">resourceId</span><span class="sxs-lookup"><span data-stu-id="1deff-123">resourceId</span></span>|<span data-ttu-id="1deff-124">string</span><span class="sxs-lookup"><span data-stu-id="1deff-124">string</span></span>|<span data-ttu-id="1deff-125">Die Ressourcen-ID.</span><span class="sxs-lookup"><span data-stu-id="1deff-125">The resource id.</span></span>|
|<span data-ttu-id="1deff-126">resourceLocation</span><span class="sxs-lookup"><span data-stu-id="1deff-126">resourceLocation</span></span>|<span data-ttu-id="1deff-127">string</span><span class="sxs-lookup"><span data-stu-id="1deff-127">string</span></span>|<span data-ttu-id="1deff-p101">Der Ressourcen-URI für das Objekt. Beispielsweise der Ressource-URI für eine kopierte Seite oder einen kopierten Abschnitt.</span><span class="sxs-lookup"><span data-stu-id="1deff-p101">The resource URI for the object. For example, the resource URI for a copied page or section.</span></span> |
|<span data-ttu-id="1deff-130">status</span><span class="sxs-lookup"><span data-stu-id="1deff-130">status</span></span>|<span data-ttu-id="1deff-131">string</span><span class="sxs-lookup"><span data-stu-id="1deff-131">string</span></span>|<span data-ttu-id="1deff-132">Der aktuellen Status des Vorgangs: `notstarted`, `running`, `completed`, `failed`</span><span class="sxs-lookup"><span data-stu-id="1deff-132">The current status of the operation: `notstarted`, `running`, `completed`, `failed`</span></span> |
|<span data-ttu-id="1deff-133">percentComplete</span><span class="sxs-lookup"><span data-stu-id="1deff-133">percentComplete</span></span>|<span data-ttu-id="1deff-134">string</span><span class="sxs-lookup"><span data-stu-id="1deff-134">string</span></span>|<span data-ttu-id="1deff-135">Der abgeschlossene Prozentsatz des Vorgangs, sofern der Vorgang noch den Status `running` hat.</span><span class="sxs-lookup"><span data-stu-id="1deff-135">The operation percent complete if the operation is still in `running` status</span></span>

## <a name="relationships"></a><span data-ttu-id="1deff-136">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="1deff-136">Relationships</span></span>
<span data-ttu-id="1deff-137">Keine</span><span class="sxs-lookup"><span data-stu-id="1deff-137">None</span></span>


## <a name="methods"></a><span data-ttu-id="1deff-138">Methoden</span><span class="sxs-lookup"><span data-stu-id="1deff-138">Methods</span></span>

| <span data-ttu-id="1deff-139">Methode</span><span class="sxs-lookup"><span data-stu-id="1deff-139">Method</span></span>           | <span data-ttu-id="1deff-140">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="1deff-140">Return Type</span></span>    |<span data-ttu-id="1deff-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1deff-141">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1deff-142">Vorgang abrufen</span><span class="sxs-lookup"><span data-stu-id="1deff-142">Get operation</span></span>](../api/onenoteoperation-get.md) | [<span data-ttu-id="1deff-143">onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="1deff-143">onenoteOperation</span></span>](onenoteoperation.md) |<span data-ttu-id="1deff-144">Dient zum Abrufen des Status des Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="1deff-144">Get the status of the operation.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
