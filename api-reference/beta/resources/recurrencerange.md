---
title: recurrenceRange-Ressourcentyp
description: 'Beschreibt den Datumsbereich, über den sich ein wiederkehrendes Ereignis wiederholt. '
ms.openlocfilehash: f3d627606dc9d0d41dd52f735ab87052d731af0d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061238"
---
# <a name="recurrencerange-resource-type"></a><span data-ttu-id="6b6ab-103">recurrenceRange-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6b6ab-103">recurrenceRange resource type</span></span>

> <span data-ttu-id="6b6ab-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6b6ab-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6b6ab-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6b6ab-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6b6ab-106">Beschreibt den Datumsbereich, über den sich ein wiederkehrendes [Ereignis](event.md) wiederholt.</span><span class="sxs-lookup"><span data-stu-id="6b6ab-106">Describes a date range over which a recurring [event](event.md) repeats.</span></span> 

<span data-ttu-id="6b6ab-107">Je nach Ihrem Szenario können Sie den Datumsbereich einer Ereignisserie in einer der drei folgenden Arten angeben.</span><span class="sxs-lookup"><span data-stu-id="6b6ab-107">You can specify the date range for a recurring event in one of 3 ways depending on your scenario.</span></span> <span data-ttu-id="6b6ab-108">Sie müssen zwar immer einen **startDate**-Wert für den Datumsbereich angeben, Sie können aber auch ein wiederkehrendes Ereignis angeben, das an einen angegebenen Datum endet, das nicht endet oder das nach 5 Vorkommen endet.</span><span class="sxs-lookup"><span data-stu-id="6b6ab-108">While you must always specify a **startDate** value for the date range, you can specify a recurring event that ends by a specific date, or that doesn't end, or that ends after a specific number of occurrences.</span></span> <span data-ttu-id="6b6ab-109">Beachten Sie, dass die tatsächlichen Vorkommen innerhalb des Datumsbereichs immer dem Serienmuster folgen, das Sie für das wiederkehrende Ereignis angeben.</span><span class="sxs-lookup"><span data-stu-id="6b6ab-109">Note that the actual occurrences within the date range always follow the recurrence pattern that you specify for the recurring event.</span></span> <span data-ttu-id="6b6ab-110">Ein wiederkehrendes Ereignis wird immer durch sein [recurrencePattern](recurrencepattern.md) (wie oft sich das Ereignis wiederholt), und seinen **recurrenceRange** (über welchen Zeitraum sich das Ereignis wiederholt) definiert.</span><span class="sxs-lookup"><span data-stu-id="6b6ab-110">A recurring event is always defined by its [recurrencePattern](recurrencepattern.md) (how frequently the event repeats), and its **recurrenceRange** (for how long the event repeats).</span></span>


## <a name="properties"></a><span data-ttu-id="6b6ab-111">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6b6ab-111">Properties</span></span>

