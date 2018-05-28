# <a name="schedule-repeating-appointments-as-recurring-events-in-outlook"></a><span data-ttu-id="bc46c-101">Planen wiederkehrender Termine als wiederkehrende Ereignisse in Outlook</span><span class="sxs-lookup"><span data-stu-id="bc46c-101">Schedule repeating appointments as recurring events in Outlook</span></span>

<span data-ttu-id="bc46c-102">Ereignisserien sind ein wichtiger Bestandteil der Kalenderfunktionen von Outlook.</span><span class="sxs-lookup"><span data-stu-id="bc46c-102">Recurring events are an important part of Outlook calendaring.</span></span> <span data-ttu-id="bc46c-103">Ganz gleich, ob es sich um eine wöchentliche Besprechung mit Ihrem Vorgesetzten oder eine Abteilungsbesprechung handelt, die jeden zweiten Dienstag im Monat stattfindet, mit Ereignisserien können Sie ganz einfach eine Ereignisserie erstellen und der Server füllt den Kalender mit dem Rest der Serie.</span><span class="sxs-lookup"><span data-stu-id="bc46c-103">Whether it's a weekly one-on-one meeting with your manager, or a division-wide review meeting that happens on the second Tuesday of each month, recurring events make it easy to create the event once, and let the server fill in the rest of the series.</span></span>

