---
title: Ressourcentyp dataPolicyOperation
description: Stellt einen gesendete Daten Richtlinie Vorgang dar. Sie enthält die erforderlichen Informationen für das Nachverfolgen des Status eines Vorgangs. Beispielsweise kann ein Unternehmensadministrator anfordern, Daten Richtlinie Vorgang zum Exportieren eines Mitarbeiters Unternehmensdaten verwendet, und klicken Sie dann die Anforderung später verfolgen.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4547221c8c1b859d4738a5468603ac6890246263
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29570925"
---
# <a name="datapolicyoperation-resource-type"></a><span data-ttu-id="0ddfb-105">Ressourcentyp dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="0ddfb-105">dataPolicyOperation resource type</span></span>

<span data-ttu-id="0ddfb-106">Stellt einen gesendete Daten Richtlinie Vorgang dar.</span><span class="sxs-lookup"><span data-stu-id="0ddfb-106">Represents a submitted data policy operation.</span></span> <span data-ttu-id="0ddfb-107">Sie enthält die erforderlichen Informationen für das Nachverfolgen des Status eines Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="0ddfb-107">It contains necessary information for tracking the status of an operation.</span></span> <span data-ttu-id="0ddfb-108">Beispielsweise kann ein Unternehmensadministrator anfordern, Daten Richtlinie Vorgang zum Exportieren eines Mitarbeiters Unternehmensdaten verwendet, und klicken Sie dann die Anforderung später verfolgen.</span><span class="sxs-lookup"><span data-stu-id="0ddfb-108">For example, a company administrator can submit a data policy operation request to export an employee's company data, and then later track that request.</span></span>

## <a name="methods"></a><span data-ttu-id="0ddfb-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="0ddfb-109">Methods</span></span>

| <span data-ttu-id="0ddfb-110">Methode</span><span class="sxs-lookup"><span data-stu-id="0ddfb-110">Method</span></span>           | <span data-ttu-id="0ddfb-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="0ddfb-111">Return Type</span></span>    |<span data-ttu-id="0ddfb-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0ddfb-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0ddfb-113">Abrufen von dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="0ddfb-113">Get dataPolicyOperation</span></span>](../api/datapolicyoperation-get.md) | [<span data-ttu-id="0ddfb-114">dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="0ddfb-114">dataPolicyOperation</span></span>](datapolicyoperation.md) |<span data-ttu-id="0ddfb-115">Lesen Sie die Eigenschaften des DataPolicyOperation-Objekts.</span><span class="sxs-lookup"><span data-stu-id="0ddfb-115">Read properties of the dataPolicyOperation object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0ddfb-116">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0ddfb-116">Properties</span></span>

> <span data-ttu-id="0ddfb-117">**Hinweis:** Alle Eigenschaften dieser Ressource sind schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="0ddfb-117">**Note:** All properties of this resource are read-only.</span></span>

| <span data-ttu-id="0ddfb-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0ddfb-118">Property</span></span>     | <span data-ttu-id="0ddfb-119">Typ</span><span class="sxs-lookup"><span data-stu-id="0ddfb-119">Type</span></span>   |<span data-ttu-id="0ddfb-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0ddfb-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0ddfb-121">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="0ddfb-121">completedDateTime</span></span>|<span data-ttu-id="0ddfb-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ddfb-122">DateTimeOffset</span></span>|<span data-ttu-id="0ddfb-123">Stellt die bei die Anforderung für diese Richtlinie Datenvorgangs, in UTC-Zeit mit abgeschlossen wurde im ISO 8601-Format.</span><span class="sxs-lookup"><span data-stu-id="0ddfb-123">Represents when the request for this data policy operation was completed, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="0ddfb-124">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="0ddfb-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="0ddfb-125">"NULL", bis der Vorgang abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="0ddfb-125">Null until the operation completes.</span></span>|
|<span data-ttu-id="0ddfb-126">id</span><span class="sxs-lookup"><span data-stu-id="0ddfb-126">id</span></span>|<span data-ttu-id="0ddfb-127">String</span><span class="sxs-lookup"><span data-stu-id="0ddfb-127">String</span></span>| <span data-ttu-id="0ddfb-128">Eindeutiger Schlüssel für diesen Vorgang.</span><span class="sxs-lookup"><span data-stu-id="0ddfb-128">Unique key for this operation.</span></span> |
|<span data-ttu-id="0ddfb-129">status</span><span class="sxs-lookup"><span data-stu-id="0ddfb-129">status</span></span>|<span data-ttu-id="0ddfb-130">string</span><span class="sxs-lookup"><span data-stu-id="0ddfb-130">string</span></span>| <span data-ttu-id="0ddfb-131">Mögliche Werte sind: `notStarted`, `running`, `complete`, `failed` und `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="0ddfb-131">Possible values are: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="0ddfb-132">storageLocation</span><span class="sxs-lookup"><span data-stu-id="0ddfb-132">storageLocation</span></span>|<span data-ttu-id="0ddfb-133">String</span><span class="sxs-lookup"><span data-stu-id="0ddfb-133">String</span></span>|<span data-ttu-id="0ddfb-134">Der URL-Adresse an, in dem Daten für exportanforderungen exportiert werden.</span><span class="sxs-lookup"><span data-stu-id="0ddfb-134">The URL location to where data is being exported for export requests.</span></span>|
|<span data-ttu-id="0ddfb-135">userId</span><span class="sxs-lookup"><span data-stu-id="0ddfb-135">userId</span></span>|<span data-ttu-id="0ddfb-136">String</span><span class="sxs-lookup"><span data-stu-id="0ddfb-136">String</span></span>|<span data-ttu-id="0ddfb-137">Die Id für den Benutzer, auf dem die Operation ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="0ddfb-137">The id for the user on whom the operation is performed.</span></span>|
|<span data-ttu-id="0ddfb-138">submittedDateTime</span><span class="sxs-lookup"><span data-stu-id="0ddfb-138">submittedDateTime</span></span>|<span data-ttu-id="0ddfb-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ddfb-139">DateTimeOffset</span></span>|<span data-ttu-id="0ddfb-140">Stellt die bei die Anforderung für diesen Datenvorgang im ISO 8601-Format verwenden übermittelt wurde, im UTC-Zeit.</span><span class="sxs-lookup"><span data-stu-id="0ddfb-140">Represents when the request for this data operation was submitted, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="0ddfb-141">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="0ddfb-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="0ddfb-142">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0ddfb-142">Relationships</span></span>
<span data-ttu-id="0ddfb-143">Keine</span><span class="sxs-lookup"><span data-stu-id="0ddfb-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="0ddfb-144">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0ddfb-144">JSON representation</span></span>

<span data-ttu-id="0ddfb-145">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0ddfb-145">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.dataPolicyOperation"
}-->

```json
{
  "completedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "status": "string",
  "storageLocation": "String",
  "userId": "String",
  "submittedDateTime": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "dataPolicyOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
