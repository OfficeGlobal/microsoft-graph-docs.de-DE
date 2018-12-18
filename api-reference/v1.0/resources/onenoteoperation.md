---
title: onenoteOperation-Ressourcentyp
description: Der Status bestimmter lange dauernder OneNote-Vorgänge.
author: Jewan-microsoft
ms.openlocfilehash: bbb7b9457ce5a3d7ba9faf45d893ae86cdfd8b32
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326908"
---
# <a name="onenoteoperation-resource-type"></a><span data-ttu-id="79d6b-103">onenoteOperation-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="79d6b-103">onenoteOperation resource type</span></span>

<span data-ttu-id="79d6b-104">Der Status bestimmter lange dauernder OneNote-Vorgänge.</span><span class="sxs-lookup"><span data-stu-id="79d6b-104">The status of certain long-running OneNote operations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="79d6b-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="79d6b-105">JSON representation</span></span>

<span data-ttu-id="79d6b-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="79d6b-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="79d6b-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="79d6b-107">Properties</span></span>
| <span data-ttu-id="79d6b-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="79d6b-108">Property</span></span>     | <span data-ttu-id="79d6b-109">Typ</span><span class="sxs-lookup"><span data-stu-id="79d6b-109">Type</span></span>   |<span data-ttu-id="79d6b-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="79d6b-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="79d6b-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="79d6b-111">createdDateTime</span></span>| <span data-ttu-id="79d6b-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79d6b-112">DateTimeOffset</span></span> |<span data-ttu-id="79d6b-113">Die Startzeit des Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="79d6b-113">The start time of the operation.</span></span>|
|<span data-ttu-id="79d6b-114">error</span><span class="sxs-lookup"><span data-stu-id="79d6b-114">error</span></span>|[<span data-ttu-id="79d6b-115">onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="79d6b-115">onenoteOperationError</span></span>](onenoteoperationerror.md)|<span data-ttu-id="79d6b-116">Der Fehler, der vom Vorgang zurückgegeben wird.</span><span class="sxs-lookup"><span data-stu-id="79d6b-116">The error returned by the operation.</span></span>|
|<span data-ttu-id="79d6b-117">id</span><span class="sxs-lookup"><span data-stu-id="79d6b-117">id</span></span>|<span data-ttu-id="79d6b-118">string</span><span class="sxs-lookup"><span data-stu-id="79d6b-118">string</span></span>|<span data-ttu-id="79d6b-119">Die Vorgangs-ID. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="79d6b-119">The operation id. Read-only.</span></span>|
|<span data-ttu-id="79d6b-120">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="79d6b-120">lastActionDateTime</span></span>| <span data-ttu-id="79d6b-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79d6b-121">DateTimeOffset</span></span> |<span data-ttu-id="79d6b-122">Der Zeitpunkt der letzten Aktion des Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="79d6b-122">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="79d6b-123">resourceId</span><span class="sxs-lookup"><span data-stu-id="79d6b-123">resourceId</span></span>|<span data-ttu-id="79d6b-124">string</span><span class="sxs-lookup"><span data-stu-id="79d6b-124">string</span></span>|<span data-ttu-id="79d6b-125">Die Ressourcen-ID.</span><span class="sxs-lookup"><span data-stu-id="79d6b-125">The resource id.</span></span>|
|<span data-ttu-id="79d6b-126">resourceLocation</span><span class="sxs-lookup"><span data-stu-id="79d6b-126">resourceLocation</span></span>|<span data-ttu-id="79d6b-127">string</span><span class="sxs-lookup"><span data-stu-id="79d6b-127">string</span></span>|<span data-ttu-id="79d6b-p101">Der Ressourcen-URI für das Objekt. Beispielsweise der Ressource-URI für eine kopierte Seite oder einen kopierten Abschnitt.</span><span class="sxs-lookup"><span data-stu-id="79d6b-p101">The resource URI for the object. For example, the resource URI for a copied page or section.</span></span> |
|<span data-ttu-id="79d6b-130">status</span><span class="sxs-lookup"><span data-stu-id="79d6b-130">status</span></span>|<span data-ttu-id="79d6b-131">string</span><span class="sxs-lookup"><span data-stu-id="79d6b-131">string</span></span>|<span data-ttu-id="79d6b-132">Der aktuellen Status des Vorgangs: `notstarted`, `running`, `completed`, `failed`</span><span class="sxs-lookup"><span data-stu-id="79d6b-132">The current status of the operation: `notstarted`, `running`, `completed`, `failed`</span></span> |
|<span data-ttu-id="79d6b-133">percentComplete</span><span class="sxs-lookup"><span data-stu-id="79d6b-133">percentComplete</span></span>|<span data-ttu-id="79d6b-134">string</span><span class="sxs-lookup"><span data-stu-id="79d6b-134">string</span></span>|<span data-ttu-id="79d6b-135">Der abgeschlossene Prozentsatz des Vorgangs, sofern der Vorgang noch den Status `running` hat.</span><span class="sxs-lookup"><span data-stu-id="79d6b-135">The operation percent complete if the operation is still in `running` status</span></span>

## <a name="relationships"></a><span data-ttu-id="79d6b-136">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="79d6b-136">Relationships</span></span>
<span data-ttu-id="79d6b-137">Keine</span><span class="sxs-lookup"><span data-stu-id="79d6b-137">None</span></span>


## <a name="methods"></a><span data-ttu-id="79d6b-138">Methoden</span><span class="sxs-lookup"><span data-stu-id="79d6b-138">Methods</span></span>

| <span data-ttu-id="79d6b-139">Methode</span><span class="sxs-lookup"><span data-stu-id="79d6b-139">Method</span></span>           | <span data-ttu-id="79d6b-140">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="79d6b-140">Return Type</span></span>    |<span data-ttu-id="79d6b-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="79d6b-141">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="79d6b-142">Vorgang abrufen</span><span class="sxs-lookup"><span data-stu-id="79d6b-142">Get operation</span></span>](../api/onenoteoperation-get.md) | [<span data-ttu-id="79d6b-143">onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="79d6b-143">onenoteOperation</span></span>](onenoteoperation.md) |<span data-ttu-id="79d6b-144">Dient zum Abrufen des Status des Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="79d6b-144">Get the status of the operation.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
