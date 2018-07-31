# <a name="get-incremental-changes-for-groups"></a><span data-ttu-id="7f861-101">Dient zum Abrufen inkrementeller Änderungen für Gruppen.</span><span class="sxs-lookup"><span data-stu-id="7f861-101">Get incremental changes for groups</span></span>

<span data-ttu-id="7f861-p101">Mit der [Delta-Abfrage](./delta_query_overview.md) können Sie Ergänzungen, Löschungen oder Aktualisierungen an Gruppen anhand von einer Serie von [Delta](../api-reference/v1.0/api/group_delta.md)-Funktionsaufrufen abfragen. Mit der Delta-Abfrage können Sie Änderungen an Gruppen ermitteln, ohne den gesamten Satz von Gruppen von Microsoft Graph abrufen und Änderungen vergleichen zu müssen.</span><span class="sxs-lookup"><span data-stu-id="7f861-p101">[Delta query](./delta_query_overview.md) lets you query for additions, deletions, or updates to groups, by way of a series of [delta](../api-reference/v1.0/api/group_delta.md) function calls. Delta query enables you discover changes to groups without having to fetch the entire set of groups from Microsoft Graph and compare changes.</span></span>

<span data-ttu-id="7f861-p102">Clients, die Gruppen mit einem lokalen Profilspeicher synchronisieren, können Delta Abfragen für die anfängliche vollständige Synchronisierung und für inkrementelle Synchronisierungen in der Zukunft verwenden. In der Regel führt ein Client eine anfängliche vollständige Synchronisierung aller Gruppen in einem Mandanten durch und ruft anschließend regelmäßig inkrementelle Änderungen an Gruppen ab.</span><span class="sxs-lookup"><span data-stu-id="7f861-p102">Clients using synchronizing groups with a local profile store can use Delta Query for both their initial full synchronization along with incremental synchronizations in the future. Typically, a client would do an initial full synchronization of all the groups in a tenant, and subsequently, get incremental changes to groups periodically.</span></span>

## <a name="tracking-group-changes"></a><span data-ttu-id="7f861-106">Nachverfolgen von Gruppenänderungen</span><span class="sxs-lookup"><span data-stu-id="7f861-106">Tracking group changes</span></span>

<span data-ttu-id="7f861-p103">Das Nachverfolgen von Gruppenänderungen ist eine Runde von einer oder mehreren GET-Anforderungen mit der **Delta**-Funktion. Eine GET-Anforderung wird ähnlich wie das [Auflisten von Gruppen](../api-reference/v1.0/api/group_list.md) durchgeführt, außer dass Folgendes eingeschlossen wird:</span><span class="sxs-lookup"><span data-stu-id="7f861-p103">Tracking group changes is a round of one or more GET requests with the **delta** function. You make a GET request much like the way you [list groups](../api-reference/v1.0/api/group_list.md), except that you include the following:</span></span>

- <span data-ttu-id="7f861-109">Die **Delta**-Funktion.</span><span class="sxs-lookup"><span data-stu-id="7f861-109">The **delta** function.</span></span>
- <span data-ttu-id="7f861-110">Ein [Statustoken](./delta_query_overview.md) (*deltaToken* oder *skipToken*) aus dem vorherigen GET-**Delta**-Funktionsaufruf.</span><span class="sxs-lookup"><span data-stu-id="7f861-110">A [state token](./delta_query_overview.md) (*deltaToken* or *skipToken*) from the previous GET **delta** function call.</span></span>

## <a name="example"></a><span data-ttu-id="7f861-111">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7f861-111">Example</span></span>

<span data-ttu-id="7f861-112">Das folgende Beispiel zeigt eine Serienanforderung zum Nachverfolgen von Änderungen an Gruppen:</span><span class="sxs-lookup"><span data-stu-id="7f861-112">The following example shows a series  requests to track changes to groups:</span></span>

