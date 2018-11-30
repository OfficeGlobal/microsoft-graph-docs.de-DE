---
title: recurrenceRange-Ressourcentyp
description: 'Beschreibt den Datumsbereich, über den sich ein wiederkehrendes Ereignis wiederholt. '
ms.openlocfilehash: 0e255c28ea2d1e72ae3219e082b3e62b166b1f4c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018944"
---
# <a name="recurrencerange-resource-type"></a><span data-ttu-id="e0c3e-103">recurrenceRange-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e0c3e-103">recurrenceRange resource type</span></span>

<span data-ttu-id="e0c3e-104">Beschreibt den Datumsbereich, über den sich ein wiederkehrendes [Ereignis](event.md) wiederholt.</span><span class="sxs-lookup"><span data-stu-id="e0c3e-104">Describes a date range over which a recurring [event](event.md) repeats.</span></span> 

<span data-ttu-id="e0c3e-105">Je nach Ihrem Szenario können Sie den Datumsbereich einer Ereignisserie in einer der drei folgenden Arten angeben.</span><span class="sxs-lookup"><span data-stu-id="e0c3e-105">You can specify the date range for a recurring event in one of 3 ways depending on your scenario.</span></span> <span data-ttu-id="e0c3e-106">Sie müssen zwar immer einen **startDate**-Wert für den Datumsbereich angeben, Sie können aber auch ein wiederkehrendes Ereignis angeben, das an einen angegebenen Datum endet, das nicht endet oder das nach 5 Vorkommen endet.</span><span class="sxs-lookup"><span data-stu-id="e0c3e-106">While you must always specify a **startDate** value for the date range, you can specify a recurring event that ends by a specific date, or that doesn't end, or that ends after a specific number of occurrences.</span></span> <span data-ttu-id="e0c3e-107">Beachten Sie, dass die tatsächlichen Vorkommen innerhalb des Datumsbereichs immer dem Serienmuster folgen, das Sie für das wiederkehrende Ereignis angeben.</span><span class="sxs-lookup"><span data-stu-id="e0c3e-107">Note that the actual occurrences within the date range always follow the recurrence pattern that you specify for the recurring event.</span></span> <span data-ttu-id="e0c3e-108">Ein wiederkehrendes Ereignis wird immer durch sein [recurrencePattern](recurrencepattern.md) (wie oft sich das Ereignis wiederholt), und seinen **recurrenceRange** (über welchen Zeitraum sich das Ereignis wiederholt) definiert.</span><span class="sxs-lookup"><span data-stu-id="e0c3e-108">A recurring event is always defined by its [recurrencePattern](recurrencepattern.md) (how frequently the event repeats), and its **recurrenceRange** (for how long the event repeats).</span></span>

## <a name="properties"></a><span data-ttu-id="e0c3e-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e0c3e-109">Properties</span></span>

