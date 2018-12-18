---
title: Planen wiederkehrender Termine als wiederkehrende Ereignisse in Outlook
description: Ereignisserien sind ein wichtiger Bestandteil der Kalenderfunktionen von Outlook. Ganz gleich, ob es sich um eine wöchentliche Besprechung mit Ihrem Vorgesetzten oder eine Abteilungsbesprechung handelt, die jeden zweiten Dienstag im Monat stattfindet, mit Ereignisserien können Sie ganz einfach eine Ereignisserie erstellen und der Server füllt den Kalender mit dem Rest der Serie.
author: angelgolfer-ms
ms.openlocfilehash: 85d856cd9f59ee7df643ff74ed4b3dd9f48ba3a4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340075"
---
# <a name="schedule-repeating-appointments-as-recurring-events-in-outlook"></a><span data-ttu-id="0a0dd-104">Planen wiederkehrender Termine als wiederkehrende Ereignisse in Outlook</span><span class="sxs-lookup"><span data-stu-id="0a0dd-104">Schedule repeating appointments as recurring events in Outlook</span></span>

<span data-ttu-id="0a0dd-105">Ereignisserien sind ein wichtiger Bestandteil der Kalenderfunktionen von Outlook.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-105">Recurring events are an important part of Outlook calendaring.</span></span> <span data-ttu-id="0a0dd-106">Ganz gleich, ob es sich um eine wöchentliche Besprechung mit Ihrem Vorgesetzten oder eine Abteilungsbesprechung handelt, die jeden zweiten Dienstag im Monat stattfindet, mit Ereignisserien können Sie ganz einfach eine Ereignisserie erstellen und der Server füllt den Kalender mit dem Rest der Serie.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-106">Whether it's a weekly one-on-one meeting with your manager, or a division-wide review meeting that happens on the second Tuesday of each month, recurring events make it easy to create the event once, and let the server fill in the rest of the series.</span></span>

