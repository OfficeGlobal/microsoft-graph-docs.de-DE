# <a name="schedule-repeating-appointments-as-recurring-events-in-outlook"></a><span data-ttu-id="b5e64-101">Planen wiederkehrender Termine als wiederkehrende Ereignisse in Outlook</span><span class="sxs-lookup"><span data-stu-id="b5e64-101">Schedule repeating appointments as recurring events in Outlook</span></span>

<span data-ttu-id="b5e64-102">Ereignisserien sind ein wichtiger Bestandteil der Kalenderfunktionen von Outlook.</span><span class="sxs-lookup"><span data-stu-id="b5e64-102">Recurring events are an important part of Outlook calendaring.</span></span> <span data-ttu-id="b5e64-103">Ganz gleich, ob es sich um eine wöchentliche Besprechung mit Ihrem Vorgesetzten oder eine Abteilungsbesprechung handelt, die jeden zweiten Dienstag im Monat stattfindet, mit Ereignisserien können Sie ganz einfach eine Ereignisserie erstellen und der Server füllt den Kalender mit dem Rest der Serie.</span><span class="sxs-lookup"><span data-stu-id="b5e64-103">Whether it's a weekly one-on-one meeting with your manager, or a division-wide review meeting that happens on the second Tuesday of each month, recurring events make it easy to create the event once, and let the server fill in the rest of the series.</span></span>