| <span data-ttu-id="6b6ab-112">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6b6ab-112">Property</span></span>     | <span data-ttu-id="6b6ab-113">Typ</span><span class="sxs-lookup"><span data-stu-id="6b6ab-113">Type</span></span>   |<span data-ttu-id="6b6ab-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6b6ab-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6b6ab-115">endDate</span><span class="sxs-lookup"><span data-stu-id="6b6ab-115">endDate</span></span>|<span data-ttu-id="6b6ab-116">Datum</span><span class="sxs-lookup"><span data-stu-id="6b6ab-116">Date</span></span>|<span data-ttu-id="6b6ab-117">Das Datum zum Beenden des Anwendens des Musters.</span><span class="sxs-lookup"><span data-stu-id="6b6ab-117">The date to stop applying the recurrence pattern.</span></span> <span data-ttu-id="6b6ab-118">Je nach dem Serienmuster des Ereignisses ist das letzte Vorkommen der Besprechung möglicherweise nicht an diesem Datum.</span><span class="sxs-lookup"><span data-stu-id="6b6ab-118">Depending on the recurrence pattern of the event, the last occurrence of the meeting may not be this date.</span></span> <span data-ttu-id="6b6ab-119">Erforderlich, wenn **type** `endDate` ist.</span><span class="sxs-lookup"><span data-stu-id="6b6ab-119">Required if **type** is `endDate`.</span></span>|
|<span data-ttu-id="6b6ab-120">numberOfOccurrences</span><span class="sxs-lookup"><span data-stu-id="6b6ab-120">numberOfOccurrences</span></span>|<span data-ttu-id="6b6ab-121">Int32</span><span class="sxs-lookup"><span data-stu-id="6b6ab-121">Int32</span></span>|<span data-ttu-id="6b6ab-122">Die Anzahl von Wiederholungen für das Ereignis.</span><span class="sxs-lookup"><span data-stu-id="6b6ab-122">The number of times to repeat the event.</span></span> <span data-ttu-id="6b6ab-123">Erforderlich; muss positiv sein, wenn **type** `numbered` ist.</span><span class="sxs-lookup"><span data-stu-id="6b6ab-123">Required and must be positive if **type** is `numbered`.</span></span>|
|<span data-ttu-id="6b6ab-124">recurrenceTimeZone</span><span class="sxs-lookup"><span data-stu-id="6b6ab-124">recurrenceTimeZone</span></span>|<span data-ttu-id="6b6ab-125">String</span><span class="sxs-lookup"><span data-stu-id="6b6ab-125">String</span></span> |<span data-ttu-id="6b6ab-126">Zeitzone für die **startDate**- und **endDate**-Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="6b6ab-126">Time zone for the **startDate** and **endDate** properties.</span></span> <span data-ttu-id="6b6ab-127">Optional.</span><span class="sxs-lookup"><span data-stu-id="6b6ab-127">Optional.</span></span> <span data-ttu-id="6b6ab-128">Falls nicht angegeben, wird die Zeitzone des Ereignisses verwendet.</span><span class="sxs-lookup"><span data-stu-id="6b6ab-128">If not specified, the time zone of the event is used.</span></span>|
|<span data-ttu-id="6b6ab-129">startDate</span><span class="sxs-lookup"><span data-stu-id="6b6ab-129">startDate</span></span>|<span data-ttu-id="6b6ab-130">Datum</span><span class="sxs-lookup"><span data-stu-id="6b6ab-130">Date</span></span>|<span data-ttu-id="6b6ab-131">Das Datum zum Starten des Anwendens des Musters.</span><span class="sxs-lookup"><span data-stu-id="6b6ab-131">The date to start applying the recurrence pattern.</span></span> <span data-ttu-id="6b6ab-132">Je nach dem Serienmuster des Ereignisses findet das erste Vorkommen der Besprechung möglicherweise an diesem Datum oder später statt.</span><span class="sxs-lookup"><span data-stu-id="6b6ab-132">The first occurrence of the meeting may be this date or later, depending on the recurrence pattern of the event.</span></span> <span data-ttu-id="6b6ab-133">Muss der gleiche Wert wie die **start**-Eigenschaft des wiederkehrenden [Ereignisses](event.md) sein.</span><span class="sxs-lookup"><span data-stu-id="6b6ab-133">Must be the same value as the **start** property of the recurring [event](event.md).</span></span> <span data-ttu-id="6b6ab-134">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6b6ab-134">Required.</span></span>|
|<span data-ttu-id="6b6ab-135">type</span><span class="sxs-lookup"><span data-stu-id="6b6ab-135">type</span></span>|<span data-ttu-id="6b6ab-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6b6ab-136">String</span></span>|<span data-ttu-id="6b6ab-137">Der Serienbereich.</span><span class="sxs-lookup"><span data-stu-id="6b6ab-137">The recurrence range.</span></span> <span data-ttu-id="6b6ab-138">Mögliche Werte: `endDate`, `noEnd`, `numbered`.</span><span class="sxs-lookup"><span data-stu-id="6b6ab-138">Possible values are: `endDate`, `noEnd`, `numbered`.</span></span> <span data-ttu-id="6b6ab-139">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6b6ab-139">Required.</span></span>|

<span data-ttu-id="6b6ab-140">Verwenden Sie die **type**-Eigenschaft, um die unterschiedlichen Typen von **recurrenceRange** anzugeben.</span><span class="sxs-lookup"><span data-stu-id="6b6ab-140">Use the **type** property to specify the different types of **recurrenceRange**.</span></span> <span data-ttu-id="6b6ab-141">Beachten Sie die erforderlichen Eigenschaften für jeden Typ, wie in der folgenden Tabelle beschrieben.</span><span class="sxs-lookup"><span data-stu-id="6b6ab-141">Note the required properties for each type, as described in the following table.</span></span>

