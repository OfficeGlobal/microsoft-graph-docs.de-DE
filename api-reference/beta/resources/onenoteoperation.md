---
title: onenoteOperation-Ressourcentyp
description: Der Status bestimmter lange dauernder OneNote-Vorgänge.
author: Jewan-microsoft
localization_priority: Normal
ms.openlocfilehash: 7632186c3e44afbfe0d6cbf3d079ad0758514b38
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860263"
---
# <a name="onenoteoperation-resource-type"></a><span data-ttu-id="88c7a-103">onenoteOperation-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="88c7a-103">onenoteOperation resource type</span></span>

> <span data-ttu-id="88c7a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="88c7a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="88c7a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="88c7a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="88c7a-106">Der Status bestimmter lange dauernder OneNote-Vorgänge.</span><span class="sxs-lookup"><span data-stu-id="88c7a-106">The status of certain long-running OneNote operations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="88c7a-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="88c7a-107">JSON representation</span></span>

<span data-ttu-id="88c7a-108">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="88c7a-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
## <a name="properties"></a><span data-ttu-id="88c7a-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="88c7a-109">Properties</span></span>
| <span data-ttu-id="88c7a-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="88c7a-110">Property</span></span>     | <span data-ttu-id="88c7a-111">Typ</span><span class="sxs-lookup"><span data-stu-id="88c7a-111">Type</span></span>   |<span data-ttu-id="88c7a-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="88c7a-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="88c7a-113">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="88c7a-113">createdDateTime</span></span>| <span data-ttu-id="88c7a-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88c7a-114">DateTimeOffset</span></span> |<span data-ttu-id="88c7a-115">Die Startzeit des Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="88c7a-115">The start time of the operation.</span></span>|
|<span data-ttu-id="88c7a-116">error</span><span class="sxs-lookup"><span data-stu-id="88c7a-116">error</span></span>|[<span data-ttu-id="88c7a-117">onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="88c7a-117">onenoteOperationError</span></span>](onenoteoperationerror.md)|<span data-ttu-id="88c7a-118">Der Fehler, der vom Vorgang zurückgegeben wird.</span><span class="sxs-lookup"><span data-stu-id="88c7a-118">The error returned by the operation.</span></span>|
|<span data-ttu-id="88c7a-119">id</span><span class="sxs-lookup"><span data-stu-id="88c7a-119">id</span></span>|<span data-ttu-id="88c7a-120">string</span><span class="sxs-lookup"><span data-stu-id="88c7a-120">string</span></span>|<span data-ttu-id="88c7a-121">Die Vorgangs-ID. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="88c7a-121">The operation id. Read-only.</span></span>|
|<span data-ttu-id="88c7a-122">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="88c7a-122">lastActionDateTime</span></span>| <span data-ttu-id="88c7a-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88c7a-123">DateTimeOffset</span></span> |<span data-ttu-id="88c7a-124">Der Zeitpunkt der letzten Aktion des Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="88c7a-124">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="88c7a-125">resourceId</span><span class="sxs-lookup"><span data-stu-id="88c7a-125">resourceId</span></span>|<span data-ttu-id="88c7a-126">string</span><span class="sxs-lookup"><span data-stu-id="88c7a-126">string</span></span>|<span data-ttu-id="88c7a-127">Die Ressourcen-ID.</span><span class="sxs-lookup"><span data-stu-id="88c7a-127">The resource id.</span></span>|
|<span data-ttu-id="88c7a-128">resourceLocation</span><span class="sxs-lookup"><span data-stu-id="88c7a-128">resourceLocation</span></span>|<span data-ttu-id="88c7a-129">string</span><span class="sxs-lookup"><span data-stu-id="88c7a-129">string</span></span>|<span data-ttu-id="88c7a-p102">Der Ressourcen-URI für das Objekt. Beispielsweise der Ressource-URI für eine kopierte Seite oder einen kopierten Abschnitt.</span><span class="sxs-lookup"><span data-stu-id="88c7a-p102">The resource URI for the object. For example, the resource URI for a copied page or section.</span></span> |
|<span data-ttu-id="88c7a-132">status</span><span class="sxs-lookup"><span data-stu-id="88c7a-132">status</span></span>|<span data-ttu-id="88c7a-133">string</span><span class="sxs-lookup"><span data-stu-id="88c7a-133">string</span></span>|<span data-ttu-id="88c7a-134">Der aktuellen Status des Vorgangs: `notstarted`, `running`, `completed`, `failed`</span><span class="sxs-lookup"><span data-stu-id="88c7a-134">The current status of the operation: `notstarted`, `running`, `completed`, `failed`</span></span> |
|<span data-ttu-id="88c7a-135">percentComplete</span><span class="sxs-lookup"><span data-stu-id="88c7a-135">percentComplete</span></span>|<span data-ttu-id="88c7a-136">string</span><span class="sxs-lookup"><span data-stu-id="88c7a-136">string</span></span>|<span data-ttu-id="88c7a-137">Der abgeschlossene Prozentsatz des Vorgangs, sofern der Vorgang noch den Status `running` hat.</span><span class="sxs-lookup"><span data-stu-id="88c7a-137">The operation percent complete if the operation is still in `running` status</span></span>

## <a name="relationships"></a><span data-ttu-id="88c7a-138">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="88c7a-138">Relationships</span></span>
<span data-ttu-id="88c7a-139">Keine</span><span class="sxs-lookup"><span data-stu-id="88c7a-139">None</span></span>


## <a name="methods"></a><span data-ttu-id="88c7a-140">Methoden</span><span class="sxs-lookup"><span data-stu-id="88c7a-140">Methods</span></span>

| <span data-ttu-id="88c7a-141">Methode</span><span class="sxs-lookup"><span data-stu-id="88c7a-141">Method</span></span>           | <span data-ttu-id="88c7a-142">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="88c7a-142">Return Type</span></span>    |<span data-ttu-id="88c7a-143">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="88c7a-143">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="88c7a-144">Vorgang abrufen</span><span class="sxs-lookup"><span data-stu-id="88c7a-144">Get operation</span></span>](../api/onenoteoperation-get.md) | [<span data-ttu-id="88c7a-145">onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="88c7a-145">onenoteOperation</span></span>](onenoteoperation.md) |<span data-ttu-id="88c7a-146">Dient zum Abrufen des Status des Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="88c7a-146">Get the status of the operation.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