<span data-ttu-id="b5e64-104">Die wichtigsten Informationen, mit denen Ereignisserien in einzelne Termine „erweitert“ werden können, die Serienregel.</span><span class="sxs-lookup"><span data-stu-id="b5e64-104">The key bit of information that allows recurring events to "expand" into individual occurrences is the recurrence rule.</span></span> <span data-ttu-id="b5e64-105">In der Serie ist die Wiederholungsfrequenz und Dauer eines Ereignisses angegeben.</span><span class="sxs-lookup"><span data-stu-id="b5e64-105">The rule specifies both how often an event repeats, and for how long.</span></span> <span data-ttu-id="b5e64-106">Die Outlook-REST-APIs modellieren Serienregeln in der **Serien**-Eigenschaft der [Ereignisressource](../api-reference/v1.0/resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="b5e64-106">The Outlook REST APIs model recurrence rules in the **recurrence** property of the [event resource](../api-reference/v1.0/resources/event.md).</span></span> 

<span data-ttu-id="b5e64-107">Jede Serie besteht aus zwei Teilen: dem Serienmuster (wie oft) und dem Serienbereich (für wie lange).</span><span class="sxs-lookup"><span data-stu-id="b5e64-107">Each recurrence is made up of two parts: the recurrence pattern (how often), and the recurrence range (for how long).</span></span>

## <a name="recurrence-patterns"></a><span data-ttu-id="b5e64-108">Serienmuster</span><span class="sxs-lookup"><span data-stu-id="b5e64-108">Recurrence patterns</span></span>

<span data-ttu-id="b5e64-109">Der erste Teil einer Serie ist das Muster.</span><span class="sxs-lookup"><span data-stu-id="b5e64-109">The first part of a recurrence is the pattern.</span></span> <span data-ttu-id="b5e64-110">Darin ist angegeben, wie oft das Ereignis wiederholt wird.</span><span class="sxs-lookup"><span data-stu-id="b5e64-110">This specifies how often the event repeats.</span></span> <span data-ttu-id="b5e64-111">Beispielsweise könnte ein Ereignis „alle 3 Tage“, „jeden Donnerstag“ oder „jedes Jahr am 22. Juli“ wiederholt werden.</span><span class="sxs-lookup"><span data-stu-id="b5e64-111">For example, an event could repeat "every 3 days," "every Thursday," or "on July 22 every year."</span></span> <span data-ttu-id="b5e64-112">Ein Muster wird in der API durch die [recurrencePattern-Ressource](../api-reference/v1.0/resources/recurrencepattern.md) dargestellt.</span><span class="sxs-lookup"><span data-stu-id="b5e64-112">A pattern is represented in the API by the [recurrencePattern resource](../api-reference/v1.0/resources/recurrencepattern.md).</span></span>

<span data-ttu-id="b5e64-113">Je nach Mustertyp sind bestimmte Felder des **recurrencePattern** obligatorisch, optional oder werden ignoriert.</span><span class="sxs-lookup"><span data-stu-id="b5e64-113">Depending on the type of pattern, certain fields of the **recurrencePattern** are required, optional, or ignored.</span></span>

> <span data-ttu-id="b5e64-114">**Hinweis:** Auch wenn ein Feld ignoriert wird, wird es dennoch überprüft.</span><span class="sxs-lookup"><span data-stu-id="b5e64-114">**Note**: Even if a field is ignored, it is still validated.</span></span> <span data-ttu-id="b5e64-115">Wenn ein Feld über eine festgelegte Liste möglicher Werte verfügt, führt ein Wert außerhalb der zulässigen Gruppe von Werten zu einem Fehler, selbst wenn das Feld ignoriert wird.</span><span class="sxs-lookup"><span data-stu-id="b5e64-115">If a field has a set list of possible values, using a value outside the allowed set causes an error, even if that field is ignored.</span></span>

<span data-ttu-id="b5e64-116">Werfen Sie einen Blick auf die einzelnen Arten möglicher Muster.</span><span class="sxs-lookup"><span data-stu-id="b5e64-116">Let's take a look at each of the possible pattern types.</span></span>

### <a name="daily"></a><span data-ttu-id="b5e64-117">Täglich</span><span class="sxs-lookup"><span data-stu-id="b5e64-117">Daily</span></span>

<span data-ttu-id="b5e64-118">Das tägliche Serienmuster bewirkt, dass ein Ereignis basierend auf einer Anzahl von Tagen zwischen zwei Vorkommen wiederholt wird.</span><span class="sxs-lookup"><span data-stu-id="b5e64-118">The daily recurrence pattern causes an event to repeat based on a number of days between each occurrence.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="b5e64-119">Relevante Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b5e64-119">Relevant properties</span></span>

| <span data-ttu-id="b5e64-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b5e64-120">Property</span></span> | <span data-ttu-id="b5e64-121">Relevanz</span><span class="sxs-lookup"><span data-stu-id="b5e64-121">Relevance</span></span> | <span data-ttu-id="b5e64-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b5e64-122">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="b5e64-123">**Intervall**</span><span class="sxs-lookup"><span data-stu-id="b5e64-123">**interval**</span></span> | <span data-ttu-id="b5e64-124">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="b5e64-124">Required</span></span> | <span data-ttu-id="b5e64-125">Gibt die Anzahl der Tage zwischen zwei Vorkommen an.</span><span class="sxs-lookup"><span data-stu-id="b5e64-125">Specifies the number of days between each occurrence.</span></span> |
| <span data-ttu-id="b5e64-126">**Typ**</span><span class="sxs-lookup"><span data-stu-id="b5e64-126">**type**</span></span> | <span data-ttu-id="b5e64-127">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="b5e64-127">Required</span></span> | <span data-ttu-id="b5e64-128">Muss auf `daily` festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="b5e64-128">Must be set to `daily`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="b5e64-129">Beispiele</span><span class="sxs-lookup"><span data-stu-id="b5e64-129">Examples</span></span>

- <span data-ttu-id="b5e64-130">Dieses Ereignis täglich wiederholen</span><span class="sxs-lookup"><span data-stu-id="b5e64-130">Repeat this event every day</span></span>

  ```json
    "pattern": {
      "type": "daily",
      "interval": 1
    }
  ```
- <span data-ttu-id="b5e64-131">Dieses Ereignis alle drei Tage wiederholen</span><span class="sxs-lookup"><span data-stu-id="b5e64-131">Repeat this event every three days</span></span>

  ```json
    "pattern": {
      "type": "daily",
      "interval": 3
    }
  ```

### <a name="weekly"></a><span data-ttu-id="b5e64-132">Wöchentlich</span><span class="sxs-lookup"><span data-stu-id="b5e64-132">Weekly</span></span>

<span data-ttu-id="b5e64-133">Das wöchentliche Serienmuster bewirkt, dass ein Ereignis am gleichen Tag oder an den gleichen Tagen einer Woche basierend auf der Anzahl von Wochen zwischen zwei Vorkommen wiederholt wird.</span><span class="sxs-lookup"><span data-stu-id="b5e64-133">The weekly recurrence pattern causes an event to repeat on the same day or days of the week, based on the number of weeks between each set of occurrences.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="b5e64-134">Relevante Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b5e64-134">Relevant properties</span></span>

| <span data-ttu-id="b5e64-135">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b5e64-135">Property</span></span> | <span data-ttu-id="b5e64-136">Relevanz</span><span class="sxs-lookup"><span data-stu-id="b5e64-136">Relevance</span></span> | <span data-ttu-id="b5e64-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b5e64-137">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="b5e64-138">**daysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="b5e64-138">**daysOfWeek**</span></span> | <span data-ttu-id="b5e64-139">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="b5e64-139">Required</span></span> | <span data-ttu-id="b5e64-140">Gibt an, an welchem/-n Tag/-en der Woche das Ereignis eintritt.</span><span class="sxs-lookup"><span data-stu-id="b5e64-140">Specifies on which day(s) of the week the event occurs.</span></span> |
| <span data-ttu-id="b5e64-141">**firstDayOfWeek**</span><span class="sxs-lookup"><span data-stu-id="b5e64-141">**firstDayOfWeek**</span></span> | <span data-ttu-id="b5e64-142">Optional</span><span class="sxs-lookup"><span data-stu-id="b5e64-142">Optional</span></span> | <span data-ttu-id="b5e64-143">Gibt an, welcher Tag als erster Tag der Woche angesehen wird.</span><span class="sxs-lookup"><span data-stu-id="b5e64-143">Specifies which day is considered the first day of the week.</span></span> <span data-ttu-id="b5e64-144">Standardwert: `Sunday`.</span><span class="sxs-lookup"><span data-stu-id="b5e64-144">Default value: `Sunday`.</span></span> |
| <span data-ttu-id="b5e64-145">**Intervall**</span><span class="sxs-lookup"><span data-stu-id="b5e64-145">**interval**</span></span> | <span data-ttu-id="b5e64-146">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="b5e64-146">Required</span></span> | <span data-ttu-id="b5e64-147">Gibt die Anzahl der Wochen zwischen zwei Vorkommen an.</span><span class="sxs-lookup"><span data-stu-id="b5e64-147">Specifies the number of weeks between each set of occurrences.</span></span> |
| <span data-ttu-id="b5e64-148">**Typ**</span><span class="sxs-lookup"><span data-stu-id="b5e64-148">**type**</span></span> | <span data-ttu-id="b5e64-149">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="b5e64-149">Required</span></span> | <span data-ttu-id="b5e64-150">Muss auf `weekly` festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="b5e64-150">Must be set to `weekly`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="b5e64-151">Beispiele</span><span class="sxs-lookup"><span data-stu-id="b5e64-151">Examples</span></span>

- <span data-ttu-id="b5e64-152">Dieses Ereignis jeden Donnerstag wiederholen</span><span class="sxs-lookup"><span data-stu-id="b5e64-152">Repeat this event every Thursday</span></span>

  ```json
    "pattern": {
      "type": "weekly",
      "interval": 1,
      "daysOfWeek": [ "Thursday" ]
    }
  ```
- <span data-ttu-id="b5e64-153">Dieses Ereignis jeden Montag und Dienstag wiederholen</span><span class="sxs-lookup"><span data-stu-id="b5e64-153">Repeat this event every other Monday and Tuesday</span></span>

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

### <a name="absolute-monthly"></a><span data-ttu-id="b5e64-154">Absolut monatlich</span><span class="sxs-lookup"><span data-stu-id="b5e64-154">Absolute monthly</span></span>

<span data-ttu-id="b5e64-155">Das absolute monatliche Muster bewirkt, dass ein Ereignis am gleichen Tag des Monats (z. B. dem 15.) basierend auf der Anzahl der Monate zwischen zwei Vorkommen stattfindet.</span><span class="sxs-lookup"><span data-stu-id="b5e64-155">The absolute monthly pattern causes an event to repeat on the same day of the month (for example, the 15th), based on the number of months between each occurrence.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="b5e64-156">Relevante Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b5e64-156">Relevant properties</span></span>

| <span data-ttu-id="b5e64-157">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b5e64-157">Property</span></span> | <span data-ttu-id="b5e64-158">Relevanz</span><span class="sxs-lookup"><span data-stu-id="b5e64-158">Relevance</span></span> | <span data-ttu-id="b5e64-159">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b5e64-159">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="b5e64-160">**dayOfMonth**</span><span class="sxs-lookup"><span data-stu-id="b5e64-160">**dayOfMonth**</span></span> | <span data-ttu-id="b5e64-161">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="b5e64-161">Required</span></span> | <span data-ttu-id="b5e64-162">Gibt an, an welchem Tag des Monats das Ereignis eintritt.</span><span class="sxs-lookup"><span data-stu-id="b5e64-162">Specifies on which day of the month the event occurs.</span></span> |
| <span data-ttu-id="b5e64-163">**Intervall**</span><span class="sxs-lookup"><span data-stu-id="b5e64-163">**interval**</span></span> | <span data-ttu-id="b5e64-164">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="b5e64-164">Required</span></span> | <span data-ttu-id="b5e64-165">Gibt die Anzahl der Monate zwischen zwei Vorkommen an.</span><span class="sxs-lookup"><span data-stu-id="b5e64-165">Specifies the number of months between each occurrence.</span></span> |
| <span data-ttu-id="b5e64-166">**Typ**</span><span class="sxs-lookup"><span data-stu-id="b5e64-166">**type**</span></span> | <span data-ttu-id="b5e64-167">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="b5e64-167">Required</span></span> | <span data-ttu-id="b5e64-168">Muss auf `absoluteMonthly` festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="b5e64-168">Must be set to `absoluteMonthly`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="b5e64-169">Beispiele</span><span class="sxs-lookup"><span data-stu-id="b5e64-169">Examples</span></span>

- <span data-ttu-id="b5e64-170">Dieses Ereignis jeden Monat am 15. wiederholen</span><span class="sxs-lookup"><span data-stu-id="b5e64-170">Repeat this event on the 15th of every month</span></span>

  ```json
    "pattern": {
      "type": "absoluteMonthly",
      "interval": 1,
      "dayOfMonth": 15
    }
  ```
- <span data-ttu-id="b5e64-171">Dieses Ereignis vierteljährlich (alle 3 Monate) am 7. wiederholen</span><span class="sxs-lookup"><span data-stu-id="b5e64-171">Repeat this event quarterly (every 3 months) on the 7th</span></span>

  ```json
    "pattern": {
      "type": "absoluteMonthly",
      "interval": 3,
      "dayOfMonth": 7
    }
  ```

### <a name="relative-monthly"></a><span data-ttu-id="b5e64-172">Relativ monatlich</span><span class="sxs-lookup"><span data-stu-id="b5e64-172">Relative monthly</span></span>

<span data-ttu-id="b5e64-173">Das relative monatliche Muster bewirkt, dass ein Ereignis am gleichen Wochentag an der gleichen relativen Position des Monats basierend auf der Anzahl der Monate zwischen zwei Vorkommen stattfindet.</span><span class="sxs-lookup"><span data-stu-id="b5e64-173">The relative monthly pattern causes an event to repeat on the same day of the week in the same relative position in the month, based on the number of months between each occurrence.</span></span> <span data-ttu-id="b5e64-174">Beispielsweise „jeden zweiten Mittwoch des Monats“.</span><span class="sxs-lookup"><span data-stu-id="b5e64-174">For example, "every second Wednesday of the month."</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="b5e64-175">Relevante Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b5e64-175">Relevant properties</span></span>

| <span data-ttu-id="b5e64-176">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b5e64-176">Property</span></span> | <span data-ttu-id="b5e64-177">Relevanz</span><span class="sxs-lookup"><span data-stu-id="b5e64-177">Relevance</span></span> | <span data-ttu-id="b5e64-178">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b5e64-178">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="b5e64-179">**daysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="b5e64-179">**daysOfWeek**</span></span> | <span data-ttu-id="b5e64-180">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="b5e64-180">Required</span></span> | <span data-ttu-id="b5e64-181">Gibt an, an welchem/-n Tag/-en der Woche das Ereignis eintreten kann.</span><span class="sxs-lookup"><span data-stu-id="b5e64-181">Specifies on which day(s) of the week the event can occur.</span></span> <span data-ttu-id="b5e64-182">Relative monatliche Ereignisse treten nur einmal pro Monat ein, wird also mehr als ein Wert angegeben, fällt das Ereignis auf den ersten Tag, der das Muster erfüllt.</span><span class="sxs-lookup"><span data-stu-id="b5e64-182">Relative monthly events only occur once per month, so if more than one value is specified, the event falls on the first day that satisfies the pattern.</span></span> |
| <span data-ttu-id="b5e64-183">**Index**</span><span class="sxs-lookup"><span data-stu-id="b5e64-183">**index**</span></span> | <span data-ttu-id="b5e64-184">Optional</span><span class="sxs-lookup"><span data-stu-id="b5e64-184">Optional</span></span> | <span data-ttu-id="b5e64-185">Gibt an, in welcher Instanz der zulässigen Tage, die unter **daysOfsWeek** angegeben sind, das Ereignis eintritt, ausgehend von der ersten Instanz des Monats gezählt.</span><span class="sxs-lookup"><span data-stu-id="b5e64-185">Specifies on which instance of the allowed days specified in **daysOfsWeek** the event occurs, counted from the first instance in the month.</span></span> <span data-ttu-id="b5e64-186">Mögliche Werte: `first`, `second`, `third`, `fourth` und `last`.</span><span class="sxs-lookup"><span data-stu-id="b5e64-186">Possible values: `first`, `second`, `third`, `fourth`, and `last`.</span></span> <span data-ttu-id="b5e64-187">Standardwert: `first`.</span><span class="sxs-lookup"><span data-stu-id="b5e64-187">Default value: `first`.</span></span> |
| <span data-ttu-id="b5e64-188">**Intervall**</span><span class="sxs-lookup"><span data-stu-id="b5e64-188">**interval**</span></span> | <span data-ttu-id="b5e64-189">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="b5e64-189">Required</span></span> | <span data-ttu-id="b5e64-190">Gibt die Anzahl der Monate zwischen zwei Vorkommen an.</span><span class="sxs-lookup"><span data-stu-id="b5e64-190">Specifies the number of months between each occurrence.</span></span> |
| <span data-ttu-id="b5e64-191">**Typ**</span><span class="sxs-lookup"><span data-stu-id="b5e64-191">**type**</span></span> | <span data-ttu-id="b5e64-192">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="b5e64-192">Required</span></span> | <span data-ttu-id="b5e64-193">Muss auf `relativeMonthly` festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="b5e64-193">Must be set to `relativeMonthly`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="b5e64-194">Beispiele</span><span class="sxs-lookup"><span data-stu-id="b5e64-194">Examples</span></span>

- <span data-ttu-id="b5e64-195">Dieses Ereignis jeden zweiten Mittwoch des Monats wiederholen</span><span class="sxs-lookup"><span data-stu-id="b5e64-195">Repeat this event on the second Wednesday of every month</span></span>

  ```json
    "pattern": {
      "type": "relativeMonthly",
      "interval": 1,
      "daysOfWeek": [ "Wednesday" ],
      "index": "second"
    }
  ```
- <span data-ttu-id="b5e64-196">Dieses Ereignis jeden zweiten Mittwoch des Monats wiederholen</span><span class="sxs-lookup"><span data-stu-id="b5e64-196">Repeat this event on the first Thursday or Friday of every month</span></span>

  ```json
    "pattern": {
      "type": "relativeMonthly",
      "interval": 1,
      "daysOfWeek": [ "Thursday", "Friday" ],
      "index": "first"
    }
  ```

### <a name="absolute-yearly"></a><span data-ttu-id="b5e64-197">Absolut jährlich</span><span class="sxs-lookup"><span data-stu-id="b5e64-197">Absolute yearly</span></span>

<span data-ttu-id="b5e64-198">Das absolut jährliche Muster bewirkt, dass ein Ereignis am gleichen Tag und im gleichen Monat (z. B. dem 15. April), basierend auf der Anzahl der Jahre zwischen zwei Vorkommen stattfindet.</span><span class="sxs-lookup"><span data-stu-id="b5e64-198">The absolute yearly pattern causes an event to repeat on the same month and day (for example, April 15), based on the number of years between each occurrence.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="b5e64-199">Relevante Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b5e64-199">Relevant properties</span></span>

| <span data-ttu-id="b5e64-200">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b5e64-200">Property</span></span> | <span data-ttu-id="b5e64-201">Relevanz</span><span class="sxs-lookup"><span data-stu-id="b5e64-201">Relevance</span></span> | <span data-ttu-id="b5e64-202">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b5e64-202">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="b5e64-203">**dayOfMonth**</span><span class="sxs-lookup"><span data-stu-id="b5e64-203">**dayOfMonth**</span></span> | <span data-ttu-id="b5e64-204">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="b5e64-204">Required</span></span> | <span data-ttu-id="b5e64-205">Gibt an, an welchem Tag des Monats das Ereignis eintritt.</span><span class="sxs-lookup"><span data-stu-id="b5e64-205">Specifies on which day of the month the event occurs.</span></span> |
| <span data-ttu-id="b5e64-206">**Monat**</span><span class="sxs-lookup"><span data-stu-id="b5e64-206">**month**</span></span> | <span data-ttu-id="b5e64-207">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="b5e64-207">Required</span></span> | <span data-ttu-id="b5e64-208">Gibt an, in welchem Monat das Ereignis auftritt.</span><span class="sxs-lookup"><span data-stu-id="b5e64-208">Specifies in which month the event occurs.</span></span> |
| <span data-ttu-id="b5e64-209">**Intervall**</span><span class="sxs-lookup"><span data-stu-id="b5e64-209">**interval**</span></span> | <span data-ttu-id="b5e64-210">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="b5e64-210">Required</span></span> | <span data-ttu-id="b5e64-211">Gibt die Anzahl der Jahre zwischen zwei Vorkommen an.</span><span class="sxs-lookup"><span data-stu-id="b5e64-211">Specifies the number of years between each occurrence.</span></span> |
| <span data-ttu-id="b5e64-212">**Typ**</span><span class="sxs-lookup"><span data-stu-id="b5e64-212">**type**</span></span> | <span data-ttu-id="b5e64-213">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="b5e64-213">Required</span></span> | <span data-ttu-id="b5e64-214">Muss auf `absoluteYearly` festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="b5e64-214">Must be set to `absoluteYearly`.</span></span> |

#### <a name="example"></a><span data-ttu-id="b5e64-215">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b5e64-215">Example</span></span>

- <span data-ttu-id="b5e64-216">Dieses Ereignis jedes Jahr am 15. April wiederholen</span><span class="sxs-lookup"><span data-stu-id="b5e64-216">Repeat this event on April 15 every year</span></span>

  ```json
    "pattern": {
      "type": "absoluteYearly",
      "interval": 1,
      "dayOfMonth": 15,
      "month": 4
    }
  ```

### <a name="relative-yearly"></a><span data-ttu-id="b5e64-217">Relativ jährlich</span><span class="sxs-lookup"><span data-stu-id="b5e64-217">Relative yearly</span></span>

<span data-ttu-id="b5e64-218">Das relative jährliche Muster bewirkt, dass ein Ereignis am gleichen Wochentag an der gleichen relativen Position eines bestimmten Monats basierend auf der Anzahl der Jahre zwischen zwei Vorkommen stattfindet.</span><span class="sxs-lookup"><span data-stu-id="b5e64-218">The relative yearly pattern causes an event to repeat on the same day of the week in the same relative position in a specific month, based on the number of years between each occurrence.</span></span> <span data-ttu-id="b5e64-219">Beispielsweise „jeden letzten Mittwoch im November“.</span><span class="sxs-lookup"><span data-stu-id="b5e64-219">For example, "every last Wednesday of November."</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="b5e64-220">Relevante Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b5e64-220">Relevant properties</span></span>

| <span data-ttu-id="b5e64-221">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b5e64-221">Property</span></span> | <span data-ttu-id="b5e64-222">Relevanz</span><span class="sxs-lookup"><span data-stu-id="b5e64-222">Relevance</span></span> | <span data-ttu-id="b5e64-223">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b5e64-223">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="b5e64-224">**daysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="b5e64-224">**daysOfWeek**</span></span> | <span data-ttu-id="b5e64-225">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="b5e64-225">Required</span></span> | <span data-ttu-id="b5e64-226">Gibt an, an welchem/-n Tag/-en der Woche das Ereignis eintreten kann.</span><span class="sxs-lookup"><span data-stu-id="b5e64-226">Specifies on which day(s) of the week the event can occur.</span></span> <span data-ttu-id="b5e64-227">Relative jährliche Ereignisse treten nur einmal pro Jahr ein, wird also mehr als ein Wert angegeben, fällt das Ereignis auf den ersten Tag, der das Muster erfüllt.</span><span class="sxs-lookup"><span data-stu-id="b5e64-227">Relative yearly events only occur once per year, so if more than one value is specified, the event falls on the first day that satisfies the pattern.</span></span> |
| <span data-ttu-id="b5e64-228">**Index**</span><span class="sxs-lookup"><span data-stu-id="b5e64-228">**index**</span></span> | <span data-ttu-id="b5e64-229">Optional</span><span class="sxs-lookup"><span data-stu-id="b5e64-229">Optional</span></span> | <span data-ttu-id="b5e64-230">Gibt an, in welcher Instanz der zulässigen Tage, die unter **daysOfsWeek** angegeben sind, das Ereignis eintritt, ausgehend von der ersten Instanz des Monats gezählt.</span><span class="sxs-lookup"><span data-stu-id="b5e64-230">Specifies on which instance of the allowed days specified in **daysOfsWeek** the event occurs, counted from the first instance in the month.</span></span> <span data-ttu-id="b5e64-231">Mögliche Werte: `first`, `second`, `third`, `fourth` und `last`.</span><span class="sxs-lookup"><span data-stu-id="b5e64-231">Possible values: `first`, `second`, `third`, `fourth`, and `last`.</span></span> <span data-ttu-id="b5e64-232">Standardwert: `first`.</span><span class="sxs-lookup"><span data-stu-id="b5e64-232">Default value: `first`.</span></span> |
| <span data-ttu-id="b5e64-233">**Monat**</span><span class="sxs-lookup"><span data-stu-id="b5e64-233">**month**</span></span> | <span data-ttu-id="b5e64-234">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="b5e64-234">Required</span></span> | <span data-ttu-id="b5e64-235">Gibt an, in welchem Monat das Ereignis auftritt.</span><span class="sxs-lookup"><span data-stu-id="b5e64-235">Specifies in which month the event occurs.</span></span> |
| <span data-ttu-id="b5e64-236">**Intervall**</span><span class="sxs-lookup"><span data-stu-id="b5e64-236">**interval**</span></span> | <span data-ttu-id="b5e64-237">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="b5e64-237">Required</span></span> | <span data-ttu-id="b5e64-238">Gibt die Anzahl der Jahre zwischen zwei Vorkommen an.</span><span class="sxs-lookup"><span data-stu-id="b5e64-238">Specifies the number of years between each occurrence.</span></span> |
| <span data-ttu-id="b5e64-239">**Typ**</span><span class="sxs-lookup"><span data-stu-id="b5e64-239">**type**</span></span> | <span data-ttu-id="b5e64-240">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="b5e64-240">Required</span></span> | <span data-ttu-id="b5e64-241">Muss auf `relativeMonthly` festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="b5e64-241">Must be set to `relativeMonthly`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="b5e64-242">Beispiele</span><span class="sxs-lookup"><span data-stu-id="b5e64-242">Examples</span></span>

- <span data-ttu-id="b5e64-243">Dieses Ereignis jedes Jahr am letzten Mittwoch im November wiederholen</span><span class="sxs-lookup"><span data-stu-id="b5e64-243">Repeat this event on the last Wednesday of November every year</span></span>

  ```json
    "pattern": {
      "type": "relativeYearly",
      "interval": 1,
      "daysOfWeek": [ "Wednesday" ],
      "index": "last",
      "month": 11
    }
  ```

## <a name="recurrence-ranges"></a><span data-ttu-id="b5e64-244">Serienbereiche</span><span class="sxs-lookup"><span data-stu-id="b5e64-244">Recurrence ranges</span></span>

<span data-ttu-id="b5e64-245">Der zweite Teil einer Serie ist das Muster.</span><span class="sxs-lookup"><span data-stu-id="b5e64-245">The second part of a recurrence is the range.</span></span> <span data-ttu-id="b5e64-246">Dies gibt an, wie lange das Muster wiederholt wird.</span><span class="sxs-lookup"><span data-stu-id="b5e64-246">This specifies how long the pattern repeats.</span></span> <span data-ttu-id="b5e64-247">Ein Ereignis könnte beispielsweise nach 10 Vorkommen an einem bestimmten Datum enden oder kein Ende haben.</span><span class="sxs-lookup"><span data-stu-id="b5e64-247">For example, an event could end after 10 occurrences, by a specific date, or could have no end.</span></span> <span data-ttu-id="b5e64-248">Ein Bereich wird in der API durch die [recurrenceRange-Ressource](../api-reference/v1.0/resources/recurrencepattern.md) dargestellt.</span><span class="sxs-lookup"><span data-stu-id="b5e64-248">A range is represented in the API by the [recurrenceRange resource](../api-reference/v1.0/resources/recurrencepattern.md).</span></span>

<span data-ttu-id="b5e64-249">Je nach Bereichstyp sind bestimmte Felder der **recurrenceRange** obligatorisch oder werden ignoriert.</span><span class="sxs-lookup"><span data-stu-id="b5e64-249">Depending on the type of range, certain fields of **recurrenceRange** are required or ignored.</span></span>

> <span data-ttu-id="b5e64-250">**Hinweis:** Auch wenn ein Feld ignoriert wird, wird es dennoch überprüft.</span><span class="sxs-lookup"><span data-stu-id="b5e64-250">**Note**: Even if a field is ignored, it is still validated.</span></span> <span data-ttu-id="b5e64-251">Wenn ein Feld über eine festgelegte Liste möglicher Werte verfügt, führt ein Wert außerhalb der zulässigen Gruppe von Werten zu einem Fehler, selbst wenn das Feld ignoriert wird.</span><span class="sxs-lookup"><span data-stu-id="b5e64-251">If a field has a set list of possible values, using a value outside the allowed set causes an error, even if that field is ignored.</span></span>

<span data-ttu-id="b5e64-252">Werfen wir einen Blick auf die einzelnen Arten möglicher Bereiche.</span><span class="sxs-lookup"><span data-stu-id="b5e64-252">Let's take a look at each of the possible range types.</span></span>

### <a name="numbered-range"></a><span data-ttu-id="b5e64-253">Nummerierter Bereich</span><span class="sxs-lookup"><span data-stu-id="b5e64-253">Numbered range</span></span>

<span data-ttu-id="b5e64-254">Der nummerierte Bereich bewirkt, dass ein Ereignis eine feste Anzahl von Vorkommen (basierend auf dem Muster) ab einem Startdatum auftritt.</span><span class="sxs-lookup"><span data-stu-id="b5e64-254">The numbered range causes an event to occur a fixed number of times (based on the pattern) from a start date.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="b5e64-255">Relevante Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b5e64-255">Relevant properties</span></span>

| <span data-ttu-id="b5e64-256">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b5e64-256">Property</span></span> | <span data-ttu-id="b5e64-257">Relevanz</span><span class="sxs-lookup"><span data-stu-id="b5e64-257">Relevance</span></span> | <span data-ttu-id="b5e64-258">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b5e64-258">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="b5e64-259">**numberOfOccurences**</span><span class="sxs-lookup"><span data-stu-id="b5e64-259">**numberOfOccurences**</span></span> | <span data-ttu-id="b5e64-260">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="b5e64-260">Required</span></span> | <span data-ttu-id="b5e64-261">Gibt die Anzahl von Vorkommen an.</span><span class="sxs-lookup"><span data-stu-id="b5e64-261">Specifies the number of occurrences.</span></span> <span data-ttu-id="b5e64-262">Das Vorkommen muss eine positive ganze Zahl sein.</span><span class="sxs-lookup"><span data-stu-id="b5e64-262">Must be a positive integer.</span></span> |
| <span data-ttu-id="b5e64-263">**recurrenceTimeZone**</span><span class="sxs-lookup"><span data-stu-id="b5e64-263">**recurrenceTimeZone**</span></span> | <span data-ttu-id="b5e64-264">Optional</span><span class="sxs-lookup"><span data-stu-id="b5e64-264">Optional</span></span> | <span data-ttu-id="b5e64-265">Gibt die Zeitzone für die **StartDate**-Eigenschaft an.</span><span class="sxs-lookup"><span data-stu-id="b5e64-265">Specifies the time zone for the **startDate** property.</span></span> <span data-ttu-id="b5e64-266">Falls nicht angegeben, wird die Zeitzone des Ereignisses verwendet.</span><span class="sxs-lookup"><span data-stu-id="b5e64-266">If not specified, the time zone of the event is used.</span></span> |
| <span data-ttu-id="b5e64-267">**startDate**</span><span class="sxs-lookup"><span data-stu-id="b5e64-267">**startDate**</span></span> | <span data-ttu-id="b5e64-268">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="b5e64-268">Required</span></span> | <span data-ttu-id="b5e64-269">Gibt das Datum des Starts des Anwendens des Musters an.</span><span class="sxs-lookup"><span data-stu-id="b5e64-269">Specifies the date to start applying the pattern.</span></span> <span data-ttu-id="b5e64-270">Der Wert von **StartDate** MUSS dem Datumswert der **Start**-Eigenschaft der [Ereignisressource](../api-reference/v1.0/resources/event.md) entsprechen.</span><span class="sxs-lookup"><span data-stu-id="b5e64-270">The value of **startDate** MUST correspond to the date value of the **start** property on the [event resource](../api-reference/v1.0/resources/event.md).</span></span> <span data-ttu-id="b5e64-271">Hinweis: Das erste Vorkommen der Besprechung kann nicht an diesem Datum stattfinden, wenn es nicht in das Muster passt.</span><span class="sxs-lookup"><span data-stu-id="b5e64-271">Note that the first occurrence of the meeting may not occur on this date if it does not fit the pattern.</span></span> |
| <span data-ttu-id="b5e64-272">**Typ**</span><span class="sxs-lookup"><span data-stu-id="b5e64-272">**type**</span></span> | <span data-ttu-id="b5e64-273">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="b5e64-273">Required</span></span> | <span data-ttu-id="b5e64-274">Muss auf `numbered` festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="b5e64-274">Must be set to `numbered`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="b5e64-275">Beispiele</span><span class="sxs-lookup"><span data-stu-id="b5e64-275">Examples</span></span>

- <span data-ttu-id="b5e64-276">Dieses Ereignis 10 Mal wiederholen</span><span class="sxs-lookup"><span data-stu-id="b5e64-276">Repeat this event 10 times</span></span>

  ```json
    "range": {
      "type": "numbered",
      "startDate": "2017-04-02",
      "numberOfOccurrences": 10
    }
  ```

### <a name="end-date-range"></a><span data-ttu-id="b5e64-277">Enddatumsbereich</span><span class="sxs-lookup"><span data-stu-id="b5e64-277">End date range</span></span>

<span data-ttu-id="b5e64-278">Der Enddatumsbereich bewirkt, dass ein Ereignis an allen Tagen eintritt, die das entsprechende Muster zwischen einem Startdatum und einem Enddatum aufweisen.</span><span class="sxs-lookup"><span data-stu-id="b5e64-278">The end date range causes an event to occur on all days that fit the applicable pattern between a start date and an end date.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="b5e64-279">Relevante Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b5e64-279">Relevant properties</span></span>

| <span data-ttu-id="b5e64-280">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b5e64-280">Property</span></span> | <span data-ttu-id="b5e64-281">Relevanz</span><span class="sxs-lookup"><span data-stu-id="b5e64-281">Relevance</span></span> | <span data-ttu-id="b5e64-282">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b5e64-282">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="b5e64-283">**endDate**</span><span class="sxs-lookup"><span data-stu-id="b5e64-283">**endDate**</span></span> | <span data-ttu-id="b5e64-284">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="b5e64-284">Required</span></span> | <span data-ttu-id="b5e64-285">Gibt das Datum zum Beenden des Anwendens des Musters an.</span><span class="sxs-lookup"><span data-stu-id="b5e64-285">Specifies the date to stop applying the pattern.</span></span> <span data-ttu-id="b5e64-286">Hinweis: Das letzte Vorkommen der Besprechung kann nicht an diesem Datum auftreten, wenn es nicht in das Muster passt.</span><span class="sxs-lookup"><span data-stu-id="b5e64-286">Note that the last occurrence of the meeting may not occur on this date if it does not fit the pattern.</span></span> |
| <span data-ttu-id="b5e64-287">**recurrenceTimeZone**</span><span class="sxs-lookup"><span data-stu-id="b5e64-287">**recurrenceTimeZone**</span></span> | <span data-ttu-id="b5e64-288">Optional</span><span class="sxs-lookup"><span data-stu-id="b5e64-288">Optional</span></span> | <span data-ttu-id="b5e64-289">Gibt die Zeitzone für die **startDate**- und **endDate**-Eigenschaften an.</span><span class="sxs-lookup"><span data-stu-id="b5e64-289">Specifies the time zone for the **startDate** and **endDate** properties.</span></span> <span data-ttu-id="b5e64-290">Falls nicht angegeben, wird die Zeitzone des Ereignisses verwendet.</span><span class="sxs-lookup"><span data-stu-id="b5e64-290">If not specified, the time zone of the event is used.</span></span> |
| <span data-ttu-id="b5e64-291">**startDate**</span><span class="sxs-lookup"><span data-stu-id="b5e64-291">**startDate**</span></span> | <span data-ttu-id="b5e64-292">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="b5e64-292">Required</span></span> | <span data-ttu-id="b5e64-293">Gibt das Datum des Starts des Anwendens des Musters an.</span><span class="sxs-lookup"><span data-stu-id="b5e64-293">Specifies the date to start applying the pattern.</span></span> <span data-ttu-id="b5e64-294">Der Wert von **StartDate** MUSS dem Datumswert der **Start**-Eigenschaft der [Ereignisressource](../api-reference/v1.0/resources/event.md) entsprechen.</span><span class="sxs-lookup"><span data-stu-id="b5e64-294">The value of **startDate** MUST correspond to the date value of the **start** property on the [event resource](../api-reference/v1.0/resources/event.md).</span></span> <span data-ttu-id="b5e64-295">Hinweis: Das erste Vorkommen der Besprechung kann nicht an diesem Datum stattfinden, wenn es nicht in das Muster passt.</span><span class="sxs-lookup"><span data-stu-id="b5e64-295">Note that the first occurrence of the meeting may not occur on this date if it does not fit the pattern.</span></span> |
| <span data-ttu-id="b5e64-296">**Typ**</span><span class="sxs-lookup"><span data-stu-id="b5e64-296">**type**</span></span> | <span data-ttu-id="b5e64-297">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="b5e64-297">Required</span></span> | <span data-ttu-id="b5e64-298">Muss auf **EndDate** festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="b5e64-298">Must be set to **endDate**.</span></span> |

#### <a name="examples"></a><span data-ttu-id="b5e64-299">Beispiele</span><span class="sxs-lookup"><span data-stu-id="b5e64-299">Examples</span></span>

- <span data-ttu-id="b5e64-300">Dieses Ereignis vom 1. Juli 2017 bis zum 31. Juli 2017 wiederholen</span><span class="sxs-lookup"><span data-stu-id="b5e64-300">Repeat this event from July 1, 2017, to July 31, 2017</span></span>

  ```json
    "range": {
      "type": "endDate",
      "startDate": "2017-07-01",
      "endDate": "2017-07-31"
    }
  ```

### <a name="no-end-range"></a><span data-ttu-id="b5e64-301">Kein Endbereich</span><span class="sxs-lookup"><span data-stu-id="b5e64-301">No end range</span></span>

<span data-ttu-id="b5e64-302">Der Enddatumsbereich bewirkt, dass ein Ereignis an allen Tagen eintritt, die dem anwendbaren Muster nach einem Startdatum entsprechen.</span><span class="sxs-lookup"><span data-stu-id="b5e64-302">The no end range causes an event to occur on all days that fit the applicable pattern after a start date.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="b5e64-303">Relevante Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b5e64-303">Relevant properties</span></span>

| <span data-ttu-id="b5e64-304">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b5e64-304">Property</span></span> | <span data-ttu-id="b5e64-305">Relevanz</span><span class="sxs-lookup"><span data-stu-id="b5e64-305">Relevance</span></span> | <span data-ttu-id="b5e64-306">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b5e64-306">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="b5e64-307">**recurrenceTimeZone**</span><span class="sxs-lookup"><span data-stu-id="b5e64-307">**recurrenceTimeZone**</span></span> | <span data-ttu-id="b5e64-308">Optional</span><span class="sxs-lookup"><span data-stu-id="b5e64-308">Optional</span></span> | <span data-ttu-id="b5e64-309">Gibt die Zeitzone für die **StartDate**-Eigenschaft an.</span><span class="sxs-lookup"><span data-stu-id="b5e64-309">Specifies the time zone for the **startDate** property.</span></span> <span data-ttu-id="b5e64-310">Falls nicht angegeben, wird die Zeitzone des Ereignisses verwendet.</span><span class="sxs-lookup"><span data-stu-id="b5e64-310">If not specified, the time zone of the event is used.</span></span> |
| <span data-ttu-id="b5e64-311">**startDate**</span><span class="sxs-lookup"><span data-stu-id="b5e64-311">**startDate**</span></span> | <span data-ttu-id="b5e64-312">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="b5e64-312">Required</span></span> | <span data-ttu-id="b5e64-313">Gibt das Datum des Starts des Anwendens des Musters an.</span><span class="sxs-lookup"><span data-stu-id="b5e64-313">Specifies the date to start applying the pattern.</span></span> <span data-ttu-id="b5e64-314">Der Wert von **StartDate** MUSS dem Datumswert der **Start**-Eigenschaft der [Ereignisressource](../api-reference/v1.0/resources/event.md) entsprechen.</span><span class="sxs-lookup"><span data-stu-id="b5e64-314">The value of **startDate** MUST correspond to the date value of the **start** property on the [event resource](../api-reference/v1.0/resources/event.md).</span></span> <span data-ttu-id="b5e64-315">Hinweis: Das erste Vorkommen der Besprechung kann nicht an diesem Datum stattfinden, wenn es nicht in das Muster passt.</span><span class="sxs-lookup"><span data-stu-id="b5e64-315">Note that the first occurrence of the meeting may not occur on this date if it does not fit the pattern.</span></span> |
| <span data-ttu-id="b5e64-316">**Typ**</span><span class="sxs-lookup"><span data-stu-id="b5e64-316">**type**</span></span> | <span data-ttu-id="b5e64-317">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="b5e64-317">Required</span></span> | <span data-ttu-id="b5e64-318">Muss auf `noEnd` festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="b5e64-318">Must be set to `noEnd`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="b5e64-319">Beispiele</span><span class="sxs-lookup"><span data-stu-id="b5e64-319">Examples</span></span>

- <span data-ttu-id="b5e64-320">Dieses Ereignis ab dem 15. Mai 2017 immer wiederholen</span><span class="sxs-lookup"><span data-stu-id="b5e64-320">Repeat this event from May 15, 2017, forever</span></span>

  ```json
    "range": {
      "type": "noEnd",
      "startDate": "2017-05-15"
    }
  ```

## <a name="using-patterns-and-ranges-to-create-recurring-events"></a><span data-ttu-id="b5e64-321">Verwenden von Mustern und Bereichen zum Erstellen von Ereignisserien</span><span class="sxs-lookup"><span data-stu-id="b5e64-321">Using patterns and ranges to create recurring events</span></span>

<span data-ttu-id="b5e64-322">Nachdem wir uns nun Muster und Bereiche separat angesehen haben, schauen wir uns nun deren Zusammenwirken und Interagieren mit den **Start**- und **End**-Eigenschaften zu dem Ereignis an.</span><span class="sxs-lookup"><span data-stu-id="b5e64-322">Now that we've looked at patterns and ranges separately, let's look at how they work together and how they interact with the **start** and **end** properties on the event.</span></span>

### <a name="creating-a-recurrence-rule"></a><span data-ttu-id="b5e64-323">Erstellen einer Serienregel</span><span class="sxs-lookup"><span data-stu-id="b5e64-323">Creating a recurrence rule</span></span>

<span data-ttu-id="b5e64-324">Um eine Serienregel zu erstellen, müssen Sie sowohl ein Muster als auch einen Bereich angeben.</span><span class="sxs-lookup"><span data-stu-id="b5e64-324">To create a recurrence rule, you must specify both a pattern and a range.</span></span> <span data-ttu-id="b5e64-325">Jeder Mustertyp kann mit einem beliebigen Bereichstyp arbeiten.</span><span class="sxs-lookup"><span data-stu-id="b5e64-325">Any pattern type can work with any range type.</span></span> <span data-ttu-id="b5e64-326">Im Anschluss finden Sie einige Beispiele:</span><span class="sxs-lookup"><span data-stu-id="b5e64-326">Here are a few examples.</span></span>

#### <a name="examples"></a><span data-ttu-id="b5e64-327">Beispiele</span><span class="sxs-lookup"><span data-stu-id="b5e64-327">Examples</span></span>

- <span data-ttu-id="b5e64-328">**Besprechung von 13:00-13:30 Uhr, jeden Montag ab dem 4. September 2017 bis zum Ende des Jahres**</span><span class="sxs-lookup"><span data-stu-id="b5e64-328">**Meet from 1:00 PM to 1:30 PM every Monday starting September 4, 2017, until the end of the year**</span></span>

  - <span data-ttu-id="b5e64-329">Die Anforderung „jeden Montag“ wird ganz einfach durch den `weekly`-Serienmustertyp erfüllt.</span><span class="sxs-lookup"><span data-stu-id="b5e64-329">The "every Monday" requirement is easily met by the `weekly` recurrence pattern type.</span></span>
  - <span data-ttu-id="b5e64-330">Die Anforderung „bis zum Ende des Jahres“ gibt einen `endDate`-Serienbereichstypen an.</span><span class="sxs-lookup"><span data-stu-id="b5e64-330">The "until the end of the year" requirement indicates an `endDate` recurrence range type.</span></span>

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

  <span data-ttu-id="b5e64-331">Da der 31. Dezember 2017 auf einen Sonntag fällt, ist das letzte Vorkommen in dieser Serie am Montag, den 25. Dezember.</span><span class="sxs-lookup"><span data-stu-id="b5e64-331">Because December 31, 2017, is on a Sunday, the last occurrence in this series will be on Monday, December 25.</span></span>

- <span data-ttu-id="b5e64-332">**Besprechung von 14:00-15:00 Uhr am ersten Donnerstag jeden zweiten Monat, ab dem 29. August 2017**</span><span class="sxs-lookup"><span data-stu-id="b5e64-332">**Meet from 2:00 PM to 3:00 PM on the first Thursday of every other month starting August 29, 2017**</span></span>

  - <span data-ttu-id="b5e64-333">Die Anforderung „erster Donnerstag jeden zweiten Monat“ kann durch ein relatives monatliches Muster erfüllt werden.</span><span class="sxs-lookup"><span data-stu-id="b5e64-333">The "first Thursday of every other month" requirement is achievable by using a relative monthly pattern.</span></span> <span data-ttu-id="b5e64-334">Der Teil „jeden zweiten Monats“ gibt an, dass das **Intervall** auf `2` festgelegt werden sollte.</span><span class="sxs-lookup"><span data-stu-id="b5e64-334">The "every other month" portion indicates that the **interval** should be set to `2`.</span></span>
  - <span data-ttu-id="b5e64-335">Da es keine Anforderung an ein Enddatum gibt, kann ein `noEnd`-Bereichstyp verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="b5e64-335">Because there is no requirement on an end date, a `noEnd` range type can be used.</span></span>

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

  <span data-ttu-id="b5e64-336">Da der Wert von **startDate** nach dem ersten Donnerstag im August liegt, ist das erste Vorkommen dieser Serie im September.</span><span class="sxs-lookup"><span data-stu-id="b5e64-336">Because the value of **startDate** is after the first Thursday in August, the first occurrence of this series will be in September.</span></span>

## <a name="next-steps"></a><span data-ttu-id="b5e64-337">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="b5e64-337">Next steps</span></span>
    
<span data-ttu-id="b5e64-338">Erfahren Sie mehr zur [Integration in Outlook-Kalender](outlook-calendar-concept-overview.md).</span><span class="sxs-lookup"><span data-stu-id="b5e64-338">Find out more about [integrating with Outlook calendar](outlook-calendar-concept-overview.md).</span></span>