<span data-ttu-id="0a0dd-107">Die wichtigsten Informationen, mit denen Ereignisserien in einzelne Termine „erweitert“ werden können, die Serienregel.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-107">The key bit of information that allows recurring events to "expand" into individual occurrences is the recurrence rule.</span></span> <span data-ttu-id="0a0dd-108">In der Serie ist die Wiederholungsfrequenz und Dauer eines Ereignisses angegeben.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-108">The rule specifies both how often an event repeats, and for how long.</span></span> <span data-ttu-id="0a0dd-109">Die Outlook-REST-APIs modellieren Serienregeln in der **Serien**-Eigenschaft der [Ereignisressource](/graph/api/resources/event?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="0a0dd-109">The Outlook REST APIs model recurrence rules in the **recurrence** property of the [event resource](/graph/api/resources/event?view=graph-rest-1.0).</span></span> 

<span data-ttu-id="0a0dd-110">Jede Serie besteht aus zwei Teilen: dem Serienmuster (wie oft) und dem Serienbereich (für wie lange).</span><span class="sxs-lookup"><span data-stu-id="0a0dd-110">Each recurrence is made up of two parts: the recurrence pattern (how often), and the recurrence range (for how long).</span></span>

## <a name="recurrence-patterns"></a><span data-ttu-id="0a0dd-111">Serienmuster</span><span class="sxs-lookup"><span data-stu-id="0a0dd-111">Recurrence patterns</span></span>

<span data-ttu-id="0a0dd-112">Der erste Teil einer Serie ist das Muster.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-112">The first part of a recurrence is the pattern.</span></span> <span data-ttu-id="0a0dd-113">Darin ist angegeben, wie oft das Ereignis wiederholt wird.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-113">This specifies how often the event repeats.</span></span> <span data-ttu-id="0a0dd-114">Beispielsweise könnte ein Ereignis „alle 3 Tage“, „jeden Donnerstag“ oder „jedes Jahr am 22. Juli“ wiederholt werden.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-114">For example, an event could repeat "every 3 days," "every Thursday," or "on July 22 every year."</span></span> <span data-ttu-id="0a0dd-115">Ein Muster wird in der API durch die [recurrencePattern-Ressource](/graph/api/resources/recurrencepattern?view=graph-rest-1.0) dargestellt.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-115">A pattern is represented in the API by the [recurrencePattern resource](/graph/api/resources/recurrencepattern?view=graph-rest-1.0).</span></span>

<span data-ttu-id="0a0dd-116">Je nach Mustertyp sind bestimmte Felder des **recurrencePattern** obligatorisch, optional oder werden ignoriert.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-116">Depending on the type of pattern, certain fields of the **recurrencePattern** are required, optional, or ignored.</span></span>

> <span data-ttu-id="0a0dd-117">**Hinweis:** Auch wenn ein Feld ignoriert wird, wird es dennoch überprüft.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-117">**Note**: Even if a field is ignored, it is still validated.</span></span> <span data-ttu-id="0a0dd-118">Wenn ein Feld über eine festgelegte Liste möglicher Werte verfügt, führt ein Wert außerhalb der zulässigen Gruppe von Werten zu einem Fehler, selbst wenn das Feld ignoriert wird.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-118">If a field has a set list of possible values, using a value outside the allowed set causes an error, even if that field is ignored.</span></span>

<span data-ttu-id="0a0dd-119">Werfen Sie einen Blick auf die einzelnen Arten möglicher Muster.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-119">Let's take a look at each of the possible pattern types.</span></span>

### <a name="daily"></a><span data-ttu-id="0a0dd-120">Täglich</span><span class="sxs-lookup"><span data-stu-id="0a0dd-120">Daily</span></span>

<span data-ttu-id="0a0dd-121">Das tägliche Serienmuster bewirkt, dass ein Ereignis basierend auf einer Anzahl von Tagen zwischen zwei Vorkommen wiederholt wird.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-121">The daily recurrence pattern causes an event to repeat based on a number of days between each occurrence.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="0a0dd-122">Relevante Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0a0dd-122">Relevant properties</span></span>

| <span data-ttu-id="0a0dd-123">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0a0dd-123">Property</span></span> | <span data-ttu-id="0a0dd-124">Relevanz</span><span class="sxs-lookup"><span data-stu-id="0a0dd-124">Relevance</span></span> | <span data-ttu-id="0a0dd-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0a0dd-125">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="0a0dd-126">**Intervall**</span><span class="sxs-lookup"><span data-stu-id="0a0dd-126">**interval**</span></span> | <span data-ttu-id="0a0dd-127">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="0a0dd-127">Required</span></span> | <span data-ttu-id="0a0dd-128">Gibt die Anzahl der Tage zwischen zwei Vorkommen an.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-128">Specifies the number of days between each occurrence.</span></span> |
| <span data-ttu-id="0a0dd-129">**Typ**</span><span class="sxs-lookup"><span data-stu-id="0a0dd-129">**type**</span></span> | <span data-ttu-id="0a0dd-130">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="0a0dd-130">Required</span></span> | <span data-ttu-id="0a0dd-131">Muss auf `daily` festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-131">Must be set to `daily`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="0a0dd-132">Beispiele</span><span class="sxs-lookup"><span data-stu-id="0a0dd-132">Examples</span></span>

- <span data-ttu-id="0a0dd-133">Dieses Ereignis täglich wiederholen</span><span class="sxs-lookup"><span data-stu-id="0a0dd-133">Repeat this event every day</span></span>

  ```json
    "pattern": {
      "type": "daily",
      "interval": 1
    }
  ```
- <span data-ttu-id="0a0dd-134">Dieses Ereignis alle drei Tage wiederholen</span><span class="sxs-lookup"><span data-stu-id="0a0dd-134">Repeat this event every three days</span></span>

  ```json
    "pattern": {
      "type": "daily",
      "interval": 3
    }
  ```

### <a name="weekly"></a><span data-ttu-id="0a0dd-135">Wöchentlich</span><span class="sxs-lookup"><span data-stu-id="0a0dd-135">Weekly</span></span>

<span data-ttu-id="0a0dd-136">Das wöchentliche Serienmuster bewirkt, dass ein Ereignis am gleichen Tag oder an den gleichen Tagen einer Woche basierend auf der Anzahl von Wochen zwischen zwei Vorkommen wiederholt wird.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-136">The weekly recurrence pattern causes an event to repeat on the same day or days of the week, based on the number of weeks between each set of occurrences.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="0a0dd-137">Relevante Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0a0dd-137">Relevant properties</span></span>

| <span data-ttu-id="0a0dd-138">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0a0dd-138">Property</span></span> | <span data-ttu-id="0a0dd-139">Relevanz</span><span class="sxs-lookup"><span data-stu-id="0a0dd-139">Relevance</span></span> | <span data-ttu-id="0a0dd-140">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0a0dd-140">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="0a0dd-141">**daysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="0a0dd-141">**daysOfWeek**</span></span> | <span data-ttu-id="0a0dd-142">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="0a0dd-142">Required</span></span> | <span data-ttu-id="0a0dd-143">Gibt an, an welchem/-n Tag/-en der Woche das Ereignis eintritt.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-143">Specifies on which day(s) of the week the event occurs.</span></span> |
| <span data-ttu-id="0a0dd-144">**firstDayOfWeek**</span><span class="sxs-lookup"><span data-stu-id="0a0dd-144">**firstDayOfWeek**</span></span> | <span data-ttu-id="0a0dd-145">Optional</span><span class="sxs-lookup"><span data-stu-id="0a0dd-145">Optional</span></span> | <span data-ttu-id="0a0dd-146">Gibt an, welcher Tag als erster Tag der Woche angesehen wird.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-146">Specifies which day is considered the first day of the week.</span></span> <span data-ttu-id="0a0dd-147">Standardwert: `Sunday`.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-147">Default value: `Sunday`.</span></span> |
| <span data-ttu-id="0a0dd-148">**Intervall**</span><span class="sxs-lookup"><span data-stu-id="0a0dd-148">**interval**</span></span> | <span data-ttu-id="0a0dd-149">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="0a0dd-149">Required</span></span> | <span data-ttu-id="0a0dd-150">Gibt die Anzahl der Wochen zwischen zwei Vorkommen an.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-150">Specifies the number of weeks between each set of occurrences.</span></span> |
| <span data-ttu-id="0a0dd-151">**Typ**</span><span class="sxs-lookup"><span data-stu-id="0a0dd-151">**type**</span></span> | <span data-ttu-id="0a0dd-152">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="0a0dd-152">Required</span></span> | <span data-ttu-id="0a0dd-153">Muss auf `weekly` festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-153">Must be set to `weekly`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="0a0dd-154">Beispiele</span><span class="sxs-lookup"><span data-stu-id="0a0dd-154">Examples</span></span>

- <span data-ttu-id="0a0dd-155">Dieses Ereignis jeden Donnerstag wiederholen</span><span class="sxs-lookup"><span data-stu-id="0a0dd-155">Repeat this event every Thursday</span></span>

  ```json
    "pattern": {
      "type": "weekly",
      "interval": 1,
      "daysOfWeek": [ "Thursday" ]
    }
  ```
- <span data-ttu-id="0a0dd-156">Dieses Ereignis jeden Montag und Dienstag wiederholen</span><span class="sxs-lookup"><span data-stu-id="0a0dd-156">Repeat this event every other Monday and Tuesday</span></span>

  ```json
    "pattern": {
      "type": "weekly",
      "interval": 2,
      "daysOfWeek": [
        "Monday",
        "Tuesday"
      ]
    }
  ```

### <a name="absolute-monthly"></a><span data-ttu-id="0a0dd-157">Absolut monatlich</span><span class="sxs-lookup"><span data-stu-id="0a0dd-157">Absolute monthly</span></span>

<span data-ttu-id="0a0dd-158">Das absolute monatliche Muster bewirkt, dass ein Ereignis am gleichen Tag des Monats (z. B. dem 15.) basierend auf der Anzahl der Monate zwischen zwei Vorkommen stattfindet.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-158">The absolute monthly pattern causes an event to repeat on the same day of the month (for example, the 15th), based on the number of months between each occurrence.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="0a0dd-159">Relevante Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0a0dd-159">Relevant properties</span></span>

| <span data-ttu-id="0a0dd-160">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0a0dd-160">Property</span></span> | <span data-ttu-id="0a0dd-161">Relevanz</span><span class="sxs-lookup"><span data-stu-id="0a0dd-161">Relevance</span></span> | <span data-ttu-id="0a0dd-162">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0a0dd-162">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="0a0dd-163">**dayOfMonth**</span><span class="sxs-lookup"><span data-stu-id="0a0dd-163">**dayOfMonth**</span></span> | <span data-ttu-id="0a0dd-164">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="0a0dd-164">Required</span></span> | <span data-ttu-id="0a0dd-165">Gibt an, an welchem Tag des Monats das Ereignis eintritt.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-165">Specifies on which day of the month the event occurs.</span></span> |
| <span data-ttu-id="0a0dd-166">**Intervall**</span><span class="sxs-lookup"><span data-stu-id="0a0dd-166">**interval**</span></span> | <span data-ttu-id="0a0dd-167">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="0a0dd-167">Required</span></span> | <span data-ttu-id="0a0dd-168">Gibt die Anzahl der Monate zwischen zwei Vorkommen an.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-168">Specifies the number of months between each occurrence.</span></span> |
| <span data-ttu-id="0a0dd-169">**Typ**</span><span class="sxs-lookup"><span data-stu-id="0a0dd-169">**type**</span></span> | <span data-ttu-id="0a0dd-170">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="0a0dd-170">Required</span></span> | <span data-ttu-id="0a0dd-171">Muss auf `absoluteMonthly` festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-171">Must be set to `absoluteMonthly`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="0a0dd-172">Beispiele</span><span class="sxs-lookup"><span data-stu-id="0a0dd-172">Examples</span></span>

- <span data-ttu-id="0a0dd-173">Dieses Ereignis jeden Monat am 15. wiederholen</span><span class="sxs-lookup"><span data-stu-id="0a0dd-173">Repeat this event on the 15th of every month</span></span>

  ```json
    "pattern": {
      "type": "absoluteMonthly",
      "interval": 1,
      "dayOfMonth": 15
    }
  ```
- <span data-ttu-id="0a0dd-174">Dieses Ereignis vierteljährlich (alle 3 Monate) am 7. wiederholen</span><span class="sxs-lookup"><span data-stu-id="0a0dd-174">Repeat this event quarterly (every 3 months) on the 7th</span></span>

  ```json
    "pattern": {
      "type": "absoluteMonthly",
      "interval": 3,
      "dayOfMonth": 7
    }
  ```

### <a name="relative-monthly"></a><span data-ttu-id="0a0dd-175">Relativ monatlich</span><span class="sxs-lookup"><span data-stu-id="0a0dd-175">Relative monthly</span></span>

<span data-ttu-id="0a0dd-176">Das relative monatliche Muster bewirkt, dass ein Ereignis am gleichen Wochentag an der gleichen relativen Position des Monats basierend auf der Anzahl der Monate zwischen zwei Vorkommen stattfindet.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-176">The relative monthly pattern causes an event to repeat on the same day of the week in the same relative position in the month, based on the number of months between each occurrence.</span></span> <span data-ttu-id="0a0dd-177">Beispielsweise „jeden zweiten Mittwoch des Monats“.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-177">For example, "every second Wednesday of the month."</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="0a0dd-178">Relevante Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0a0dd-178">Relevant properties</span></span>

| <span data-ttu-id="0a0dd-179">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0a0dd-179">Property</span></span> | <span data-ttu-id="0a0dd-180">Relevanz</span><span class="sxs-lookup"><span data-stu-id="0a0dd-180">Relevance</span></span> | <span data-ttu-id="0a0dd-181">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0a0dd-181">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="0a0dd-182">**daysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="0a0dd-182">**daysOfWeek**</span></span> | <span data-ttu-id="0a0dd-183">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="0a0dd-183">Required</span></span> | <span data-ttu-id="0a0dd-184">Gibt an, an welchem/-n Tag/-en der Woche das Ereignis eintreten kann.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-184">Specifies on which day(s) of the week the event can occur.</span></span> <span data-ttu-id="0a0dd-185">Relative monatliche Ereignisse treten nur einmal pro Monat ein, wird also mehr als ein Wert angegeben, fällt das Ereignis auf den ersten Tag, der das Muster erfüllt.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-185">Relative monthly events only occur once per month, so if more than one value is specified, the event falls on the first day that satisfies the pattern.</span></span> |
| <span data-ttu-id="0a0dd-186">**Index**</span><span class="sxs-lookup"><span data-stu-id="0a0dd-186">**index**</span></span> | <span data-ttu-id="0a0dd-187">Optional</span><span class="sxs-lookup"><span data-stu-id="0a0dd-187">Optional</span></span> | <span data-ttu-id="0a0dd-188">Gibt an, in welcher Instanz der zulässigen Tage, die unter **daysOfsWeek** angegeben sind, das Ereignis eintritt, ausgehend von der ersten Instanz des Monats gezählt.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-188">Specifies on which instance of the allowed days specified in **daysOfsWeek** the event occurs, counted from the first instance in the month.</span></span> <span data-ttu-id="0a0dd-189">Mögliche Werte: `first`, `second`, `third`, `fourth` und `last`.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-189">Possible values: `first`, `second`, `third`, `fourth`, and `last`.</span></span> <span data-ttu-id="0a0dd-190">Standardwert: `first`.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-190">Default value: `first`.</span></span> |
| <span data-ttu-id="0a0dd-191">**Intervall**</span><span class="sxs-lookup"><span data-stu-id="0a0dd-191">**interval**</span></span> | <span data-ttu-id="0a0dd-192">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="0a0dd-192">Required</span></span> | <span data-ttu-id="0a0dd-193">Gibt die Anzahl der Monate zwischen zwei Vorkommen an.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-193">Specifies the number of months between each occurrence.</span></span> |
| <span data-ttu-id="0a0dd-194">**Typ**</span><span class="sxs-lookup"><span data-stu-id="0a0dd-194">**type**</span></span> | <span data-ttu-id="0a0dd-195">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="0a0dd-195">Required</span></span> | <span data-ttu-id="0a0dd-196">Muss auf `relativeMonthly` festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-196">Must be set to `relativeMonthly`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="0a0dd-197">Beispiele</span><span class="sxs-lookup"><span data-stu-id="0a0dd-197">Examples</span></span>

- <span data-ttu-id="0a0dd-198">Dieses Ereignis jeden zweiten Mittwoch des Monats wiederholen</span><span class="sxs-lookup"><span data-stu-id="0a0dd-198">Repeat this event on the second Wednesday of every month</span></span>

  ```json
    "pattern": {
      "type": "relativeMonthly",
      "interval": 1,
      "daysOfWeek": [ "Wednesday" ],
      "index": "second"
    }
  ```
- <span data-ttu-id="0a0dd-199">Dieses Ereignis jeden zweiten Mittwoch des Monats wiederholen</span><span class="sxs-lookup"><span data-stu-id="0a0dd-199">Repeat this event on the first Thursday or Friday of every month</span></span>

  ```json
    "pattern": {
      "type": "relativeMonthly",
      "interval": 1,
      "daysOfWeek": [ "Thursday", "Friday" ],
      "index": "first"
    }
  ```

### <a name="absolute-yearly"></a><span data-ttu-id="0a0dd-200">Absolut jährlich</span><span class="sxs-lookup"><span data-stu-id="0a0dd-200">Absolute yearly</span></span>

<span data-ttu-id="0a0dd-201">Das absolut jährliche Muster bewirkt, dass ein Ereignis am gleichen Tag und im gleichen Monat (z. B. dem 15. April), basierend auf der Anzahl der Jahre zwischen zwei Vorkommen stattfindet.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-201">The absolute yearly pattern causes an event to repeat on the same month and day (for example, April 15), based on the number of years between each occurrence.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="0a0dd-202">Relevante Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0a0dd-202">Relevant properties</span></span>

| <span data-ttu-id="0a0dd-203">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0a0dd-203">Property</span></span> | <span data-ttu-id="0a0dd-204">Relevanz</span><span class="sxs-lookup"><span data-stu-id="0a0dd-204">Relevance</span></span> | <span data-ttu-id="0a0dd-205">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0a0dd-205">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="0a0dd-206">**dayOfMonth**</span><span class="sxs-lookup"><span data-stu-id="0a0dd-206">**dayOfMonth**</span></span> | <span data-ttu-id="0a0dd-207">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="0a0dd-207">Required</span></span> | <span data-ttu-id="0a0dd-208">Gibt an, an welchem Tag des Monats das Ereignis eintritt.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-208">Specifies on which day of the month the event occurs.</span></span> |
| <span data-ttu-id="0a0dd-209">**Monat**</span><span class="sxs-lookup"><span data-stu-id="0a0dd-209">**month**</span></span> | <span data-ttu-id="0a0dd-210">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="0a0dd-210">Required</span></span> | <span data-ttu-id="0a0dd-211">Gibt an, in welchem Monat das Ereignis auftritt.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-211">Specifies in which month the event occurs.</span></span> |
| <span data-ttu-id="0a0dd-212">**Intervall**</span><span class="sxs-lookup"><span data-stu-id="0a0dd-212">**interval**</span></span> | <span data-ttu-id="0a0dd-213">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="0a0dd-213">Required</span></span> | <span data-ttu-id="0a0dd-214">Gibt die Anzahl der Jahre zwischen zwei Vorkommen an.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-214">Specifies the number of years between each occurrence.</span></span> |
| <span data-ttu-id="0a0dd-215">**Typ**</span><span class="sxs-lookup"><span data-stu-id="0a0dd-215">**type**</span></span> | <span data-ttu-id="0a0dd-216">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="0a0dd-216">Required</span></span> | <span data-ttu-id="0a0dd-217">Muss auf `absoluteYearly` festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-217">Must be set to `absoluteYearly`.</span></span> |

#### <a name="example"></a><span data-ttu-id="0a0dd-218">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0a0dd-218">Example</span></span>

- <span data-ttu-id="0a0dd-219">Dieses Ereignis jedes Jahr am 15. April wiederholen</span><span class="sxs-lookup"><span data-stu-id="0a0dd-219">Repeat this event on April 15 every year</span></span>

  ```json
    "pattern": {
      "type": "absoluteYearly",
      "interval": 1,
      "dayOfMonth": 15,
      "month": 4
    }
  ```

### <a name="relative-yearly"></a><span data-ttu-id="0a0dd-220">Relativ jährlich</span><span class="sxs-lookup"><span data-stu-id="0a0dd-220">Relative yearly</span></span>

<span data-ttu-id="0a0dd-221">Das relative jährliche Muster bewirkt, dass ein Ereignis am gleichen Wochentag an der gleichen relativen Position eines bestimmten Monats basierend auf der Anzahl der Jahre zwischen zwei Vorkommen stattfindet.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-221">The relative yearly pattern causes an event to repeat on the same day of the week in the same relative position in a specific month, based on the number of years between each occurrence.</span></span> <span data-ttu-id="0a0dd-222">Beispielsweise „jeden letzten Mittwoch im November“.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-222">For example, "every last Wednesday of November."</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="0a0dd-223">Relevante Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0a0dd-223">Relevant properties</span></span>

| <span data-ttu-id="0a0dd-224">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0a0dd-224">Property</span></span> | <span data-ttu-id="0a0dd-225">Relevanz</span><span class="sxs-lookup"><span data-stu-id="0a0dd-225">Relevance</span></span> | <span data-ttu-id="0a0dd-226">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0a0dd-226">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="0a0dd-227">**daysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="0a0dd-227">**daysOfWeek**</span></span> | <span data-ttu-id="0a0dd-228">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="0a0dd-228">Required</span></span> | <span data-ttu-id="0a0dd-229">Gibt an, an welchem/-n Tag/-en der Woche das Ereignis eintreten kann.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-229">Specifies on which day(s) of the week the event can occur.</span></span> <span data-ttu-id="0a0dd-230">Relative jährliche Ereignisse treten nur einmal pro Jahr ein, wird also mehr als ein Wert angegeben, fällt das Ereignis auf den ersten Tag, der das Muster erfüllt.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-230">Relative yearly events only occur once per year, so if more than one value is specified, the event falls on the first day that satisfies the pattern.</span></span> |
| <span data-ttu-id="0a0dd-231">**Index**</span><span class="sxs-lookup"><span data-stu-id="0a0dd-231">**index**</span></span> | <span data-ttu-id="0a0dd-232">Optional</span><span class="sxs-lookup"><span data-stu-id="0a0dd-232">Optional</span></span> | <span data-ttu-id="0a0dd-233">Gibt an, in welcher Instanz der zulässigen Tage, die unter **daysOfsWeek** angegeben sind, das Ereignis eintritt, ausgehend von der ersten Instanz des Monats gezählt.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-233">Specifies on which instance of the allowed days specified in **daysOfsWeek** the event occurs, counted from the first instance in the month.</span></span> <span data-ttu-id="0a0dd-234">Mögliche Werte: `first`, `second`, `third`, `fourth` und `last`.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-234">Possible values: `first`, `second`, `third`, `fourth`, and `last`.</span></span> <span data-ttu-id="0a0dd-235">Standardwert: `first`.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-235">Default value: `first`.</span></span> |
| <span data-ttu-id="0a0dd-236">**Monat**</span><span class="sxs-lookup"><span data-stu-id="0a0dd-236">**month**</span></span> | <span data-ttu-id="0a0dd-237">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="0a0dd-237">Required</span></span> | <span data-ttu-id="0a0dd-238">Gibt an, in welchem Monat das Ereignis auftritt.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-238">Specifies in which month the event occurs.</span></span> |
| <span data-ttu-id="0a0dd-239">**Intervall**</span><span class="sxs-lookup"><span data-stu-id="0a0dd-239">**interval**</span></span> | <span data-ttu-id="0a0dd-240">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="0a0dd-240">Required</span></span> | <span data-ttu-id="0a0dd-241">Gibt die Anzahl der Jahre zwischen zwei Vorkommen an.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-241">Specifies the number of years between each occurrence.</span></span> |
| <span data-ttu-id="0a0dd-242">**Typ**</span><span class="sxs-lookup"><span data-stu-id="0a0dd-242">**type**</span></span> | <span data-ttu-id="0a0dd-243">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="0a0dd-243">Required</span></span> | <span data-ttu-id="0a0dd-244">Muss auf `relativeMonthly` festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-244">Must be set to `relativeMonthly`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="0a0dd-245">Beispiele</span><span class="sxs-lookup"><span data-stu-id="0a0dd-245">Examples</span></span>

- <span data-ttu-id="0a0dd-246">Dieses Ereignis jedes Jahr am letzten Mittwoch im November wiederholen</span><span class="sxs-lookup"><span data-stu-id="0a0dd-246">Repeat this event on the last Wednesday of November every year</span></span>

  ```json
    "pattern": {
      "type": "relativeYearly",
      "interval": 1,
      "daysOfWeek": [ "Wednesday" ],
      "index": "last",
      "month": 11
    }
  ```

## <a name="recurrence-ranges"></a><span data-ttu-id="0a0dd-247">Serienbereiche</span><span class="sxs-lookup"><span data-stu-id="0a0dd-247">Recurrence ranges</span></span>

<span data-ttu-id="0a0dd-248">Der zweite Teil einer Serie ist das Muster.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-248">The second part of a recurrence is the range.</span></span> <span data-ttu-id="0a0dd-249">Dies gibt an, wie lange das Muster wiederholt wird.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-249">This specifies how long the pattern repeats.</span></span> <span data-ttu-id="0a0dd-250">Ein Ereignis könnte beispielsweise nach 10 Vorkommen an einem bestimmten Datum enden oder kein Ende haben.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-250">For example, an event could end after 10 occurrences, by a specific date, or could have no end.</span></span> <span data-ttu-id="0a0dd-251">Ein Bereich wird in der API durch die [recurrenceRange-Ressource](/graph/api/resources/recurrencepattern?view=graph-rest-1.0) dargestellt.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-251">A range is represented in the API by the [recurrenceRange resource](/graph/api/resources/recurrencepattern?view=graph-rest-1.0).</span></span>

<span data-ttu-id="0a0dd-252">Je nach Bereichstyp sind bestimmte Felder der **recurrenceRange** obligatorisch oder werden ignoriert.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-252">Depending on the type of range, certain fields of **recurrenceRange** are required or ignored.</span></span>

> <span data-ttu-id="0a0dd-253">**Hinweis:** Auch wenn ein Feld ignoriert wird, wird es dennoch überprüft.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-253">**Note**: Even if a field is ignored, it is still validated.</span></span> <span data-ttu-id="0a0dd-254">Wenn ein Feld über eine festgelegte Liste möglicher Werte verfügt, führt ein Wert außerhalb der zulässigen Gruppe von Werten zu einem Fehler, selbst wenn das Feld ignoriert wird.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-254">If a field has a set list of possible values, using a value outside the allowed set causes an error, even if that field is ignored.</span></span>

<span data-ttu-id="0a0dd-255">Werfen wir einen Blick auf die einzelnen Arten möglicher Bereiche.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-255">Let's take a look at each of the possible range types.</span></span>

### <a name="numbered-range"></a><span data-ttu-id="0a0dd-256">Nummerierter Bereich</span><span class="sxs-lookup"><span data-stu-id="0a0dd-256">Numbered range</span></span>

<span data-ttu-id="0a0dd-257">Der nummerierte Bereich bewirkt, dass ein Ereignis eine feste Anzahl von Vorkommen (basierend auf dem Muster) ab einem Startdatum auftritt.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-257">The numbered range causes an event to occur a fixed number of times (based on the pattern) from a start date.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="0a0dd-258">Relevante Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0a0dd-258">Relevant properties</span></span>

| <span data-ttu-id="0a0dd-259">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0a0dd-259">Property</span></span> | <span data-ttu-id="0a0dd-260">Relevanz</span><span class="sxs-lookup"><span data-stu-id="0a0dd-260">Relevance</span></span> | <span data-ttu-id="0a0dd-261">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0a0dd-261">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="0a0dd-262">**numberOfOccurences**</span><span class="sxs-lookup"><span data-stu-id="0a0dd-262">**numberOfOccurences**</span></span> | <span data-ttu-id="0a0dd-263">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="0a0dd-263">Required</span></span> | <span data-ttu-id="0a0dd-264">Gibt die Anzahl von Vorkommen an.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-264">Specifies the number of occurrences.</span></span> <span data-ttu-id="0a0dd-265">Das Vorkommen muss eine positive ganze Zahl sein.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-265">Must be a positive integer.</span></span> |
| <span data-ttu-id="0a0dd-266">**recurrenceTimeZone**</span><span class="sxs-lookup"><span data-stu-id="0a0dd-266">**recurrenceTimeZone**</span></span> | <span data-ttu-id="0a0dd-267">Optional</span><span class="sxs-lookup"><span data-stu-id="0a0dd-267">Optional</span></span> | <span data-ttu-id="0a0dd-268">Gibt die Zeitzone für die **StartDate**-Eigenschaft an.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-268">Specifies the time zone for the **startDate** property.</span></span> <span data-ttu-id="0a0dd-269">Falls nicht angegeben, wird die Zeitzone des Ereignisses verwendet.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-269">If not specified, the time zone of the event is used.</span></span> |
| <span data-ttu-id="0a0dd-270">**startDate**</span><span class="sxs-lookup"><span data-stu-id="0a0dd-270">**startDate**</span></span> | <span data-ttu-id="0a0dd-271">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="0a0dd-271">Required</span></span> | <span data-ttu-id="0a0dd-272">Gibt das Datum des Starts des Anwendens des Musters an.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-272">Specifies the date to start applying the pattern.</span></span> <span data-ttu-id="0a0dd-273">Der Wert von **StartDate** MUSS dem Datumswert der **Start**-Eigenschaft der [Ereignisressource](/graph/api/resources/event?view=graph-rest-1.0) entsprechen.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-273">The value of **startDate** MUST correspond to the date value of the **start** property on the [event resource](/graph/api/resources/event?view=graph-rest-1.0).</span></span> <span data-ttu-id="0a0dd-274">Hinweis: Das erste Vorkommen der Besprechung kann nicht an diesem Datum stattfinden, wenn es nicht in das Muster passt.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-274">Note that the first occurrence of the meeting may not occur on this date if it does not fit the pattern.</span></span> |
| <span data-ttu-id="0a0dd-275">**Typ**</span><span class="sxs-lookup"><span data-stu-id="0a0dd-275">**type**</span></span> | <span data-ttu-id="0a0dd-276">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="0a0dd-276">Required</span></span> | <span data-ttu-id="0a0dd-277">Muss auf `numbered` festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-277">Must be set to `numbered`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="0a0dd-278">Beispiele</span><span class="sxs-lookup"><span data-stu-id="0a0dd-278">Examples</span></span>

- <span data-ttu-id="0a0dd-279">Dieses Ereignis 10 Mal wiederholen</span><span class="sxs-lookup"><span data-stu-id="0a0dd-279">Repeat this event 10 times</span></span>

  ```json
    "range": {
      "type": "numbered",
      "startDate": "2017-04-02",
      "numberOfOccurrences": 10
    }
  ```

### <a name="end-date-range"></a><span data-ttu-id="0a0dd-280">Enddatumsbereich</span><span class="sxs-lookup"><span data-stu-id="0a0dd-280">End date range</span></span>

<span data-ttu-id="0a0dd-281">Der Enddatumsbereich bewirkt, dass ein Ereignis an allen Tagen eintritt, die das entsprechende Muster zwischen einem Startdatum und einem Enddatum aufweisen.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-281">The end date range causes an event to occur on all days that fit the applicable pattern between a start date and an end date.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="0a0dd-282">Relevante Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0a0dd-282">Relevant properties</span></span>

| <span data-ttu-id="0a0dd-283">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0a0dd-283">Property</span></span> | <span data-ttu-id="0a0dd-284">Relevanz</span><span class="sxs-lookup"><span data-stu-id="0a0dd-284">Relevance</span></span> | <span data-ttu-id="0a0dd-285">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0a0dd-285">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="0a0dd-286">**endDate**</span><span class="sxs-lookup"><span data-stu-id="0a0dd-286">**endDate**</span></span> | <span data-ttu-id="0a0dd-287">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="0a0dd-287">Required</span></span> | <span data-ttu-id="0a0dd-288">Gibt das Datum zum Beenden des Anwendens des Musters an.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-288">Specifies the date to stop applying the pattern.</span></span> <span data-ttu-id="0a0dd-289">Hinweis: Das letzte Vorkommen der Besprechung kann nicht an diesem Datum auftreten, wenn es nicht in das Muster passt.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-289">Note that the last occurrence of the meeting may not occur on this date if it does not fit the pattern.</span></span> |
| <span data-ttu-id="0a0dd-290">**recurrenceTimeZone**</span><span class="sxs-lookup"><span data-stu-id="0a0dd-290">**recurrenceTimeZone**</span></span> | <span data-ttu-id="0a0dd-291">Optional</span><span class="sxs-lookup"><span data-stu-id="0a0dd-291">Optional</span></span> | <span data-ttu-id="0a0dd-292">Gibt die Zeitzone für die **startDate**- und **endDate**-Eigenschaften an.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-292">Specifies the time zone for the **startDate** and **endDate** properties.</span></span> <span data-ttu-id="0a0dd-293">Falls nicht angegeben, wird die Zeitzone des Ereignisses verwendet.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-293">If not specified, the time zone of the event is used.</span></span> |
| <span data-ttu-id="0a0dd-294">**startDate**</span><span class="sxs-lookup"><span data-stu-id="0a0dd-294">**startDate**</span></span> | <span data-ttu-id="0a0dd-295">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="0a0dd-295">Required</span></span> | <span data-ttu-id="0a0dd-296">Gibt das Datum des Starts des Anwendens des Musters an.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-296">Specifies the date to start applying the pattern.</span></span> <span data-ttu-id="0a0dd-297">Der Wert von **StartDate** MUSS dem Datumswert der **Start**-Eigenschaft der [Ereignisressource](/graph/api/resources/event?view=graph-rest-1.0) entsprechen.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-297">The value of **startDate** MUST correspond to the date value of the **start** property on the [event resource](/graph/api/resources/event?view=graph-rest-1.0).</span></span> <span data-ttu-id="0a0dd-298">Hinweis: Das erste Vorkommen der Besprechung kann nicht an diesem Datum stattfinden, wenn es nicht in das Muster passt.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-298">Note that the first occurrence of the meeting may not occur on this date if it does not fit the pattern.</span></span> |
| <span data-ttu-id="0a0dd-299">**Typ**</span><span class="sxs-lookup"><span data-stu-id="0a0dd-299">**type**</span></span> | <span data-ttu-id="0a0dd-300">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="0a0dd-300">Required</span></span> | <span data-ttu-id="0a0dd-301">Muss auf **EndDate** festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-301">Must be set to **endDate**.</span></span> |

#### <a name="examples"></a><span data-ttu-id="0a0dd-302">Beispiele</span><span class="sxs-lookup"><span data-stu-id="0a0dd-302">Examples</span></span>

- <span data-ttu-id="0a0dd-303">Dieses Ereignis vom 1. Juli 2017 bis zum 31. Juli 2017 wiederholen</span><span class="sxs-lookup"><span data-stu-id="0a0dd-303">Repeat this event from July 1, 2017, to July 31, 2017</span></span>

  ```json
    "range": {
      "type": "endDate",
      "startDate": "2017-07-01",
      "endDate": "2017-07-31"
    }
  ```

### <a name="no-end-range"></a><span data-ttu-id="0a0dd-304">Kein Endbereich</span><span class="sxs-lookup"><span data-stu-id="0a0dd-304">No end range</span></span>

<span data-ttu-id="0a0dd-305">Der Enddatumsbereich bewirkt, dass ein Ereignis an allen Tagen eintritt, die dem anwendbaren Muster nach einem Startdatum entsprechen.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-305">The no end range causes an event to occur on all days that fit the applicable pattern after a start date.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="0a0dd-306">Relevante Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0a0dd-306">Relevant properties</span></span>

| <span data-ttu-id="0a0dd-307">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0a0dd-307">Property</span></span> | <span data-ttu-id="0a0dd-308">Relevanz</span><span class="sxs-lookup"><span data-stu-id="0a0dd-308">Relevance</span></span> | <span data-ttu-id="0a0dd-309">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0a0dd-309">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="0a0dd-310">**recurrenceTimeZone**</span><span class="sxs-lookup"><span data-stu-id="0a0dd-310">**recurrenceTimeZone**</span></span> | <span data-ttu-id="0a0dd-311">Optional</span><span class="sxs-lookup"><span data-stu-id="0a0dd-311">Optional</span></span> | <span data-ttu-id="0a0dd-312">Gibt die Zeitzone für die **StartDate**-Eigenschaft an.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-312">Specifies the time zone for the **startDate** property.</span></span> <span data-ttu-id="0a0dd-313">Falls nicht angegeben, wird die Zeitzone des Ereignisses verwendet.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-313">If not specified, the time zone of the event is used.</span></span> |
| <span data-ttu-id="0a0dd-314">**startDate**</span><span class="sxs-lookup"><span data-stu-id="0a0dd-314">**startDate**</span></span> | <span data-ttu-id="0a0dd-315">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="0a0dd-315">Required</span></span> | <span data-ttu-id="0a0dd-316">Gibt das Datum des Starts des Anwendens des Musters an.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-316">Specifies the date to start applying the pattern.</span></span> <span data-ttu-id="0a0dd-317">Der Wert von **StartDate** MUSS dem Datumswert der **Start**-Eigenschaft der [Ereignisressource](/graph/api/resources/event?view=graph-rest-1.0) entsprechen.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-317">The value of **startDate** MUST correspond to the date value of the **start** property on the [event resource](/graph/api/resources/event?view=graph-rest-1.0).</span></span> <span data-ttu-id="0a0dd-318">Hinweis: Das erste Vorkommen der Besprechung kann nicht an diesem Datum stattfinden, wenn es nicht in das Muster passt.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-318">Note that the first occurrence of the meeting may not occur on this date if it does not fit the pattern.</span></span> |
| <span data-ttu-id="0a0dd-319">**Typ**</span><span class="sxs-lookup"><span data-stu-id="0a0dd-319">**type**</span></span> | <span data-ttu-id="0a0dd-320">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="0a0dd-320">Required</span></span> | <span data-ttu-id="0a0dd-321">Muss auf `noEnd` festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-321">Must be set to `noEnd`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="0a0dd-322">Beispiele</span><span class="sxs-lookup"><span data-stu-id="0a0dd-322">Examples</span></span>

- <span data-ttu-id="0a0dd-323">Dieses Ereignis ab dem 15. Mai 2017 immer wiederholen</span><span class="sxs-lookup"><span data-stu-id="0a0dd-323">Repeat this event from May 15, 2017, forever</span></span>

  ```json
    "range": {
      "type": "noEnd",
      "startDate": "2017-05-15"
    }
  ```

## <a name="using-patterns-and-ranges-to-create-recurring-events"></a><span data-ttu-id="0a0dd-324">Verwenden von Mustern und Bereichen zum Erstellen von Ereignisserien</span><span class="sxs-lookup"><span data-stu-id="0a0dd-324">Using patterns and ranges to create recurring events</span></span>

<span data-ttu-id="0a0dd-325">Nachdem wir uns nun Muster und Bereiche separat angesehen haben, schauen wir uns nun deren Zusammenwirken und Interagieren mit den **Start**- und **End**-Eigenschaften zu dem Ereignis an.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-325">Now that we've looked at patterns and ranges separately, let's look at how they work together and how they interact with the **start** and **end** properties on the event.</span></span>

### <a name="creating-a-recurrence-rule"></a><span data-ttu-id="0a0dd-326">Erstellen einer Serienregel</span><span class="sxs-lookup"><span data-stu-id="0a0dd-326">Creating a recurrence rule</span></span>

<span data-ttu-id="0a0dd-327">Um eine Serienregel zu erstellen, müssen Sie sowohl ein Muster als auch einen Bereich angeben.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-327">To create a recurrence rule, you must specify both a pattern and a range.</span></span> <span data-ttu-id="0a0dd-328">Jeder Mustertyp kann mit einem beliebigen Bereichstyp arbeiten.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-328">Any pattern type can work with any range type.</span></span> <span data-ttu-id="0a0dd-329">Im Anschluss finden Sie einige Beispiele:</span><span class="sxs-lookup"><span data-stu-id="0a0dd-329">Here are a few examples.</span></span>

#### <a name="examples"></a><span data-ttu-id="0a0dd-330">Beispiele</span><span class="sxs-lookup"><span data-stu-id="0a0dd-330">Examples</span></span>

- <span data-ttu-id="0a0dd-331">**Besprechung von 13:00-13:30 Uhr, jeden Montag ab dem 4. September 2017 bis zum Ende des Jahres**</span><span class="sxs-lookup"><span data-stu-id="0a0dd-331">**Meet from 1:00 PM to 1:30 PM every Monday starting September 4, 2017, until the end of the year**</span></span>

  - <span data-ttu-id="0a0dd-332">Die Anforderung „jeden Montag“ wird ganz einfach durch den `weekly`-Serienmustertyp erfüllt.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-332">The "every Monday" requirement is easily met by the `weekly` recurrence pattern type.</span></span>
  - <span data-ttu-id="0a0dd-333">Die Anforderung „bis zum Ende des Jahres“ gibt einen `endDate`-Serienbereichstypen an.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-333">The "until the end of the year" requirement indicates an `endDate` recurrence range type.</span></span>

  ```json
    "recurrence": {
      "pattern": {
        "type": "weekly",
        "interval": 1,
        "daysOfWeek": [ "Monday" ]
      },
      "range": {
        "type": "endDate",
        "startDate": "2017-09-04",
        "endDate": "2017-12-31"
      }
    }
  ```

  <span data-ttu-id="0a0dd-334">Da der 31. Dezember 2017 auf einen Sonntag fällt, ist das letzte Vorkommen in dieser Serie am Montag, den 25. Dezember.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-334">Because December 31, 2017, is on a Sunday, the last occurrence in this series will be on Monday, December 25.</span></span>

- <span data-ttu-id="0a0dd-335">**Besprechung von 14:00-15:00 Uhr am ersten Donnerstag jeden zweiten Monat, ab dem 29. August 2017**</span><span class="sxs-lookup"><span data-stu-id="0a0dd-335">**Meet from 2:00 PM to 3:00 PM on the first Thursday of every other month starting August 29, 2017**</span></span>

  - <span data-ttu-id="0a0dd-336">Die Anforderung „erster Donnerstag jeden zweiten Monat“ kann durch ein relatives monatliches Muster erfüllt werden.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-336">The "first Thursday of every other month" requirement is achievable by using a relative monthly pattern.</span></span> <span data-ttu-id="0a0dd-337">Der Teil „jeden zweiten Monats“ gibt an, dass das **Intervall** auf `2` festgelegt werden sollte.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-337">The "every other month" portion indicates that the **interval** should be set to `2`.</span></span>
  - <span data-ttu-id="0a0dd-338">Da es keine Anforderung an ein Enddatum gibt, kann ein `noEnd`-Bereichstyp verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-338">Because there is no requirement on an end date, a `noEnd` range type can be used.</span></span>

  ```json
    "recurrence": {
      "pattern": {
        "type": "relativeMonthly",
        "interval": 2,
        "daysOfWeek": [ "Thursday" ],
        "index": "first"
      },
      "range": {
        "type": "noEnd",
        "startDate": "2017-08-29"
      }
    }
  ```

  <span data-ttu-id="0a0dd-339">Da der Wert von **startDate** nach dem ersten Donnerstag im August liegt, ist das erste Vorkommen dieser Serie im September.</span><span class="sxs-lookup"><span data-stu-id="0a0dd-339">Because the value of **startDate** is after the first Thursday in August, the first occurrence of this series will be in September.</span></span>

## <a name="next-steps"></a><span data-ttu-id="0a0dd-340">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="0a0dd-340">Next steps</span></span>
    
<span data-ttu-id="0a0dd-341">Erfahren Sie mehr zur [Integration in Outlook-Kalender](outlook-calendar-concept-overview.md).</span><span class="sxs-lookup"><span data-stu-id="0a0dd-341">Find out more about [integrating with Outlook calendar](outlook-calendar-concept-overview.md).</span></span>