| <span data-ttu-id="e0c3e-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e0c3e-110">Property</span></span>     | <span data-ttu-id="e0c3e-111">Typ</span><span class="sxs-lookup"><span data-stu-id="e0c3e-111">Type</span></span>   |<span data-ttu-id="e0c3e-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e0c3e-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e0c3e-113">endDate</span><span class="sxs-lookup"><span data-stu-id="e0c3e-113">endDate</span></span>|<span data-ttu-id="e0c3e-114">Datum</span><span class="sxs-lookup"><span data-stu-id="e0c3e-114">Date</span></span>|<span data-ttu-id="e0c3e-115">Das Datum zum Beenden des Anwendens des Musters.</span><span class="sxs-lookup"><span data-stu-id="e0c3e-115">The date to stop applying the recurrence pattern.</span></span> <span data-ttu-id="e0c3e-116">Je nach dem Serienmuster des Ereignisses ist das letzte Vorkommen der Besprechung möglicherweise nicht an diesem Datum.</span><span class="sxs-lookup"><span data-stu-id="e0c3e-116">Depending on the recurrence pattern of the event, the last occurrence of the meeting may not be this date.</span></span> <span data-ttu-id="e0c3e-117">Erforderlich, wenn **type** `endDate` ist.</span><span class="sxs-lookup"><span data-stu-id="e0c3e-117">Required if **type** is `endDate`.</span></span>|
|<span data-ttu-id="e0c3e-118">numberOfOccurrences</span><span class="sxs-lookup"><span data-stu-id="e0c3e-118">numberOfOccurrences</span></span>|<span data-ttu-id="e0c3e-119">Int32</span><span class="sxs-lookup"><span data-stu-id="e0c3e-119">Int32</span></span>|<span data-ttu-id="e0c3e-120">Die Anzahl von Wiederholungen für das Ereignis.</span><span class="sxs-lookup"><span data-stu-id="e0c3e-120">The number of times to repeat the event.</span></span> <span data-ttu-id="e0c3e-121">Erforderlich; muss positiv sein, wenn **type** `numbered` ist.</span><span class="sxs-lookup"><span data-stu-id="e0c3e-121">Required and must be positive if **type** is `numbered`.</span></span>|
|<span data-ttu-id="e0c3e-122">recurrenceTimeZone</span><span class="sxs-lookup"><span data-stu-id="e0c3e-122">recurrenceTimeZone</span></span>|<span data-ttu-id="e0c3e-123">String</span><span class="sxs-lookup"><span data-stu-id="e0c3e-123">String</span></span> |<span data-ttu-id="e0c3e-124">Zeitzone für die **startDate**- und **endDate**-Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="e0c3e-124">Time zone for the **startDate** and **endDate** properties.</span></span> <span data-ttu-id="e0c3e-125">Optional.</span><span class="sxs-lookup"><span data-stu-id="e0c3e-125">Optional.</span></span> <span data-ttu-id="e0c3e-126">Falls nicht angegeben, wird die Zeitzone des Ereignisses verwendet.</span><span class="sxs-lookup"><span data-stu-id="e0c3e-126">If not specified, the time zone of the event is used.</span></span>|
|<span data-ttu-id="e0c3e-127">startDate</span><span class="sxs-lookup"><span data-stu-id="e0c3e-127">startDate</span></span>|<span data-ttu-id="e0c3e-128">Datum</span><span class="sxs-lookup"><span data-stu-id="e0c3e-128">Date</span></span>|<span data-ttu-id="e0c3e-129">Das Datum zum Starten des Anwendens des Musters.</span><span class="sxs-lookup"><span data-stu-id="e0c3e-129">The date to start applying the recurrence pattern.</span></span> <span data-ttu-id="e0c3e-130">Je nach dem Serienmuster des Ereignisses findet das erste Vorkommen der Besprechung möglicherweise an diesem Datum oder später statt.</span><span class="sxs-lookup"><span data-stu-id="e0c3e-130">The first occurrence of the meeting may be this date or later, depending on the recurrence pattern of the event.</span></span> <span data-ttu-id="e0c3e-131">Muss der gleiche Wert wie die **start**-Eigenschaft des wiederkehrenden [Ereignisses](event.md) sein.</span><span class="sxs-lookup"><span data-stu-id="e0c3e-131">Must be the same value as the **start** property of the recurring [event](event.md).</span></span> <span data-ttu-id="e0c3e-132">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e0c3e-132">Required.</span></span>|
|<span data-ttu-id="e0c3e-133">type</span><span class="sxs-lookup"><span data-stu-id="e0c3e-133">type</span></span>|<span data-ttu-id="e0c3e-134">recurrenceRangeType</span><span class="sxs-lookup"><span data-stu-id="e0c3e-134">recurrenceRangeType</span></span>|<span data-ttu-id="e0c3e-135">Der Serienbereich.</span><span class="sxs-lookup"><span data-stu-id="e0c3e-135">The recurrence range.</span></span> <span data-ttu-id="e0c3e-136">Die möglichen Werte sind: `endDate`, `noEnd`, `numbered`.</span><span class="sxs-lookup"><span data-stu-id="e0c3e-136">The possible values are: `endDate`, `noEnd`, `numbered`.</span></span> <span data-ttu-id="e0c3e-137">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e0c3e-137">Required.</span></span>|

<span data-ttu-id="e0c3e-138">Verwenden Sie die **type**-Eigenschaft, um die unterschiedlichen Typen von **recurrenceRange** anzugeben.</span><span class="sxs-lookup"><span data-stu-id="e0c3e-138">Use the **type** property to specify the different types of **recurrenceRange**.</span></span> <span data-ttu-id="e0c3e-139">Beachten Sie die erforderlichen Eigenschaften für jeden Typ, wie in der folgenden Tabelle beschrieben.</span><span class="sxs-lookup"><span data-stu-id="e0c3e-139">Note the required properties for each type, as described in the following table.</span></span>