1. <span data-ttu-id="7f861-113">[Ursprüngliche Anforderung](#initial-request) und [Antwort](#initial-response)</span><span class="sxs-lookup"><span data-stu-id="7f861-113">[Initial request](#initial-request) and [response](#initial-response)</span></span>
2. <span data-ttu-id="7f861-114">[nextLink-Anforderung](#nextlink-request) und [Antwort](#nextlink-response)</span><span class="sxs-lookup"><span data-stu-id="7f861-114">[nextLink request](#nextlink-request) and [response](#nextlink-response)</span></span>
3. <span data-ttu-id="7f861-115">[Letzte nextLink-Anforderung](#final-nextlink-request) und [Antwort](#final-nextlink-response)</span><span class="sxs-lookup"><span data-stu-id="7f861-115">[Final nextLink request](#final-nextlink-request) and [response](#final-nextlink-response)</span></span>
4. <span data-ttu-id="7f861-116">[deltaLink-Anforderung](#deltalink-request) und [deltaLink-Antwort](#deltalink-response)</span><span class="sxs-lookup"><span data-stu-id="7f861-116">[deltaLink request](#deltalink-request) and [deltaLink response](#deltalink-response)</span></span>

## <a name="initial-request"></a><span data-ttu-id="7f861-117">Ursprüngliche Anforderung</span><span class="sxs-lookup"><span data-stu-id="7f861-117">Initial request</span></span>

<span data-ttu-id="7f861-118">Um Änderungen an der Gruppenressource nachzuverfolgen, nehmen Sie zunächst eine Anforderung einschließlich der Delta-Funktion für die Gruppenressource vor.</span><span class="sxs-lookup"><span data-stu-id="7f861-118">To begin tracking changes in the group resource, you make a request including the delta function on the group resource.</span></span>

<span data-ttu-id="7f861-119">Beachten Sie Folgendes:</span><span class="sxs-lookup"><span data-stu-id="7f861-119">Note the following:</span></span>

- <span data-ttu-id="7f861-120">Der optionale `$select`-Abfrageparameter wird in die Anforderung eingeschlossen, um zu veranschaulichen, wie Abfrageparameter automatisch in zukünftige Anforderungen eingeschlossen werden.</span><span class="sxs-lookup"><span data-stu-id="7f861-120">The optional $select query parameter is included in the request to demonstrate how query parameters are automatically included in future requests.</span></span>
- <span data-ttu-id="7f861-121">Der optionale `$expand`-Abfrageparameter wird eingeschlossen, um anzuzeigen, wie Mitglieder der Gruppe zusammen mit Objekten der Gruppe abgerufen werden können.</span><span class="sxs-lookup"><span data-stu-id="7f861-121">The optional `$expand` query parameter is included to show how group members can be retrieved together with group objects.</span></span> <span data-ttu-id="7f861-122">Dadurch können Änderungen der Mitgliedschaft nachverfolgt werden, wenn z. B. Benutzer zu Gruppen hinzugefügt oder daraus entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="7f861-122">This allows tracking of membership changes, such as when users are added or removed from groups.</span></span>
- <span data-ttu-id="7f861-p105">Die ursprüngliche Anforderung enthält kein Statustoken. Statustoken werden in nachfolgenden Anforderungen verwendet.</span><span class="sxs-lookup"><span data-stu-id="7f861-p105">The initial request does not include a state token. State tokens will be used in subsequent requests.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description&$expand=members
```

## <a name="initial-response"></a><span data-ttu-id="7f861-125">Ursprüngliche Antwort</span><span class="sxs-lookup"><span data-stu-id="7f861-125">Initial response</span></span>

<span data-ttu-id="7f861-126">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [group](../api-reference/v1.0/resources/group.md)-Sammlungsobjekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7f861-126">If successful, this method returns `200 OK` response code and [group](../api-reference/v1.0/resources/group.md) object in the response body.</span></span> <span data-ttu-id="7f861-127">Wenn der gesamte Gruppensatz zu groß ist, um in eine Antwort zu passen, wird ebenfalls ein `nextLink` mit einem Statustoken eingeschlossen.</span><span class="sxs-lookup"><span data-stu-id="7f861-127">If the entire set of groups is too large to fit in one response, a `nextLink` containing a state token will also be included.</span></span>

<span data-ttu-id="7f861-128">In diesem Beispiel wurde ein `nextLink` eingeschlossen; die ursprünglichen `$select`- und `$expand`-Abfrageparameter werden im Statustoken codiert.</span><span class="sxs-lookup"><span data-stu-id="7f861-128">In this example, a `nextLink` was included; the original `$select` and `$expand` query parameters are encoded in the state token.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups(displayName,description)",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjvB7XnF_yllFsCrZJ",
  "value": [
    {
      "displayName":"TestGroup1",
      "description":"Employees in test group 1",
      "id":"c2f798fd-f95d-4623-8824-63aec21fffff",
      "members@delta": [
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "693acd06-2877-4339-8ade-b704261fe7a0"
               },
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "49320844-be99-4164-8167-87ff5d047ace"
               }
      ]
    },
    {
      "displayName":"TestGroup2",
      "description":"Employees in test group 2",
      "id":"ec22655c-8eb2-432a-b4ea-8b8a254bffff"
    }
  ]
}
```

><span data-ttu-id="7f861-129">**Hinweis:** Die `members@delta`-Eigenschaft ist im ersten Gruppenobjekts – TestGroup1 – enthalten und enthält die beiden aktuellen Mitglieder der Gruppe.</span><span class="sxs-lookup"><span data-stu-id="7f861-129">**Note:** The `members@delta` property is included in the first group object - TestGroup1 - and contains the two current members of the group.</span></span> <span data-ttu-id="7f861-130">TestGroup2 enthält diese Eigenschaft nicht, da die Gruppe keine Mitglieder besitzt.</span><span class="sxs-lookup"><span data-stu-id="7f861-130">TestGroup2 does not contain that property because the group does not have any members.</span></span>

## <a name="nextlink-request"></a><span data-ttu-id="7f861-131">nextLink-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7f861-131">nextLink request</span></span>

<span data-ttu-id="7f861-132">Die zweite Anforderung verwendet `nextLink` aus der vorherigen Antwort, die `skipToken` enthält.</span><span class="sxs-lookup"><span data-stu-id="7f861-132">The second request uses the `nextLink` from the previous response, which contains the `skipToken`.</span></span> <span data-ttu-id="7f861-133">Beachten Sie, dass die `$select`- und `$expand` -Parameter nicht explizit vorhanden sind, da sie im Token codiert werden.</span><span class="sxs-lookup"><span data-stu-id="7f861-133">Notice the `$select` and `$expand` parameters are not explicitly present as they are encoded in the token.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjvB7XnF_yllFsCrZJ
```

## <a name="nextlink-response"></a><span data-ttu-id="7f861-134">nextLink-Antwort</span><span class="sxs-lookup"><span data-stu-id="7f861-134">nextLink response</span></span>

<span data-ttu-id="7f861-135">Die Antwort enthält ein weiteres `nextLink` mit einem neuen `skipToken`-Wert, wodurch angegeben wird, dass weitere Gruppen verfügbar sind.</span><span class="sxs-lookup"><span data-stu-id="7f861-135">The response contains another `nextLink` with a new `skipToken` value, indicating there are more groups available.</span></span> <span data-ttu-id="7f861-136">Sie nehmen weiterhin Anforderungen über die `nextLink`-URL vor, bis eine `deltaLink`-URL in der endgültigen Antwort zurückgegeben wird.</span><span class="sxs-lookup"><span data-stu-id="7f861-136">The response contains a  and another , indicating there are more groups available. You continue making requests using the nextLink URL until a deltaLink URL is returned in the response.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjtQ5LOhVoS7qQG_wdVCHHlbQpga7",
  "value": [
    {
      "displayName":"TestGroup3",
      "description":"Employees in test group 3",
      "id":"2e5807ce-58f3-4a94-9b37-ffff2e085957",
      "members@delta": [
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "632f6bb2-3ec8-4c1f-9073-0027a8c68593"
               }
      ]
    },
    {
      "displayName":"TestGroup4",
      "description":"Employees in test group 4",
      "id":"421e797f-9406-4934-b778-4908421e3505",
      "members@delta": [
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "3c8ac7c4-d365-4df9-abfa-356a9dd7763c"
               },
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "49320844-be99-4164-8167-87ff5d047ace"
               }
      ]
    }
  ]
}
```

## <a name="final-nextlink-request"></a><span data-ttu-id="7f861-137">Letzte nextLink-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7f861-137">Final nextLink request</span></span>

<span data-ttu-id="7f861-138">Die dritte Anforderung verwendet erneut die neueste `nextLink`.</span><span class="sxs-lookup"><span data-stu-id="7f861-138">The third request again uses the latest `nextLink`.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=ppqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjtQ5LOhVoS7qQG_wdVCHHlbQpga7
```

## <a name="final-nextlink-response"></a><span data-ttu-id="7f861-139">Letzte nextLink-Antwort</span><span class="sxs-lookup"><span data-stu-id="7f861-139">Final nextLink response</span></span>

<span data-ttu-id="7f861-140">Zum Schluss wird die `deltaLink`-URL zurückgegeben, was bedeutet, dass keine weitere Daten für den vorhandenen Status von Gruppen vorhanden sind.</span><span class="sxs-lookup"><span data-stu-id="7f861-140">Finally, the `deltaLink` URL is returned, which means there is no more data for the existing state of groups.</span></span> <span data-ttu-id="7f861-141">Für künftige Anforderungen verwendet die Anwendung die enthaltenen Werte `deltaLink` und `deltaToken`, um neue Änderungen an Gruppen abzufragen.</span><span class="sxs-lookup"><span data-stu-id="7f861-141">For future requests, the application uses the `deltaLink` and the `deltaToken` value it contains to learn about new changes to groups.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw",
  "value": [
    {
      "displayName":"TestGroup5",
      "description":"Employees in test group 5",
      "id":"bed7f0d4-750e-4e7e-ffff-169002d06fc9"
    },
    {
      "displayName":"TestGroup6",
      "description":"Employees in test group 6",
      "id":"421e797f-9406-ffff-b778-4908421e3505"
    }
  ]
}
```

## <a name="deltalink-request"></a><span data-ttu-id="7f861-142">deltaLink-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7f861-142">deltaLink request</span></span>

<span data-ttu-id="7f861-143">Mit dem `deltaLink` aus der [letzten Antwort](#final-nextlink-response) können Sie seit der letzten Anforderung vorgenommene Änderungen an Gruppen abrufen.</span><span class="sxs-lookup"><span data-stu-id="7f861-143">Using the `deltaLink` from the [last response](#final-nextlink-response), you will be able to get changed (by being added, deleted, or updated) groups since the last request.</span></span> <span data-ttu-id="7f861-144">Dazu gehören:</span><span class="sxs-lookup"><span data-stu-id="7f861-144">Changes include:</span></span>
- <span data-ttu-id="7f861-145">Neu erstelle Gruppenobjekte</span><span class="sxs-lookup"><span data-stu-id="7f861-145">Newly created group objects.</span></span>
- <span data-ttu-id="7f861-146">Gelöschte Gruppenobjekte</span><span class="sxs-lookup"><span data-stu-id="7f861-146">Deleted group objects.</span></span>
- <span data-ttu-id="7f861-147">Gruppenobjekte, für die eine Eigenschaft geändert wurde (z. B. **displayName** wurde geändert).</span><span class="sxs-lookup"><span data-stu-id="7f861-147">Group objects for which a property has changed (e.g. **displayName** has been modified).</span></span>
- <span data-ttu-id="7f861-148">Gruppenobjekte, für die Mitgliedsobjekte hinzugefügt oder entfernt wurden.</span><span class="sxs-lookup"><span data-stu-id="7f861-148">Group objects for which member objects have been added or removed.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw
```

## <a name="deltalink-response"></a><span data-ttu-id="7f861-149">deltaLink-Antwort</span><span class="sxs-lookup"><span data-stu-id="7f861-149">deltaLink response</span></span>

<span data-ttu-id="7f861-150">Falls keine Änderungen vorgenommen wurden, wird `deltaLink` ohne Ergebnisse zurückgegeben – die Eigenschaft `value` ist leer.</span><span class="sxs-lookup"><span data-stu-id="7f861-150">If no changes have occurred, a `deltaLink` is returned with no results - the `value` property is empty.</span></span> <span data-ttu-id="7f861-151">Stellen Sie sicher, dass Sie den vorherigen Link in der Anwendung durch den neuen für die Verwendung in kommenden Anrufen ersetzen.</span><span class="sxs-lookup"><span data-stu-id="7f861-151">Make sure to replace the previous link in the application with the new one for use in future calls.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw",
  "value": []
}
```

<span data-ttu-id="7f861-152">Wenn Änderungen vorgenommen wurden, ist eine Sammlung der geänderten Gruppen enthalten.</span><span class="sxs-lookup"><span data-stu-id="7f861-152">If changes have occurred, the same  is returned including a collection of changed groups.</span></span> <span data-ttu-id="7f861-153">Die Antwort enthält zudem `nextLink` – falls mehrere Seiten mit Änderungen abgerufen werden müssen – oder `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="7f861-153">The response also contains either a `nextLink` - in case there are multiple pages of changes to retrieve - or a `deltaLink`.</span></span> <span data-ttu-id="7f861-154">Sie sollten nach `nextLinks` das gleiche Muster implementieren wie zuvor und die endgültige Eigenschaft `deltaLink` für zukünftige Anrufe beibehalten.</span><span class="sxs-lookup"><span data-stu-id="7f861-154">You should implement the same pattern of following the `nextLinks` as before and persist the final `deltaLink` for future calls.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw",
  "value": [
          {
              "displayName": "TestGroup3",
              "description": "A test group for change tracking",
              "id": "2e5807ce-58f3-4a94-9b37-ffff2e085957",
              "members@delta": [
                  {
                      "@odata.type": "#microsoft.graph.user",
                      "id": "632f6bb2-3ec8-4c1f-9073-0027a8c6859",
                      "@removed": {
                          "reason": "deleted"
                      }
                  },
                  {
                      "@odata.type": "#microsoft.graph.user",
                      "id": "37de1ae3-408f-4702-8636-20824abda004"
                  }
              ]
          }
      ]
}
```
<span data-ttu-id="7f861-155">Einige Punkte, die Sie bei der oben aufgeführten Beispielantwort beachten sollten:</span><span class="sxs-lookup"><span data-stu-id="7f861-155">Some things to note about the example response above:</span></span>
- <span data-ttu-id="7f861-156">Die Objekte werden mit demselben Eigenschaftensatz zurückgegeben, der ursprünglich mit den Abfrageparametern `$select` und `$expand` angegeben wurde.</span><span class="sxs-lookup"><span data-stu-id="7f861-156">The objects are returned with the same set of properties originally specified via the `$select` and `$expand` query parameters.</span></span>
- <span data-ttu-id="7f861-157">Es sind sowohl geänderte als auch nicht geänderte Eigenschaften enthalten.</span><span class="sxs-lookup"><span data-stu-id="7f861-157">Both changed and unchanged properties are included.</span></span> <span data-ttu-id="7f861-158">Im Beispiel oben hat die Eigenschaft `description` einen neuen Wert, während die Eigenschaft `displayName` nicht geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="7f861-158">In the example above, the `description` property has a new value, while the `displayName` property has not changed.</span></span>
- <span data-ttu-id="7f861-159">`members@delta` enthält alle Änderungen an der Mitgliedschaft.</span><span class="sxs-lookup"><span data-stu-id="7f861-159">`members@delta` contains any changes to membership.</span></span>
  - <span data-ttu-id="7f861-160">Der erste Benutzer in der Liste wurde aus der Gruppe entfernt – entweder durch Entfernen der Mitgliedschaft oder durch Löschen des Benutzerobjekts selbst.</span><span class="sxs-lookup"><span data-stu-id="7f861-160">The first user in the list has been removed from the group - either by removing the membership or by deleting the user object itself.</span></span> <span data-ttu-id="7f861-161">Die Eigenschaft `@removed` beschreibt dies.</span><span class="sxs-lookup"><span data-stu-id="7f861-161">The `@removed` property describes that.</span></span>
  - <span data-ttu-id="7f861-162">Der zweite Benutzer wurde zur Gruppe hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="7f861-162">The second user has been added to the group.</span></span>

## <a name="paging-through-members-in-a-large-group"></a><span data-ttu-id="7f861-163">Blättern durch Mitglieder in einer großen Gruppe</span><span class="sxs-lookup"><span data-stu-id="7f861-163">Paging through members in a large group</span></span>
<span data-ttu-id="7f861-164">Die Eigenschaft `members@delta` ist standardmäßig in Gruppenobjekten enthalten, wenn der Abfrageparameter `$select` nicht angegeben oder der Parameter `$expand=members` explizit angegeben wird.</span><span class="sxs-lookup"><span data-stu-id="7f861-164">The `members@delta` property is included in group objects by default, when the `$select` query parameter has not been specified, or when the `$expand=members` parameter is explicitly specified.</span></span> <span data-ttu-id="7f861-165">Bei Gruppen mit vielen Mitgliedern ist es möglich, dass nicht alle Mitglieder in eine einzelne Antwort passen. In diesem Abschnitt beschreiben wir das Muster, das Sie in solchen Fällen implementieren sollten.</span><span class="sxs-lookup"><span data-stu-id="7f861-165">For groups with many members it is possible that all members cannot fit into a single response; in this section we describe the pattern you should implement to handle such cases.</span></span>

><span data-ttu-id="7f861-166">**Hinweis:** Dieses Muster bezieht sich sowohl auf den anfänglichen Abruf des Gruppenzustands als auch auf nachfolgende Aufrufe zum Abrufen von Delta-Änderungen.</span><span class="sxs-lookup"><span data-stu-id="7f861-166">**Note:** This pattern applies to both the initial retrieval of group state as well as to subsequent calls to get delta changes.</span></span>

<span data-ttu-id="7f861-167">Nehmen wir an, dass Sie die folgende Delta-Abfrage ausführen, um entweder den kompletten Anfangszustand der Gruppe oder zu einem späteren Zeitpunkt die Delta-Änderungen abzufragen:</span><span class="sxs-lookup"><span data-stu-id="7f861-167">Let's assume you are executing the following delta query - either to capture the initial full state of groups, or later on to get delta changes:</span></span>

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description&$expand=members
```

1. <span data-ttu-id="7f861-168">Microsoft Graph gibt möglicherweise eine Antwort zurück, die nur ein Gruppenobjekt mit einer langen Liste von Mitgliedern in der Eigenschaft `members@delta` enthält:</span><span class="sxs-lookup"><span data-stu-id="7f861-168">Microsoft Graph may return a response that contains just one group object, with a large list of members in the `members@delta` property:</span></span>

<span data-ttu-id="7f861-169">**Erste Seite**</span><span class="sxs-lookup"><span data-stu-id="7f861-169">**First Page**</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=<...>",
  "value": [
    {
      "displayName":"LargeGroup",
      "description":"A group containing thousands of users",
      "id":"2e5807ce-58f3-4a94-9b37-ffff2e085957",
      "members@delta": [
          {
              "@odata.type": "#microsoft.graph.user",
              "id": "632f6bb2-3ec8-4c1f-9073-0027a8c6859",
              "@removed": {
                  "reason": "deleted"
              }
          },
          {
              "@odata.type": "#microsoft.graph.user",
              "id": "37de1ae3-408f-4702-8636-20824abda004"
          },
          <...more users here...>
      ]
    }
    <...no more groups included - this group filled out the entire response...>
  ]
}
```

2. <span data-ttu-id="7f861-170">Wenn Sie `nextLink` folgen, erhalten Sie möglicherweise erneut eine Antwort mit demselben Gruppenobjekt.</span><span class="sxs-lookup"><span data-stu-id="7f861-170">When you follow the `nextLink` you may receive a response again containing the same group object.</span></span> <span data-ttu-id="7f861-171">Die gleichen Eigenschaftswerte werden zurückgegeben, aber die erweiterte Eigenschaft `members@delta` enthält jetzt eine andere Benutzerliste.</span><span class="sxs-lookup"><span data-stu-id="7f861-171">The same property values will be returned but the expanded `members@delta` property now contains a different list of users.</span></span>

<span data-ttu-id="7f861-172">**Zweite Seite**</span><span class="sxs-lookup"><span data-stu-id="7f861-172">**Second page**</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=<...>",
  "value": [
    {
      "displayName":"LargeGroup",
      "description":"A group containing thousands of users",
      "id":"2e5807ce-58f3-4a94-9b37-ffff2e085957",
      "members@delta": [
          {
              "@odata.type": "#microsoft.graph.user",
              "id": "c08a463b-7b8a-40a4-aa31-f9bf690b9551",
              "@removed": {
                  "reason": "deleted"
              }
          },
          {
              "@odata.type": "#microsoft.graph.user",
              "id": "23423fa6-821e-44b2-aae4-d039d33884c2"
          },
          <...more users here...>
      ]
    }
    <...no more groups included - this group filled out the entire response...>
  ]
}
```

3. <span data-ttu-id="7f861-173">Schließlich wird auf diese Weise die gesamten Mitgliederliste zurückgegeben, und andere Gruppen werden in der Antwort angezeigt.</span><span class="sxs-lookup"><span data-stu-id="7f861-173">Eventually, the entire member list will be returned in this fashion, and other groups will start showing up in the response.</span></span>

<span data-ttu-id="7f861-174">Es wird empfohlen, die folgenden bewährten Methoden zu verwenden, um dieses Muster zu verarbeiten:</span><span class="sxs-lookup"><span data-stu-id="7f861-174">We recommend the following best practices to correctly handle this pattern:</span></span>
- <span data-ttu-id="7f861-175">Folgen Sie stets `nextLink` und führen Sie den Zustand jeder Gruppe lokal zusammen: Wenn Sie Antworten im Zusammenhang mit der gleichen Gruppe erhalten haben, verwenden Sie diese, um in Ihrer Anwendung die komplette Mitgliederliste zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="7f861-175">Always follow `nextLink` and locally merge each group's state: as you receive responses related to the same group, use them to build the full membership list in your application.</span></span>
- <span data-ttu-id="7f861-176">Es empfiehlt sich, bei den Antworten von keiner bestimmten Sequenz auszugehen.</span><span class="sxs-lookup"><span data-stu-id="7f861-176">It is best not to assume a specific sequence of the responses.</span></span> <span data-ttu-id="7f861-177">Gehen Sie davon aus, dass die gleiche Gruppe an einer beliebigen Stelle in der Sequenz `nextLink` angezeigt werden kann und berücksichtigen Sie dies in Ihrer Zusammenführungslogik.</span><span class="sxs-lookup"><span data-stu-id="7f861-177">Assume that the same group could show up anywhere in the `nextLink` sequence and handle that in your merge logic.</span></span>


## <a name="see-also"></a><span data-ttu-id="7f861-178">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="7f861-178">See also</span></span>
<span data-ttu-id="7f861-179">[Microsoft Graph-Delta-Abfrage](../concepts/delta_query_overview.md) – Übersicht.</span><span class="sxs-lookup"><span data-stu-id="7f861-179">[Microsoft Graph delta query](../concepts/delta_query_overview.md) overview.</span></span>
