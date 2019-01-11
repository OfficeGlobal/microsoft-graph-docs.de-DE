---
title: Ressourcentyp dataPolicyOperation
description: Stellt einen gesendete Daten Richtlinie Vorgang dar. Sie enthält die erforderlichen Informationen für das Nachverfolgen des Status eines Vorgangs. Beispielsweise kann ein Unternehmensadministrator anfordern, Daten Richtlinie Vorgang zum Exportieren eines Mitarbeiters Unternehmensdaten verwendet, und klicken Sie dann die Anforderung später verfolgen.
localization_priority: Normal
ms.openlocfilehash: b56cfe766bbfcae9339805dd61ce816e372d02f4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876006"
---
# <a name="datapolicyoperation-resource-type"></a><span data-ttu-id="9e38a-105">Ressourcentyp dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="9e38a-105">dataPolicyOperation resource type</span></span>

<span data-ttu-id="9e38a-106">Stellt einen gesendete Daten Richtlinie Vorgang dar.</span><span class="sxs-lookup"><span data-stu-id="9e38a-106">Represents a submitted data policy operation.</span></span> <span data-ttu-id="9e38a-107">Sie enthält die erforderlichen Informationen für das Nachverfolgen des Status eines Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="9e38a-107">It contains necessary information for tracking the status of an operation.</span></span> <span data-ttu-id="9e38a-108">Beispielsweise kann ein Unternehmensadministrator anfordern, Daten Richtlinie Vorgang zum Exportieren eines Mitarbeiters Unternehmensdaten verwendet, und klicken Sie dann die Anforderung später verfolgen.</span><span class="sxs-lookup"><span data-stu-id="9e38a-108">For example, a company administrator can submit a data policy operation request to export an employee's company data, and then later track that request.</span></span>

## <a name="methods"></a><span data-ttu-id="9e38a-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="9e38a-109">Methods</span></span>

| <span data-ttu-id="9e38a-110">Methode</span><span class="sxs-lookup"><span data-stu-id="9e38a-110">Method</span></span>           | <span data-ttu-id="9e38a-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="9e38a-111">Return Type</span></span>    |<span data-ttu-id="9e38a-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9e38a-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9e38a-113">Abrufen von dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="9e38a-113">Get dataPolicyOperation</span></span>](../api/datapolicyoperation-get.md) | [<span data-ttu-id="9e38a-114">dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="9e38a-114">dataPolicyOperation</span></span>](datapolicyoperation.md) |<span data-ttu-id="9e38a-115">Lesen Sie die Eigenschaften des DataPolicyOperation-Objekts.</span><span class="sxs-lookup"><span data-stu-id="9e38a-115">Read properties of the dataPolicyOperation object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9e38a-116">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9e38a-116">Properties</span></span>

> <span data-ttu-id="9e38a-117">**Hinweis:** Alle Eigenschaften dieser Ressource sind schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9e38a-117">**Note:** All properties of this resource are read-only.</span></span>

| <span data-ttu-id="9e38a-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9e38a-118">Property</span></span>     | <span data-ttu-id="9e38a-119">Typ</span><span class="sxs-lookup"><span data-stu-id="9e38a-119">Type</span></span>   |<span data-ttu-id="9e38a-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9e38a-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9e38a-121">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="9e38a-121">completedDateTime</span></span>|<span data-ttu-id="9e38a-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e38a-122">DateTimeOffset</span></span>|<span data-ttu-id="9e38a-123">Stellt die bei die Anforderung für diese Richtlinie Datenvorgangs, in UTC-Zeit mit abgeschlossen wurde im ISO 8601-Format.</span><span class="sxs-lookup"><span data-stu-id="9e38a-123">Represents when the request for this data policy operation was completed, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="9e38a-124">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="9e38a-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="9e38a-125">"NULL", bis der Vorgang abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="9e38a-125">Null until the operation completes.</span></span>|
|<span data-ttu-id="9e38a-126">id</span><span class="sxs-lookup"><span data-stu-id="9e38a-126">id</span></span>|<span data-ttu-id="9e38a-127">String</span><span class="sxs-lookup"><span data-stu-id="9e38a-127">String</span></span>| <span data-ttu-id="9e38a-128">Eindeutiger Schlüssel für diesen Vorgang.</span><span class="sxs-lookup"><span data-stu-id="9e38a-128">Unique key for this operation.</span></span> |
|<span data-ttu-id="9e38a-129">status</span><span class="sxs-lookup"><span data-stu-id="9e38a-129">status</span></span>|<span data-ttu-id="9e38a-130">string</span><span class="sxs-lookup"><span data-stu-id="9e38a-130">string</span></span>| <span data-ttu-id="9e38a-131">Mögliche Werte sind: `notStarted`, `running`, `complete`, `failed` und `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="9e38a-131">Possible values are: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="9e38a-132">storageLocation</span><span class="sxs-lookup"><span data-stu-id="9e38a-132">storageLocation</span></span>|<span data-ttu-id="9e38a-133">String</span><span class="sxs-lookup"><span data-stu-id="9e38a-133">String</span></span>|<span data-ttu-id="9e38a-134">Der URL-Adresse an, in dem Daten für exportanforderungen exportiert werden.</span><span class="sxs-lookup"><span data-stu-id="9e38a-134">The URL location to where data is being exported for export requests.</span></span>|
|<span data-ttu-id="9e38a-135">userId</span><span class="sxs-lookup"><span data-stu-id="9e38a-135">userId</span></span>|<span data-ttu-id="9e38a-136">String</span><span class="sxs-lookup"><span data-stu-id="9e38a-136">String</span></span>|<span data-ttu-id="9e38a-137">Die Id für den Benutzer, auf dem die Operation ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="9e38a-137">The id for the user on whom the operation is performed.</span></span>|
|<span data-ttu-id="9e38a-138">submittedDateTime</span><span class="sxs-lookup"><span data-stu-id="9e38a-138">submittedDateTime</span></span>|<span data-ttu-id="9e38a-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e38a-139">DateTimeOffset</span></span>|<span data-ttu-id="9e38a-140">Stellt die bei die Anforderung für diesen Datenvorgang im ISO 8601-Format verwenden übermittelt wurde, im UTC-Zeit.</span><span class="sxs-lookup"><span data-stu-id="9e38a-140">Represents when the request for this data operation was submitted, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="9e38a-141">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="9e38a-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="9e38a-142">progress</span><span class="sxs-lookup"><span data-stu-id="9e38a-142">progress</span></span>|<span data-ttu-id="9e38a-143">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="9e38a-143">Double</span></span>|<span data-ttu-id="9e38a-144">Gibt den Fortschritt eines Vorgangs an.</span><span class="sxs-lookup"><span data-stu-id="9e38a-144">Specifies the progress of an operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9e38a-145">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9e38a-145">Relationships</span></span>
<span data-ttu-id="9e38a-146">Keine</span><span class="sxs-lookup"><span data-stu-id="9e38a-146">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="9e38a-147">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9e38a-147">JSON representation</span></span>

<span data-ttu-id="9e38a-148">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9e38a-148">Here is a JSON representation of the resource.</span></span>

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
  "submittedDateTime": "String (timestamp)",
  "progress": "Double"
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