| <span data-ttu-id="e0c3e-140">Eigenschaft "type"</span><span class="sxs-lookup"><span data-stu-id="e0c3e-140">type property</span></span>  | <span data-ttu-id="e0c3e-141">Typ des Serienbereichs</span><span class="sxs-lookup"><span data-stu-id="e0c3e-141">Type of recurrence range</span></span> | <span data-ttu-id="e0c3e-142">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e0c3e-142">Description</span></span> | <span data-ttu-id="e0c3e-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e0c3e-143">Example</span></span> | <span data-ttu-id="e0c3e-144">Erforderliche Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e0c3e-144">Required properties</span></span> |
|:-------|:---------------|:--------|:--------|:--------|
|`endDate` |<span data-ttu-id="e0c3e-145">Bereich mit Enddatum</span><span class="sxs-lookup"><span data-stu-id="e0c3e-145">Range with end date</span></span> | <span data-ttu-id="e0c3e-146">Ereignis an allen Tagen wiederholen, die mit dem entsprechenden Serienmuster zwischen dem **startDate** und dem **endDate** übereinstimmen.</span><span class="sxs-lookup"><span data-stu-id="e0c3e-146">Event repeats on all the days that fit the corresponding recurrence pattern between the **startDate** and **endDate** inclusive.</span></span> | <span data-ttu-id="e0c3e-147">Ereignis im Datumsbereich zwischen 1. Juni 2017 und 15. Juni 2017 wiederholen.</span><span class="sxs-lookup"><span data-stu-id="e0c3e-147">Repeat event in the date range between June 1, 2017 and June 15, 2017.</span></span> | <span data-ttu-id="e0c3e-148">**type**, **startDate**, **endDate**</span><span class="sxs-lookup"><span data-stu-id="e0c3e-148">**type**, **startDate**, **endDate**</span></span> | 
|`noEnd`  |<span data-ttu-id="e0c3e-149">Bereich ohne Enddatum</span><span class="sxs-lookup"><span data-stu-id="e0c3e-149">Range without an end date</span></span> | <span data-ttu-id="e0c3e-150">Ereignis an allen Tagen wiederholen, die mit dem entsprechenden Serienmuster beginnend am **startDate** übereinstimmen.</span><span class="sxs-lookup"><span data-stu-id="e0c3e-150">Event repeats on all the days that fit the corresponding recurrence pattern beginning on the **startDate**.</span></span> | <span data-ttu-id="e0c3e-151">Ereignis im Datumsbereich beginnend am 1. Juni 2017 unbegrenzt wiederholen.</span><span class="sxs-lookup"><span data-stu-id="e0c3e-151">Repeat event in the date range starting on June 1, 2017 indefinitely.</span></span> | <span data-ttu-id="e0c3e-152">**type**, **startDate**</span><span class="sxs-lookup"><span data-stu-id="e0c3e-152">**type**, **startDate**</span></span> |
|`numbered`|<span data-ttu-id="e0c3e-153">Bereich mit einer bestimmten Anzahl von Vorkommen</span><span class="sxs-lookup"><span data-stu-id="e0c3e-153">Range with specific number of occurrences</span></span> | <span data-ttu-id="e0c3e-154">Ereignis für die **numberOfOccurrences** basierend auf dem Serienmuster beginnend am **startDate** wiederholen.</span><span class="sxs-lookup"><span data-stu-id="e0c3e-154">Event repeats for the **numberOfOccurrences** based on the recurrence pattern beginning on the **startDate**.</span></span> | <span data-ttu-id="e0c3e-155">Ereignis im Datumsbereich beginnend am 1. Juni 2017 für 10 Vorkommen wiederholen.</span><span class="sxs-lookup"><span data-stu-id="e0c3e-155">Repeat event in the date range starting on June 1, 2017, for 10 occurrences.</span></span>  | <span data-ttu-id="e0c3e-156">**type**, **startDate**, **numberOfOccurrences**</span><span class="sxs-lookup"><span data-stu-id="e0c3e-156">**type**, **startDate**, **numberOfOccurrences**</span></span> |


## <a name="json-representation"></a><span data-ttu-id="e0c3e-157">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e0c3e-157">JSON representation</span></span>

<span data-ttu-id="e0c3e-158">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e0c3e-158">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recurrenceRange"
}-->

```json
{
  "endDate": "String (timestamp)",
  "numberOfOccurrences": 1024,
  "recurrenceTimeZone": "string",
  "startDate": "String (timestamp)",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recurrenceRange resource",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
      "Warning: /api-reference/v1.0/resources/recurrencerange.md:
      Failed to parse any rows out of table with headers: | type property  | Type of recurrence range | Description | Example | Required properties |"
  ],
  "tocPath": ""
}-->