<span data-ttu-id="bc46c-104">Die wichtigsten Informationen, mit denen Ereignisserien in einzelne Termine „erweitert“ werden können, die Serienregel.</span><span class="sxs-lookup"><span data-stu-id="bc46c-104">The key bit of information that allows recurring events to "expand" into individual occurrences is the recurrence rule.</span></span> <span data-ttu-id="bc46c-105">In der Serie ist die Wiederholungsfrequenz und Dauer eines Ereignisses angegeben.</span><span class="sxs-lookup"><span data-stu-id="bc46c-105">The rule specifies both how often an event repeats, and for how long.</span></span> <span data-ttu-id="bc46c-106">Die Outlook-REST-APIs modellieren Serienregeln in der **Serien**-Eigenschaft der [Ereignisressource](../api-reference/v1.0/resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="bc46c-106">The Outlook REST APIs model recurrence rules in the **** property of the [event resource](../api-reference/v1.0/resources/event.md).</span></span> 

<span data-ttu-id="bc46c-107">Jede Serie besteht aus zwei Teilen: dem Serienmuster (wie oft) und dem Serienbereich (für wie lange).</span><span class="sxs-lookup"><span data-stu-id="bc46c-107">Each  is made up of two parts: the recurrence pattern (how often), and the recurrence range (for how long).</span></span>

## <a name="recurrence-patterns"></a><span data-ttu-id="bc46c-108">Serienmuster</span><span class="sxs-lookup"><span data-stu-id="bc46c-108">Recurrence patterns</span></span>

<span data-ttu-id="bc46c-109">Der erste Teil einer Serie ist das Muster.</span><span class="sxs-lookup"><span data-stu-id="bc46c-109">The first part of a recurrence is the pattern.</span></span> <span data-ttu-id="bc46c-110">Darin ist angegeben, wie oft das Ereignis wiederholt wird.</span><span class="sxs-lookup"><span data-stu-id="bc46c-110">This specifies how often the event repeats.</span></span> <span data-ttu-id="bc46c-111">Beispielsweise könnte ein Ereignis „alle 3 Tage“, „jeden Donnerstag“ oder „jedes Jahr am 22. Juli“ wiederholt werden.</span><span class="sxs-lookup"><span data-stu-id="bc46c-111">For example, an event could repeat "every 3 days", "every Thursday", or "on July 22 every year".</span></span> <span data-ttu-id="bc46c-112">Ein Muster wird in der API durch die [recurrencePattern-Ressource](../api-reference/v1.0/resources/recurrencepattern.md) dargestellt.</span><span class="sxs-lookup"><span data-stu-id="bc46c-112">A pattern is represented in the API by the [recurrencePattern resource](../api-reference/v1.0/resources/recurrencepattern.md).</span></span>

<span data-ttu-id="bc46c-113">Je nach Mustertyp sind bestimmte Felder des **recurrencePattern** obligatorisch, optional oder werden ignoriert.</span><span class="sxs-lookup"><span data-stu-id="bc46c-113">Depending on the type of pattern, certain fields of the **** are required, optional, or ignored.</span></span>

> <span data-ttu-id="bc46c-114">**Hinweis:** Auch wenn ein Feld ignoriert wird, wird es dennoch überprüft.</span><span class="sxs-lookup"><span data-stu-id="bc46c-114">Even if a field is ignored, it is still validated.</span></span> <span data-ttu-id="bc46c-115">Wenn ein Feld über eine festgelegte Liste möglicher Werte verfügt, führt ein Wert außerhalb der zulässigen Gruppe von Werten zu einem Fehler, selbst wenn das Feld ignoriert wird.</span><span class="sxs-lookup"><span data-stu-id="bc46c-115">If a field has a set list of possible values, using a value outside the allowed set will cause an error, even if that field is ignored.</span></span>

<span data-ttu-id="bc46c-116">Werfen Sie einen Blick auf die einzelnen Arten möglicher Muster.</span><span class="sxs-lookup"><span data-stu-id="bc46c-116">Let's take a look at each of the possible pattern types.</span></span>

### <a name="daily"></a><span data-ttu-id="bc46c-117">Täglich</span><span class="sxs-lookup"><span data-stu-id="bc46c-117">Daily</span></span>

<span data-ttu-id="bc46c-118">Das tägliche Serienmuster bewirkt, dass ein Ereignis basierend auf einer Anzahl von Tagen zwischen zwei Vorkommen wiederholt wird.</span><span class="sxs-lookup"><span data-stu-id="bc46c-118">The daily recurrence pattern causes an event to repeat based on a number of days between each occurrence.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="bc46c-119">Relevante Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bc46c-119">Relevant properties</span></span>

| <span data-ttu-id="bc46c-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bc46c-120">Property</span></span> | <span data-ttu-id="bc46c-121">Relevanz</span><span class="sxs-lookup"><span data-stu-id="bc46c-121">Relevance</span></span> | <span data-ttu-id="bc46c-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bc46c-122">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="bc46c-123">**Intervall**</span><span class="sxs-lookup"><span data-stu-id="bc46c-123">**interval**</span></span> | <span data-ttu-id="bc46c-124">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="bc46c-124">Required</span></span> | <span data-ttu-id="bc46c-125">Gibt die Anzahl der Tage zwischen zwei Vorkommen an.</span><span class="sxs-lookup"><span data-stu-id="bc46c-125">Specifies the number of days between each occurrence.</span></span> |
| <span data-ttu-id="bc46c-126">**Typ**</span><span class="sxs-lookup"><span data-stu-id="bc46c-126">**type**</span></span> | <span data-ttu-id="bc46c-127">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="bc46c-127">Required</span></span> | <span data-ttu-id="bc46c-128">Muss auf `daily` festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="bc46c-128">Must be set to `daily`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="bc46c-129">Beispiele</span><span class="sxs-lookup"><span data-stu-id="bc46c-129">Examples</span></span>

- <span data-ttu-id="bc46c-130">Dieses Ereignis täglich wiederholen</span><span class="sxs-lookup"><span data-stu-id="bc46c-130">Repeat this event every day</span></span>

  ```json
    "pattern": {
      "type": "daily",
      "interval": 1
    }
  ```
- <span data-ttu-id="bc46c-131">Dieses Ereignis alle drei Tage wiederholen</span><span class="sxs-lookup"><span data-stu-id="bc46c-131">Repeat this event every three days</span></span>

  ```json
    "pattern": {
      "type": "daily",
      "interval": 3
    }
  ```

### <a name="weekly"></a><span data-ttu-id="bc46c-132">Wöchentlich</span><span class="sxs-lookup"><span data-stu-id="bc46c-132">Weekly</span></span>

<span data-ttu-id="bc46c-133">Das wöchentliche Serienmuster bewirkt, dass ein Ereignis am gleichen Tag oder an den gleichen Tagen einer Woche basierend auf der Anzahl von Wochen zwischen zwei Vorkommen wiederholt wird.</span><span class="sxs-lookup"><span data-stu-id="bc46c-133">The weekly recurrence pattern causes an event to repeat on the same day or days of the week, based on the number of weeks between each set of occurrences.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="bc46c-134">Relevante Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bc46c-134">Relevant properties</span></span>

| <span data-ttu-id="bc46c-135">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bc46c-135">Property</span></span> | <span data-ttu-id="bc46c-136">Relevanz</span><span class="sxs-lookup"><span data-stu-id="bc46c-136">Relevance</span></span> | <span data-ttu-id="bc46c-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bc46c-137">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="bc46c-138">**daysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="bc46c-138">**daysOfWeek**</span></span> | <span data-ttu-id="bc46c-139">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="bc46c-139">Required</span></span> | <span data-ttu-id="bc46c-140">Gibt an, an welchem/-n Tag/-en der Woche das Ereignis eintritt.</span><span class="sxs-lookup"><span data-stu-id="bc46c-140">Specifies on which day(s) of the week the event occurs.</span></span> |
| <span data-ttu-id="bc46c-141">**firstDayOfWeek**</span><span class="sxs-lookup"><span data-stu-id="bc46c-141">**firstDayOfWeek**</span></span> | <span data-ttu-id="bc46c-142">Optional</span><span class="sxs-lookup"><span data-stu-id="bc46c-142">Optional</span></span> | <span data-ttu-id="bc46c-143">Gibt an, welcher Tag als erster Tag der Woche angesehen wird.</span><span class="sxs-lookup"><span data-stu-id="bc46c-143">Specifies which day is considered the first day of the week.</span></span> <span data-ttu-id="bc46c-144">Standardwert: `Sunday`.</span><span class="sxs-lookup"><span data-stu-id="bc46c-144">Default value: `Sunday`.</span></span> |
| <span data-ttu-id="bc46c-145">**Intervall**</span><span class="sxs-lookup"><span data-stu-id="bc46c-145">**interval**</span></span> | <span data-ttu-id="bc46c-146">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="bc46c-146">Required</span></span> | <span data-ttu-id="bc46c-147">Gibt die Anzahl der Wochen zwischen zwei Vorkommen an.</span><span class="sxs-lookup"><span data-stu-id="bc46c-147">Specifies the number of weeks between each set of occurrences.</span></span> |
| <span data-ttu-id="bc46c-148">**Typ**</span><span class="sxs-lookup"><span data-stu-id="bc46c-148">**type**</span></span> | <span data-ttu-id="bc46c-149">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="bc46c-149">Required</span></span> | <span data-ttu-id="bc46c-150">Muss auf `weekly` festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="bc46c-150">Must be set to `weekly`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="bc46c-151">Beispiele</span><span class="sxs-lookup"><span data-stu-id="bc46c-151">Examples</span></span>

- <span data-ttu-id="bc46c-152">Dieses Ereignis jeden Donnerstag wiederholen</span><span class="sxs-lookup"><span data-stu-id="bc46c-152">Repeat this event every Thursday</span></span>

  ```json
    "pattern": {
      "type": "weekly",
      "interval": 1,
      "daysOfWeek": [ "Thursday" ]
    }
  ```
- <span data-ttu-id="bc46c-153">Dieses Ereignis jeden Montag und Dienstag wiederholen</span><span class="sxs-lookup"><span data-stu-id="bc46c-153">Repeat this event every other Monday and Tuesday</span></span>

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

### <a name="absolute-monthly"></a><span data-ttu-id="bc46c-154">Absolut monatlich</span><span class="sxs-lookup"><span data-stu-id="bc46c-154">Absolute monthly</span></span>

<span data-ttu-id="bc46c-155">Das absolute monatliche Muster bewirkt, dass ein Ereignis am gleichen Tag des Monats (z. B. dem 15.) basierend auf der Anzahl der Monate zwischen zwei Vorkommen stattfindet.</span><span class="sxs-lookup"><span data-stu-id="bc46c-155">The absolute monthly pattern causes an event to repeat on the same day of the month (e.g. the 15th), based on the number of months between each occurrence.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="bc46c-156">Relevante Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bc46c-156">Relevant properties</span></span>

| <span data-ttu-id="bc46c-157">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bc46c-157">Property</span></span> | <span data-ttu-id="bc46c-158">Relevanz</span><span class="sxs-lookup"><span data-stu-id="bc46c-158">Relevance</span></span> | <span data-ttu-id="bc46c-159">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bc46c-159">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="bc46c-160">**dayOfMonth**</span><span class="sxs-lookup"><span data-stu-id="bc46c-160">**dayOfMonth**</span></span> | <span data-ttu-id="bc46c-161">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="bc46c-161">Required</span></span> | <span data-ttu-id="bc46c-162">Gibt an, an welchem Tag des Monats das Ereignis eintritt.</span><span class="sxs-lookup"><span data-stu-id="bc46c-162">Specifies on which day of the month the event occurs.</span></span> |
| <span data-ttu-id="bc46c-163">**Intervall**</span><span class="sxs-lookup"><span data-stu-id="bc46c-163">**interval**</span></span> | <span data-ttu-id="bc46c-164">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="bc46c-164">Required</span></span> | <span data-ttu-id="bc46c-165">Gibt die Anzahl der Monate zwischen zwei Vorkommen an.</span><span class="sxs-lookup"><span data-stu-id="bc46c-165">Specifies the number of months between each occurrence.</span></span> |
| <span data-ttu-id="bc46c-166">**Typ**</span><span class="sxs-lookup"><span data-stu-id="bc46c-166">**type**</span></span> | <span data-ttu-id="bc46c-167">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="bc46c-167">Required</span></span> | <span data-ttu-id="bc46c-168">Muss auf `absoluteMonthly` festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="bc46c-168">Must be set to `absoluteMonthly`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="bc46c-169">Beispiele</span><span class="sxs-lookup"><span data-stu-id="bc46c-169">Examples</span></span>

- <span data-ttu-id="bc46c-170">Dieses Ereignis jeden Monat am 15. wiederholen</span><span class="sxs-lookup"><span data-stu-id="bc46c-170">Repeat this event on the 15th of every month</span></span>

  ```json
    "pattern": {
      "type": "absoluteMonthly",
      "interval": 1,
      "dayOfMonth": 15
    }
  ```
- <span data-ttu-id="bc46c-171">Dieses Ereignis vierteljährlich (alle 3 Monate) am 7. wiederholen</span><span class="sxs-lookup"><span data-stu-id="bc46c-171">Repeat this event quarterly (every 3 months) on the 7th</span></span>

  ```json
    "pattern": {
      "type": "absoluteMonthly",
      "interval": 3,
      "dayOfMonth": 7
    }
  ```

### <a name="relative-monthly"></a><span data-ttu-id="bc46c-172">Relativ monatlich</span><span class="sxs-lookup"><span data-stu-id="bc46c-172">Relative monthly</span></span>

<span data-ttu-id="bc46c-173">Das relative monatliche Muster bewirkt, dass ein Ereignis am gleichen Wochentag an der gleichen relativen Position des Monats basierend auf der Anzahl der Monate zwischen zwei Vorkommen stattfindet.</span><span class="sxs-lookup"><span data-stu-id="bc46c-173">The relative monthly pattern causes an event to repeat on the same day of the week in the same relative position in the month, based on the number of months between each occurrence.</span></span> <span data-ttu-id="bc46c-174">Beispielsweise „jeden zweiten Mittwoch des Monats“.</span><span class="sxs-lookup"><span data-stu-id="bc46c-174">For example, "every second Wednesday of the month".</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="bc46c-175">Relevante Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bc46c-175">Relevant properties</span></span>

| <span data-ttu-id="bc46c-176">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bc46c-176">Property</span></span> | <span data-ttu-id="bc46c-177">Relevanz</span><span class="sxs-lookup"><span data-stu-id="bc46c-177">Relevance</span></span> | <span data-ttu-id="bc46c-178">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bc46c-178">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="bc46c-179">**daysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="bc46c-179">**daysOfWeek**</span></span> | <span data-ttu-id="bc46c-180">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="bc46c-180">Required</span></span> | <span data-ttu-id="bc46c-181">Gibt an, an welchem/-n Tag/-en der Woche das Ereignis eintreten kann.</span><span class="sxs-lookup"><span data-stu-id="bc46c-181">Specifies on which day(s) of the week the event can occur.</span></span> <span data-ttu-id="bc46c-182">Relative monatliche Ereignisse treten nur einmal pro Monat ein, wird also mehr als ein Wert angegeben, fällt das Ereignis auf den ersten Tag, der das Muster erfüllt.</span><span class="sxs-lookup"><span data-stu-id="bc46c-182">Relative monthly events only occur once per month, so if more than one value is specified, the event falls on the first day that satisfies the pattern.</span></span> |
| <span data-ttu-id="bc46c-183">**Index**</span><span class="sxs-lookup"><span data-stu-id="bc46c-183">**index**</span></span> | <span data-ttu-id="bc46c-184">Optional</span><span class="sxs-lookup"><span data-stu-id="bc46c-184">Optional</span></span> | <span data-ttu-id="bc46c-185">Gibt an, in welcher Instanz der zulässigen Tage, die unter **daysOfsWeek** angegeben sind, das Ereignis eintritt, ausgehend von der ersten Instanz des Monats gezählt.</span><span class="sxs-lookup"><span data-stu-id="bc46c-185">Specifies on which instance of the allowed days specified in **daysOfsWeek** the event occurs, counted from the first instance in the month.</span></span> <span data-ttu-id="bc46c-186">Mögliche Werte: `first`, `second`, `third`, `fourth` und `last`.</span><span class="sxs-lookup"><span data-stu-id="bc46c-186">Possible values: `first`, `second`, `third`, `fourth`, and `last`.</span></span> <span data-ttu-id="bc46c-187">Standardwert: `first`.</span><span class="sxs-lookup"><span data-stu-id="bc46c-187">Default value: `first`.</span></span> |
| <span data-ttu-id="bc46c-188">**Intervall**</span><span class="sxs-lookup"><span data-stu-id="bc46c-188">**interval**</span></span> | <span data-ttu-id="bc46c-189">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="bc46c-189">Required</span></span> | <span data-ttu-id="bc46c-190">Gibt die Anzahl der Monate zwischen zwei Vorkommen an.</span><span class="sxs-lookup"><span data-stu-id="bc46c-190">Specifies the number of months between each occurrence.</span></span> |
| <span data-ttu-id="bc46c-191">**Typ**</span><span class="sxs-lookup"><span data-stu-id="bc46c-191">**type**</span></span> | <span data-ttu-id="bc46c-192">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="bc46c-192">Required</span></span> | <span data-ttu-id="bc46c-193">Muss auf `relativeMonthly` festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="bc46c-193">Must be set to `relativeMonthly`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="bc46c-194">Beispiele</span><span class="sxs-lookup"><span data-stu-id="bc46c-194">Examples</span></span>

- <span data-ttu-id="bc46c-195">Dieses Ereignis jeden zweiten Mittwoch des Monats wiederholen</span><span class="sxs-lookup"><span data-stu-id="bc46c-195">Repeat this event on the second Wednesday of every month</span></span>

  ```json
    "pattern": {
      "type": "relativeMonthly",
      "interval": 1,
      "daysOfWeek": [ "Wednesday" ],
      "index": "second"
    }
  ```
- <span data-ttu-id="bc46c-196">Dieses Ereignis jeden zweiten Mittwoch des Monats wiederholen</span><span class="sxs-lookup"><span data-stu-id="bc46c-196">Repeat this event on the first Thursday or Friday of every month</span></span>

  ```json
    "pattern": {
      "type": "relativeMonthly",
      "interval": 1,
      "daysOfWeek": [ "Thursday", "Friday" ],
      "index": "first"
    }
  ```

### <a name="absolute-yearly"></a><span data-ttu-id="bc46c-197">Absolut jährlich</span><span class="sxs-lookup"><span data-stu-id="bc46c-197">Absolute yearly</span></span>

<span data-ttu-id="bc46c-198">Das absolut jährliche Muster bewirkt, dass ein Ereignis am gleichen Tag und im gleichen Monat (z. B. dem 15. April), basierend auf der Anzahl der Jahre zwischen zwei Vorkommen stattfindet.</span><span class="sxs-lookup"><span data-stu-id="bc46c-198">The absolute yearly pattern causes an event to repeat on the same month and day (e.g. April 15th), based on the number of years between each occurrence.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="bc46c-199">Relevante Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bc46c-199">Relevant properties</span></span>

| <span data-ttu-id="bc46c-200">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bc46c-200">Property</span></span> | <span data-ttu-id="bc46c-201">Relevanz</span><span class="sxs-lookup"><span data-stu-id="bc46c-201">Relevance</span></span> | <span data-ttu-id="bc46c-202">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bc46c-202">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="bc46c-203">**dayOfMonth**</span><span class="sxs-lookup"><span data-stu-id="bc46c-203">**dayOfMonth**</span></span> | <span data-ttu-id="bc46c-204">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="bc46c-204">Required</span></span> | <span data-ttu-id="bc46c-205">Gibt an, an welchem Tag des Monats das Ereignis eintritt.</span><span class="sxs-lookup"><span data-stu-id="bc46c-205">Specifies on which day of the month the event occurs.</span></span> |
| <span data-ttu-id="bc46c-206">**Monat**</span><span class="sxs-lookup"><span data-stu-id="bc46c-206">**month**</span></span> | <span data-ttu-id="bc46c-207">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="bc46c-207">Required</span></span> | <span data-ttu-id="bc46c-208">Gibt an, in welchem Monat das Ereignis auftritt.</span><span class="sxs-lookup"><span data-stu-id="bc46c-208">Specifies in which month the event occurs.</span></span> |
| <span data-ttu-id="bc46c-209">**Intervall**</span><span class="sxs-lookup"><span data-stu-id="bc46c-209">**interval**</span></span> | <span data-ttu-id="bc46c-210">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="bc46c-210">Required</span></span> | <span data-ttu-id="bc46c-211">Gibt die Anzahl der Jahre zwischen zwei Vorkommen an.</span><span class="sxs-lookup"><span data-stu-id="bc46c-211">Specifies the number of years between each occurrence.</span></span> |
| <span data-ttu-id="bc46c-212">**Typ**</span><span class="sxs-lookup"><span data-stu-id="bc46c-212">**type**</span></span> | <span data-ttu-id="bc46c-213">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="bc46c-213">Required</span></span> | <span data-ttu-id="bc46c-214">Muss auf `absoluteYearly` festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="bc46c-214">Must be set to `absoluteYearly`.</span></span> |

#### <a name="example"></a><span data-ttu-id="bc46c-215">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bc46c-215">Example</span></span>

- <span data-ttu-id="bc46c-216">Dieses Ereignis jedes Jahr am 15. April wiederholen</span><span class="sxs-lookup"><span data-stu-id="bc46c-216">Repeat this event on April 15 every year</span></span>

  ```json
    "pattern": {
      "type": "absoluteYearly",
      "interval": 1,
      "dayOfMonth": 15,
      "month": 4
    }
  ```

### <a name="relative-yearly"></a><span data-ttu-id="bc46c-217">Relativ jährlich</span><span class="sxs-lookup"><span data-stu-id="bc46c-217">Relative yearly</span></span>

<span data-ttu-id="bc46c-218">Das relative jährliche Muster bewirkt, dass ein Ereignis am gleichen Wochentag an der gleichen relativen Position eines bestimmten Monats basierend auf der Anzahl der Jahre zwischen zwei Vorkommen stattfindet.</span><span class="sxs-lookup"><span data-stu-id="bc46c-218">The relative yearly pattern causes an event to repeat on the same day of the week in the same relative position in a specific month, based on the number of years between each occurrence.</span></span> <span data-ttu-id="bc46c-219">Beispielsweise „jeden letzten Mittwoch im November“.</span><span class="sxs-lookup"><span data-stu-id="bc46c-219">For example, "every last Wednesday of November".</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="bc46c-220">Relevante Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bc46c-220">Relevant properties</span></span>

| <span data-ttu-id="bc46c-221">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bc46c-221">Property</span></span> | <span data-ttu-id="bc46c-222">Relevanz</span><span class="sxs-lookup"><span data-stu-id="bc46c-222">Relevance</span></span> | <span data-ttu-id="bc46c-223">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bc46c-223">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="bc46c-224">**daysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="bc46c-224">**daysOfWeek**</span></span> | <span data-ttu-id="bc46c-225">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="bc46c-225">Required</span></span> | <span data-ttu-id="bc46c-226">Gibt an, an welchem/-n Tag/-en der Woche das Ereignis eintreten kann.</span><span class="sxs-lookup"><span data-stu-id="bc46c-226">Specifies on which day(s) of the week the event can occur.</span></span> <span data-ttu-id="bc46c-227">Relative jährliche Ereignisse treten nur einmal pro Jahr ein, wird also mehr als ein Wert angegeben, fällt das Ereignis auf den ersten Tag, der das Muster erfüllt.</span><span class="sxs-lookup"><span data-stu-id="bc46c-227">Relative yearly events only occur once per year, so if more than one value is specified, the event falls on the first day that satisfies the pattern.</span></span> |
| <span data-ttu-id="bc46c-228">**Index**</span><span class="sxs-lookup"><span data-stu-id="bc46c-228">**index**</span></span> | <span data-ttu-id="bc46c-229">Optional</span><span class="sxs-lookup"><span data-stu-id="bc46c-229">Optional</span></span> | <span data-ttu-id="bc46c-230">Gibt an, in welcher Instanz der zulässigen Tage, die unter **daysOfsWeek** angegeben sind, das Ereignis eintritt, ausgehend von der ersten Instanz des Monats gezählt.</span><span class="sxs-lookup"><span data-stu-id="bc46c-230">Specifies on which instance of the allowed days specified in **daysOfsWeek** the event occurs, counted from the first instance in the month.</span></span> <span data-ttu-id="bc46c-231">Mögliche Werte: `first`, `second`, `third`, `fourth` und `last`.</span><span class="sxs-lookup"><span data-stu-id="bc46c-231">Possible values: `first`, `second`, `third`, `fourth`, and `last`.</span></span> <span data-ttu-id="bc46c-232">Standardwert: `first`.</span><span class="sxs-lookup"><span data-stu-id="bc46c-232">Default value: `first`.</span></span> |
| <span data-ttu-id="bc46c-233">**Monat**</span><span class="sxs-lookup"><span data-stu-id="bc46c-233">**month**</span></span> | <span data-ttu-id="bc46c-234">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="bc46c-234">Required</span></span> | <span data-ttu-id="bc46c-235">Gibt an, in welchem Monat das Ereignis auftritt.</span><span class="sxs-lookup"><span data-stu-id="bc46c-235">Specifies in which month the event occurs.</span></span> |
| <span data-ttu-id="bc46c-236">**Intervall**</span><span class="sxs-lookup"><span data-stu-id="bc46c-236">**interval**</span></span> | <span data-ttu-id="bc46c-237">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="bc46c-237">Required</span></span> | <span data-ttu-id="bc46c-238">Gibt die Anzahl der Jahre zwischen zwei Vorkommen an.</span><span class="sxs-lookup"><span data-stu-id="bc46c-238">Specifies the number of years between each occurrence.</span></span> |
| <span data-ttu-id="bc46c-239">**Typ**</span><span class="sxs-lookup"><span data-stu-id="bc46c-239">**type**</span></span> | <span data-ttu-id="bc46c-240">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="bc46c-240">Required</span></span> | <span data-ttu-id="bc46c-241">Muss auf `relativeMonthly` festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="bc46c-241">Must be set to `relativeMonthly`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="bc46c-242">Beispiele</span><span class="sxs-lookup"><span data-stu-id="bc46c-242">Examples</span></span>

- <span data-ttu-id="bc46c-243">Dieses Ereignis jedes Jahr am letzten Mittwoch im November wiederholen</span><span class="sxs-lookup"><span data-stu-id="bc46c-243">Repeat this event on the last Wednesday of November every year</span></span>

  ```json
    "pattern": {
      "type": "relativeYearly",
      "interval": 1,
      "daysOfWeek": [ "Wednesday" ],
      "index": "last",
      "month": 11
    }
  ```

## <a name="recurrence-ranges"></a><span data-ttu-id="bc46c-244">Serienbereiche</span><span class="sxs-lookup"><span data-stu-id="bc46c-244">Recurrence ranges</span></span>

<span data-ttu-id="bc46c-245">Der zweite Teil einer Serie ist das Muster.</span><span class="sxs-lookup"><span data-stu-id="bc46c-245">The second part of a recurrence is the range.</span></span> <span data-ttu-id="bc46c-246">Dies gibt an, wie lange das Muster wiederholt wird.</span><span class="sxs-lookup"><span data-stu-id="bc46c-246">This specifies how long the pattern repeats.</span></span> <span data-ttu-id="bc46c-247">Ein Ereignis könnte beispielsweise nach 10 Vorkommen an einem bestimmten Datum enden oder kein Ende haben.</span><span class="sxs-lookup"><span data-stu-id="bc46c-247">For example, an event could end after 10 occurrences, by a specific date, or could have no end.</span></span> <span data-ttu-id="bc46c-248">Ein Bereich wird in der API durch die [recurrenceRange-Ressource](../api-reference/v1.0/resources/recurrencepattern.md) dargestellt.</span><span class="sxs-lookup"><span data-stu-id="bc46c-248">A range is represented in the API by the [recurrenceRange resource](../api-reference/v1.0/resources/recurrencepattern.md).</span></span>

<span data-ttu-id="bc46c-249">Je nach Bereichstyp sind bestimmte Felder der **recurrenceRange** obligatorisch oder werden ignoriert.</span><span class="sxs-lookup"><span data-stu-id="bc46c-249">Depending on the type of range, certain fields of the **** are required or ignored.</span></span>

> <span data-ttu-id="bc46c-250">**Hinweis:** Auch wenn ein Feld ignoriert wird, wird es dennoch überprüft.</span><span class="sxs-lookup"><span data-stu-id="bc46c-250">Even if a field is ignored, it is still validated.</span></span> <span data-ttu-id="bc46c-251">Wenn ein Feld über eine festgelegte Liste möglicher Werte verfügt, führt ein Wert außerhalb der zulässigen Gruppe von Werten zu einem Fehler, selbst wenn das Feld ignoriert wird.</span><span class="sxs-lookup"><span data-stu-id="bc46c-251">If a field has a set list of possible values, using a value outside the allowed set will cause an error, even if that field is ignored.</span></span>

<span data-ttu-id="bc46c-252">Werfen wir einen Blick auf die einzelnen Arten möglicher Bereiche.</span><span class="sxs-lookup"><span data-stu-id="bc46c-252">Let's take a look at each of the possible range types.</span></span>

### <a name="numbered-range"></a><span data-ttu-id="bc46c-253">Nummerierter Bereich</span><span class="sxs-lookup"><span data-stu-id="bc46c-253">Numbered range</span></span>

<span data-ttu-id="bc46c-254">Der nummerierte Bereich bewirkt, dass ein Ereignis eine feste Anzahl von Vorkommen (basierend auf dem Muster) ab einem Startdatum auftritt.</span><span class="sxs-lookup"><span data-stu-id="bc46c-254">The numbered range causes an event to occur a fixed number of times (based on the pattern) from a start date.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="bc46c-255">Relevante Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bc46c-255">Relevant properties</span></span>

| <span data-ttu-id="bc46c-256">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bc46c-256">Property</span></span> | <span data-ttu-id="bc46c-257">Relevanz</span><span class="sxs-lookup"><span data-stu-id="bc46c-257">Relevance</span></span> | <span data-ttu-id="bc46c-258">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bc46c-258">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="bc46c-259">**numberOfOccurences**</span><span class="sxs-lookup"><span data-stu-id="bc46c-259">**numberOfOccurences**</span></span> | <span data-ttu-id="bc46c-260">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="bc46c-260">Required</span></span> | <span data-ttu-id="bc46c-261">Gibt die Anzahl von Vorkommen an.</span><span class="sxs-lookup"><span data-stu-id="bc46c-261">Specifies the number of occurrences.</span></span> <span data-ttu-id="bc46c-262">Das Vorkommen muss eine positive ganze Zahl sein.</span><span class="sxs-lookup"><span data-stu-id="bc46c-262">Must be a positive integer.</span></span> |
| <span data-ttu-id="bc46c-263">**recurrenceTimeZone**</span><span class="sxs-lookup"><span data-stu-id="bc46c-263">**recurrenceTimeZone**</span></span> | <span data-ttu-id="bc46c-264">Optional</span><span class="sxs-lookup"><span data-stu-id="bc46c-264">Optional</span></span> | <span data-ttu-id="bc46c-265">Gibt die Zeitzone für die **StartDate**-Eigenschaft an.</span><span class="sxs-lookup"><span data-stu-id="bc46c-265">Specifies the time zone for the **** property.</span></span> <span data-ttu-id="bc46c-266">Falls nicht angegeben, wird die Zeitzone des Ereignisses verwendet.</span><span class="sxs-lookup"><span data-stu-id="bc46c-266">If not specified, the time zone of the event is used.</span></span> |
| <span data-ttu-id="bc46c-267">**startDate**</span><span class="sxs-lookup"><span data-stu-id="bc46c-267">**startDate**</span></span> | <span data-ttu-id="bc46c-268">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="bc46c-268">Required</span></span> | <span data-ttu-id="bc46c-269">Gibt das Datum des Starts des Anwendens des Musters an.</span><span class="sxs-lookup"><span data-stu-id="bc46c-269">Specifies the date to start applying the pattern.</span></span> <span data-ttu-id="bc46c-270">Der Wert von **StartDate** MUSS dem Datumswert der **Start**-Eigenschaft der [Ereignisressource](../api-reference/v1.0/resources/event.md) entsprechen.</span><span class="sxs-lookup"><span data-stu-id="bc46c-270">The value of **** MUST correspond to the date value of the **** property on the [event resource](../api-reference/v1.0/resources/event.md).</span></span> <span data-ttu-id="bc46c-271">Hinweis: Das erste Vorkommen der Besprechung kann nicht an diesem Datum stattfinden, wenn es nicht in das Muster passt.</span><span class="sxs-lookup"><span data-stu-id="bc46c-271">Note: the first occurrence of the meeting may not occur on this date if it does not fit the pattern.</span></span> |
| <span data-ttu-id="bc46c-272">**Typ**</span><span class="sxs-lookup"><span data-stu-id="bc46c-272">**type**</span></span> | <span data-ttu-id="bc46c-273">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="bc46c-273">Required</span></span> | <span data-ttu-id="bc46c-274">Muss auf `numbered` festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="bc46c-274">Must be set to `numbered`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="bc46c-275">Beispiele</span><span class="sxs-lookup"><span data-stu-id="bc46c-275">Examples</span></span>

- <span data-ttu-id="bc46c-276">Dieses Ereignis 10 Mal wiederholen</span><span class="sxs-lookup"><span data-stu-id="bc46c-276">Repeat this event 10 times</span></span>

  ```json
    "range": {
      "type": "numbered",
      "startDate": "2017-04-02",
      "numberOfOccurrences": 10
    }
  ```

### <a name="end-date-range"></a><span data-ttu-id="bc46c-277">Enddatumsbereich</span><span class="sxs-lookup"><span data-stu-id="bc46c-277">End date range</span></span>

<span data-ttu-id="bc46c-278">Der Enddatumsbereich bewirkt, dass ein Ereignis an allen Tagen eintritt, die das entsprechende Muster zwischen einem Startdatum und einem Enddatum aufweisen.</span><span class="sxs-lookup"><span data-stu-id="bc46c-278">The end date range causes an event to occur on all days that fit the applicable pattern between a start date and an end date.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="bc46c-279">Relevante Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bc46c-279">Relevant properties</span></span>

| <span data-ttu-id="bc46c-280">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bc46c-280">Property</span></span> | <span data-ttu-id="bc46c-281">Relevanz</span><span class="sxs-lookup"><span data-stu-id="bc46c-281">Relevance</span></span> | <span data-ttu-id="bc46c-282">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bc46c-282">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="bc46c-283">**endDate**</span><span class="sxs-lookup"><span data-stu-id="bc46c-283">**endDate**</span></span> | <span data-ttu-id="bc46c-284">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="bc46c-284">Required</span></span> | <span data-ttu-id="bc46c-285">Gibt das Datum zum Beenden des Anwendens des Musters an.</span><span class="sxs-lookup"><span data-stu-id="bc46c-285">Specifies the date to stop applying the pattern.</span></span> <span data-ttu-id="bc46c-286">Hinweis: Das letzte Vorkommen der Besprechung kann nicht an diesem Datum auftreten, wenn es nicht in das Muster passt.</span><span class="sxs-lookup"><span data-stu-id="bc46c-286">Note: the last occurrence of the meeting may not occur on this date if it does not fit the pattern.</span></span> |
| <span data-ttu-id="bc46c-287">**recurrenceTimeZone**</span><span class="sxs-lookup"><span data-stu-id="bc46c-287">**recurrenceTimeZone**</span></span> | <span data-ttu-id="bc46c-288">Optional</span><span class="sxs-lookup"><span data-stu-id="bc46c-288">Optional</span></span> | <span data-ttu-id="bc46c-289">Gibt die Zeitzone für die **startDate**- und **endDate**-Eigenschaften an.</span><span class="sxs-lookup"><span data-stu-id="bc46c-289">Specifies the time zone for the **** and **** properties.</span></span> <span data-ttu-id="bc46c-290">Falls nicht angegeben, wird die Zeitzone des Ereignisses verwendet.</span><span class="sxs-lookup"><span data-stu-id="bc46c-290">If not specified, the time zone of the event is used.</span></span> |
| <span data-ttu-id="bc46c-291">**startDate**</span><span class="sxs-lookup"><span data-stu-id="bc46c-291">**startDate**</span></span> | <span data-ttu-id="bc46c-292">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="bc46c-292">Required</span></span> | <span data-ttu-id="bc46c-293">Gibt das Datum des Starts des Anwendens des Musters an.</span><span class="sxs-lookup"><span data-stu-id="bc46c-293">Specifies the date to start applying the pattern.</span></span> <span data-ttu-id="bc46c-294">Der Wert von **StartDate** MUSS dem Datumswert der **Start**-Eigenschaft der [Ereignisressource](../api-reference/v1.0/resources/event.md) entsprechen.</span><span class="sxs-lookup"><span data-stu-id="bc46c-294">The value of **** MUST correspond to the date value of the **** property on the [event resource](../api-reference/v1.0/resources/event.md).</span></span> <span data-ttu-id="bc46c-295">Hinweis: Das erste Vorkommen der Besprechung kann nicht an diesem Datum stattfinden, wenn es nicht in das Muster passt.</span><span class="sxs-lookup"><span data-stu-id="bc46c-295">Note: the first occurrence of the meeting may not occur on this date if it does not fit the pattern.</span></span> |
| <span data-ttu-id="bc46c-296">**Typ**</span><span class="sxs-lookup"><span data-stu-id="bc46c-296">**type**</span></span> | <span data-ttu-id="bc46c-297">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="bc46c-297">Required</span></span> | <span data-ttu-id="bc46c-298">Muss auf **EndDate** festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="bc46c-298">Must be set to ****.</span></span> |

#### <a name="examples"></a><span data-ttu-id="bc46c-299">Beispiele</span><span class="sxs-lookup"><span data-stu-id="bc46c-299">Examples</span></span>

- <span data-ttu-id="bc46c-300">Dieses Ereignis vom 1. Juli 2017 bis zum 31. Juli 2017 wiederholen</span><span class="sxs-lookup"><span data-stu-id="bc46c-300">Repeat this event from July 1 2017 to July 31 2017</span></span>

  ```json
    "range": {
      "type": "endDate",
      "startDate": "2017-07-01",
      "endDate": "2017-07-31"
    }
  ```

### <a name="no-end-range"></a><span data-ttu-id="bc46c-301">Kein Endbereich</span><span class="sxs-lookup"><span data-stu-id="bc46c-301">No end range</span></span>

<span data-ttu-id="bc46c-302">Der Enddatumsbereich bewirkt, dass ein Ereignis an allen Tagen eintritt, die dem anwendbaren Muster nach einem Startdatum entsprechen.</span><span class="sxs-lookup"><span data-stu-id="bc46c-302">The no end range causes an event to occur on all days that fit the applicable pattern after a start date.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="bc46c-303">Relevante Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bc46c-303">Relevant properties</span></span>

| <span data-ttu-id="bc46c-304">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bc46c-304">Property</span></span> | <span data-ttu-id="bc46c-305">Relevanz</span><span class="sxs-lookup"><span data-stu-id="bc46c-305">Relevance</span></span> | <span data-ttu-id="bc46c-306">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bc46c-306">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="bc46c-307">**recurrenceTimeZone**</span><span class="sxs-lookup"><span data-stu-id="bc46c-307">**recurrenceTimeZone**</span></span> | <span data-ttu-id="bc46c-308">Optional</span><span class="sxs-lookup"><span data-stu-id="bc46c-308">Optional</span></span> | <span data-ttu-id="bc46c-309">Gibt die Zeitzone für die **StartDate**-Eigenschaft an.</span><span class="sxs-lookup"><span data-stu-id="bc46c-309">Specifies the time zone for the **** property.</span></span> <span data-ttu-id="bc46c-310">Falls nicht angegeben, wird die Zeitzone des Ereignisses verwendet.</span><span class="sxs-lookup"><span data-stu-id="bc46c-310">If not specified, the time zone of the event is used.</span></span> |
| <span data-ttu-id="bc46c-311">**startDate**</span><span class="sxs-lookup"><span data-stu-id="bc46c-311">**startDate**</span></span> | <span data-ttu-id="bc46c-312">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="bc46c-312">Required</span></span> | <span data-ttu-id="bc46c-313">Gibt das Datum des Starts des Anwendens des Musters an.</span><span class="sxs-lookup"><span data-stu-id="bc46c-313">Specifies the date to start applying the pattern.</span></span> <span data-ttu-id="bc46c-314">Der Wert von **StartDate** MUSS dem Datumswert der **Start**-Eigenschaft der [Ereignisressource](../api-reference/v1.0/resources/event.md) entsprechen.</span><span class="sxs-lookup"><span data-stu-id="bc46c-314">The value of **** MUST correspond to the date value of the **** property on the [event resource](../api-reference/v1.0/resources/event.md).</span></span> <span data-ttu-id="bc46c-315">Hinweis: Das erste Vorkommen der Besprechung kann nicht an diesem Datum stattfinden, wenn es nicht in das Muster passt.</span><span class="sxs-lookup"><span data-stu-id="bc46c-315">Note: the first occurrence of the meeting may not occur on this date if it does not fit the pattern.</span></span> |
| <span data-ttu-id="bc46c-316">**Typ**</span><span class="sxs-lookup"><span data-stu-id="bc46c-316">**type**</span></span> | <span data-ttu-id="bc46c-317">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="bc46c-317">Required</span></span> | <span data-ttu-id="bc46c-318">Muss auf `noEnd` festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="bc46c-318">Must be set to `noEnd`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="bc46c-319">Beispiele</span><span class="sxs-lookup"><span data-stu-id="bc46c-319">Examples</span></span>

- <span data-ttu-id="bc46c-320">Dieses Ereignis ab dem 15. Mai 2017 immer wiederholen</span><span class="sxs-lookup"><span data-stu-id="bc46c-320">Repeat this event from May 15 2017 forever</span></span>

  ```json
    "range": {
      "type": "noEnd",
      "startDate": "2017-05-15"
    }
  ```

## <a name="using-patterns-and-ranges-to-create-recurring-events"></a><span data-ttu-id="bc46c-321">Verwenden von Mustern und Bereichen zum Erstellen von Ereignisserien</span><span class="sxs-lookup"><span data-stu-id="bc46c-321">Using patterns and ranges to create recurring events</span></span>

<span data-ttu-id="bc46c-322">Nachdem wir uns nun Muster und Bereiche separat angesehen haben, schauen wir uns nun deren Zusammenwirken und Interagieren mit den **Start**- und **End**-Eigenschaften zu dem Ereignis an.</span><span class="sxs-lookup"><span data-stu-id="bc46c-322">Now that we've looked at patterns and ranges separately, let's look at how they work together and how they interact with the **** and **** properties on the event.</span></span>

### <a name="creating-a-recurrence-rule"></a><span data-ttu-id="bc46c-323">Erstellen einer Serienregel</span><span class="sxs-lookup"><span data-stu-id="bc46c-323">Creating a recurrence rule</span></span>

<span data-ttu-id="bc46c-324">Um eine Serienregel zu erstellen, müssen Sie sowohl ein Muster als auch einen Bereich angeben.</span><span class="sxs-lookup"><span data-stu-id="bc46c-324">In order to create a recurrence rule, you must specify both a pattern and a range.</span></span> <span data-ttu-id="bc46c-325">Jeder Mustertyp kann mit einem beliebigen Bereichstyp arbeiten.</span><span class="sxs-lookup"><span data-stu-id="bc46c-325">Any pattern type can work with any range type.</span></span> <span data-ttu-id="bc46c-326">Im Anschluss finden Sie einige Beispiele:</span><span class="sxs-lookup"><span data-stu-id="bc46c-326">Here are a few suggestions:</span></span>

#### <a name="examples"></a><span data-ttu-id="bc46c-327">Beispiele</span><span class="sxs-lookup"><span data-stu-id="bc46c-327">Examples</span></span>

- <span data-ttu-id="bc46c-328">**Besprechung von 13:00-13:30 Uhr, jeden Montag ab dem 4. September 2017 bis zum Ende des Jahres**</span><span class="sxs-lookup"><span data-stu-id="bc46c-328">**Meet from 1:00 PM to 1:30 PM every Monday starting September 4, 2017 until the end of the year**</span></span>

  - <span data-ttu-id="bc46c-329">Die Anforderung „jeden Montag“ wird ganz einfach durch den `weekly`-Serienmustertyp erfüllt.</span><span class="sxs-lookup"><span data-stu-id="bc46c-329">The "every Monday" requirement is easily met by the `weekly` recurrence pattern type.</span></span>
  - <span data-ttu-id="bc46c-330">Die Anforderung „bis zum Ende des Jahres“ gibt einen `endDate`-Serienbereichstypen an.</span><span class="sxs-lookup"><span data-stu-id="bc46c-330">The "until the end of the year" requirement indicates an `endDate` recurrence range type.</span></span>

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

  <span data-ttu-id="bc46c-331">Da der 31. Dezember 2017 auf einen Sonntag fällt, ist das letzte Vorkommen in dieser Serie am Montag, den 25. Dezember.</span><span class="sxs-lookup"><span data-stu-id="bc46c-331">Because December 31, 2017 is on a Sunday, the last occurrence in this series will be on Monday, December 25.</span></span>

- <span data-ttu-id="bc46c-332">**Besprechung von 14:00-15:00 Uhr am ersten Donnerstag jeden zweiten Monat, ab dem 29. August 2017**</span><span class="sxs-lookup"><span data-stu-id="bc46c-332">**Meet from 2:00 PM to 3:00 PM on the first Thursday of every other month starting August 29, 2017**</span></span>

  - <span data-ttu-id="bc46c-333">Die Anforderung „erster Donnerstag jeden zweiten Monat“ kann durch ein relatives monatliches Muster erfüllt werden.</span><span class="sxs-lookup"><span data-stu-id="bc46c-333">The "first Thursday of every other month" requirement is achievable using a relative monthly pattern.</span></span> <span data-ttu-id="bc46c-334">Der Teil „jeden zweiten Monats“ gibt an, dass das **Intervall** auf `2` festgelegt werden sollte.</span><span class="sxs-lookup"><span data-stu-id="bc46c-334">The "every other month" portion indicates the **** should be set to `2`.</span></span>
  - <span data-ttu-id="bc46c-335">Da es keine Anforderung an ein Enddatum gibt, kann ein `noEnd`-Bereichstyp verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="bc46c-335">Since there is no requirement on an end date, a `noEnd` range type can be used.</span></span>

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

  <span data-ttu-id="bc46c-336">Da der Wert von **startDate** nach dem ersten Donnerstag im August liegt, ist das erste Vorkommen dieser Serie im September.</span><span class="sxs-lookup"><span data-stu-id="bc46c-336">Because the value of **** is after the first Thursday in August, the first occurrence of this series will be in September.</span></span>

## <a name="next-steps"></a><span data-ttu-id="bc46c-337">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="bc46c-337">Next steps</span></span>
    
<span data-ttu-id="bc46c-338">Erfahren Sie mehr zur [Integration in Outlook-Kalender](outlook-calendar-concept-overview.md).</span><span class="sxs-lookup"><span data-stu-id="bc46c-338">Find out more about [integrating with Outlook calendar](outlook-calendar-concept-overview.md).</span></span>