| <span data-ttu-id="6b6ab-142">Eigenschaft "type"</span><span class="sxs-lookup"><span data-stu-id="6b6ab-142">type property</span></span>  | <span data-ttu-id="6b6ab-143">Typ des Serienbereichs</span><span class="sxs-lookup"><span data-stu-id="6b6ab-143">Type of recurrence range</span></span> | <span data-ttu-id="6b6ab-144">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6b6ab-144">Description</span></span> | <span data-ttu-id="6b6ab-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6b6ab-145">Example</span></span> | <span data-ttu-id="6b6ab-146">Erforderliche Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6b6ab-146">Required properties</span></span> |
|:-------|:---------------|:--------|:--------|:--------|
|`endDate` |<span data-ttu-id="6b6ab-147">Bereich mit Enddatum</span><span class="sxs-lookup"><span data-stu-id="6b6ab-147">Range with end date</span></span> | <span data-ttu-id="6b6ab-148">Ereignis an allen Tagen wiederholen, die mit dem entsprechenden Serienmuster zwischen dem **startDate** und dem **endDate** übereinstimmen.</span><span class="sxs-lookup"><span data-stu-id="6b6ab-148">Event repeats on all the days that fit the corresponding recurrence pattern between the **startDate** and **endDate** inclusive.</span></span> | <span data-ttu-id="6b6ab-149">Ereignis im Datumsbereich zwischen 1. Juni 2017 und 15. Juni 2017 wiederholen.</span><span class="sxs-lookup"><span data-stu-id="6b6ab-149">Repeat event in the date range between June 1, 2017 and June 15, 2017.</span></span> | <span data-ttu-id="6b6ab-150">**type**, **startDate**, **endDate**</span><span class="sxs-lookup"><span data-stu-id="6b6ab-150">**type**, **startDate**, **endDate**</span></span> | 
|`noEnd`   |<span data-ttu-id="6b6ab-151">Bereich ohne Enddatum</span><span class="sxs-lookup"><span data-stu-id="6b6ab-151">Range without an end date</span></span> | <span data-ttu-id="6b6ab-152">Ereignis an allen Tagen wiederholen, die mit dem entsprechenden Serienmuster beginnend am **startDate** übereinstimmen.</span><span class="sxs-lookup"><span data-stu-id="6b6ab-152">Event repeats on all the days that fit the corresponding recurrence pattern beginning on the **startDate**.</span></span> | <span data-ttu-id="6b6ab-153">Ereignis im Datumsbereich beginnend am 1. Juni 2017 unbegrenzt wiederholen.</span><span class="sxs-lookup"><span data-stu-id="6b6ab-153">Repeat event in the date range starting on June 1, 2017 indefinitely.</span></span> | <span data-ttu-id="6b6ab-154">**type**, **startDate**</span><span class="sxs-lookup"><span data-stu-id="6b6ab-154">**type**, **startDate**</span></span> |
|`numbered`|<span data-ttu-id="6b6ab-155">Bereich mit einer bestimmten Anzahl von Vorkommen</span><span class="sxs-lookup"><span data-stu-id="6b6ab-155">Range with specific number of occurrences</span></span> | <span data-ttu-id="6b6ab-156">Ereignis für die **numberOfOccurrences** basierend auf dem Serienmuster beginnend am **startDate** wiederholen.</span><span class="sxs-lookup"><span data-stu-id="6b6ab-156">Event repeats for the **numberOfOccurrences** based on the recurrence pattern beginning on the **startDate**.</span></span> | <span data-ttu-id="6b6ab-157">Ereignis im Datumsbereich beginnend am 1. Juni 2017 für 10 Vorkommen wiederholen.</span><span class="sxs-lookup"><span data-stu-id="6b6ab-157">Repeat event in the date range starting on June 1, 2017, for 10 occurrences.</span></span>  | <span data-ttu-id="6b6ab-158">**type**, **startDate**, **numberOfOccurrences**</span><span class="sxs-lookup"><span data-stu-id="6b6ab-158">**type**, **startDate**, **numberOfOccurrences**</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6b6ab-159">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6b6ab-159">JSON representation</span></span>

<span data-ttu-id="6b6ab-160">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6b6ab-160">Here is a JSON representation of the resource</span></span>

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
      "Warning: /api-reference/beta/resources/recurrencerange.md:
      Failed to parse any rows out of table with headers: | type property  | Type of recurrence range | Description | Example | Required properties |"
  ],
  "tocPath": ""
}-->
