# <a name="group-delta"></a><span data-ttu-id="5d32f-101">group: delta</span><span class="sxs-lookup"><span data-stu-id="5d32f-101">group: delta</span></span>
<span data-ttu-id="5d32f-102">Get neu erstellt, aktualisiert oder Gruppen, einschließlich der Gruppenmitgliedschaft ändert, ohne zum Ausführen eines alles Lesen der ganzen Gruppe-Auflistung gelöscht.</span><span class="sxs-lookup"><span data-stu-id="5d32f-102">Get newly created, updated, or deleted groups, including group membership changes, without having to perform a full read of the entire group collection.</span></span> <span data-ttu-id="5d32f-103">Einzelheiten finden Sie unter [Delta-Abfrage verwenden](../../../concepts/delta_query_overview.md) .</span><span class="sxs-lookup"><span data-stu-id="5d32f-103">See [Using Delta Query](../../../concepts/delta_query_overview.md) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="5d32f-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5d32f-104">Permissions</span></span>

<span data-ttu-id="5d32f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5d32f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5d32f-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5d32f-107">Permission type</span></span>      | <span data-ttu-id="5d32f-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5d32f-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d32f-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5d32f-109">Delegated (work or school account)</span></span> | <span data-ttu-id="5d32f-110">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d32f-110">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5d32f-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5d32f-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d32f-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5d32f-112">Not supported.</span></span>    |
|<span data-ttu-id="5d32f-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5d32f-113">Application</span></span> | <span data-ttu-id="5d32f-114">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d32f-114">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5d32f-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5d32f-115">HTTP request</span></span>

<span data-ttu-id="5d32f-116">Um Änderungen nachzuverfolgen, führe Sie zunächst eine Anforderung einschließlich der delta-Funktion für die Gruppenressource aus.</span><span class="sxs-lookup"><span data-stu-id="5d32f-116">To begin tracking changes, you make a request including the delta function on the groups resource.</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/delta
```

## <a name="query-parameters"></a><span data-ttu-id="5d32f-117">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="5d32f-117">Query parameters</span></span>

<span data-ttu-id="5d32f-p103">Beim Nachverfolgen von Änderungen in Gruppen wird eine Runde von einem oder mehreren **delta**-Funktionsaufrufen ausgeführt. Wenn Sie Abfrageparameter (außer `$deltatoken` und `$skiptoken`) verwenden, müssen Sie sie in der ursprünglichen **delta**-Anforderung angeben. Microsoft Graph codiert automatisch alle angegebenen Parameter in den Tokenteil der in der Antwort enthaltenen `nextLink`- oder `deltaLink`-URL.</span><span class="sxs-lookup"><span data-stu-id="5d32f-p103">Tracking changes in groups incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="5d32f-121">Sie müssen alle gewünschten Abfrageparameter nur einmal im Vorfeld angeben.</span><span class="sxs-lookup"><span data-stu-id="5d32f-121">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="5d32f-122">In nachfolgenden Anforderungen können Sie die  `nextLink`- oder `deltaLink`-URL aus der vorherigen Antwort kopieren und anwenden, da diese URL bereits die codierten gewünschten Parameter enthält.</span><span class="sxs-lookup"><span data-stu-id="5d32f-122">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="5d32f-123">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="5d32f-123">Query parameter</span></span> | <span data-ttu-id="5d32f-124">Typ</span><span class="sxs-lookup"><span data-stu-id="5d32f-124">Type</span></span>  |<span data-ttu-id="5d32f-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5d32f-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5d32f-126">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="5d32f-126">$deltatoken</span></span> | <span data-ttu-id="5d32f-127">string</span><span class="sxs-lookup"><span data-stu-id="5d32f-127">string</span></span> | <span data-ttu-id="5d32f-p104">Ein [Statustoken](../../../concepts/delta_query_overview.md), das in der `deltaLink`-URL des vorhergehenden **delta**-Funktionsaufrufs für dieselbe Gruppensammlung zurückgegeben wird und den Abschluss dieser Runde der Änderungsnachverfolgung anzeigt. Speichern Sie die gesamte `deltaLink`-URL einschließlich dieses Tokens, und wenden Sie sie in der ersten Anforderung der nächsten Änderungsnachverfolgungsrunde für diese Sammlung an.</span><span class="sxs-lookup"><span data-stu-id="5d32f-p104">A [state token](../../../concepts/delta_query_overview.md) returned in the `deltaLink` URL of the previous **delta** function call for the same group collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="5d32f-130">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="5d32f-130">$skiptoken</span></span> | <span data-ttu-id="5d32f-131">string</span><span class="sxs-lookup"><span data-stu-id="5d32f-131">string</span></span> | <span data-ttu-id="5d32f-132">Ein [Statustoken](../../../concepts/delta_query_overview.md), das in der `nextLink`-URL des vorhergehenden **delta**-Funktionsaufrufs zurückgegeben wird und anzeigt, dass in derselben Gruppensammlung weitere Änderungen zum Nachverfolgen vorliegen.</span><span class="sxs-lookup"><span data-stu-id="5d32f-132">A [state token](../../../concepts/delta_query_overview.md) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same group collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="5d32f-133">OData-Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="5d32f-133">OData query parameters</span></span>

<span data-ttu-id="5d32f-134">Diese Methode unterstützt optionale Parameter der OData-Abfrage, mit denen die Antwort anpassen.</span><span class="sxs-lookup"><span data-stu-id="5d32f-134">This method supports optional OData query parameters to help customize the response.</span></span>

- <span data-ttu-id="5d32f-p105">Sie können wie bei jeder GET-Anforderung den Abfrageparameter `$select` verwenden, um zwecks Leistungsoptimierung nur die benötigten Eigenschaften anzugeben. Die Eigenschaft *id* wird immer zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5d32f-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The *id* property is always returned.</span></span>
- <span data-ttu-id="5d32f-137">Sie können `$expand=members` mitgliedschaftsänderungen abgerufen.</span><span class="sxs-lookup"><span data-stu-id="5d32f-137">You can use `$expand=members` to get membership changes.</span></span>
- <span data-ttu-id="5d32f-138">Es ist eingeschränkte Unterstützung für `$filter`:</span><span class="sxs-lookup"><span data-stu-id="5d32f-138">There is limited support for `$filter`:</span></span>
  - <span data-ttu-id="5d32f-139">Der einzige unterstützte `$filter`-Ausdruck dient zum Nachverfolgen von Änderungen an einem bestimmten Objekt: `$filter=id+eq+{value}`.</span><span class="sxs-lookup"><span data-stu-id="5d32f-139">The only supported `$filter` expression is for tracking changes on a specific object: `$filter=id+eq+{value}`.</span></span> <span data-ttu-id="5d32f-140">Sie können mehrere Objekte filtern.</span><span class="sxs-lookup"><span data-stu-id="5d32f-140">You can filter multiple objects.</span></span> <span data-ttu-id="5d32f-141">Beispiel: `https://graph.microsoft.com/v1.0/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span><span class="sxs-lookup"><span data-stu-id="5d32f-141">For example, `https://graph.microsoft.com/v1.0/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span></span> <span data-ttu-id="5d32f-142">Es gilt ein Grenzwert von 50 gefilterten Objekten.</span><span class="sxs-lookup"><span data-stu-id="5d32f-142">There is a limit of 50 filtered objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5d32f-143">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5d32f-143">Request headers</span></span>

| <span data-ttu-id="5d32f-144">Name</span><span class="sxs-lookup"><span data-stu-id="5d32f-144">Name</span></span>       | <span data-ttu-id="5d32f-145">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5d32f-145">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5d32f-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d32f-146">Authorization</span></span>  | <span data-ttu-id="5d32f-147">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="5d32f-147">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="5d32f-148">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5d32f-148">Content-Type</span></span>  | <span data-ttu-id="5d32f-149">application/json</span><span class="sxs-lookup"><span data-stu-id="5d32f-149">application/json</span></span> |
| <span data-ttu-id="5d32f-150">Prefer</span><span class="sxs-lookup"><span data-stu-id="5d32f-150">Prefer</span></span> | <span data-ttu-id="5d32f-151">zurückgeben = minimal</span><span class="sxs-lookup"><span data-stu-id="5d32f-151">return=minimal</span></span> <br><br><span data-ttu-id="5d32f-152">Angabe dieser Header mit einer Anforderung, die verwendet eine `deltaLink` würde zurückgeben nur die Eigenschaften des Objekts, die seit der letzten Round geändert wurden.</span><span class="sxs-lookup"><span data-stu-id="5d32f-152">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="5d32f-153">Optional.</span><span class="sxs-lookup"><span data-stu-id="5d32f-153">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5d32f-154">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5d32f-154">Request body</span></span>

<span data-ttu-id="5d32f-155">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5d32f-155">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="5d32f-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="5d32f-156">Response</span></span>

<span data-ttu-id="5d32f-157">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [group](../resources/group.md)-Sammlungsobjekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5d32f-157">If successful, this method returns `200 OK` response code and [group](../resources/group.md) collection object in the response body.</span></span> <span data-ttu-id="5d32f-158">Die Antwort enthält auch ein Status-Token der entweder ein `nextLink` URL oder eine `deltaLink` URL.</span><span class="sxs-lookup"><span data-stu-id="5d32f-158">The response also includes a state token which is either a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="5d32f-159">Wenn ein `nextLink` URL zurückgegeben wird:</span><span class="sxs-lookup"><span data-stu-id="5d32f-159">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="5d32f-160">Dies gibt an, dass es sind zusätzliche Seiten mit Daten aus der Sitzung abgerufen werden sollen.</span><span class="sxs-lookup"><span data-stu-id="5d32f-160">This indicates there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="5d32f-161">Die Anwendung weiterhin tätigen Anforderungen mithilfe der `nextLink` URL bis eine `deltaLink` URL in der Antwort enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="5d32f-161">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="5d32f-162">Die Antwort enthält den gleichen Satz an Eigenschaften wie in der ersten Delta abfrageanforderung.</span><span class="sxs-lookup"><span data-stu-id="5d32f-162">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="5d32f-163">Dadurch können Sie den vollständigen aktuellen Status der Objekte erfasst werden, wenn den Delta-Zyklus zu initiieren.</span><span class="sxs-lookup"><span data-stu-id="5d32f-163">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="5d32f-164">Wenn ein `deltaLink` URL zurückgegeben wird:</span><span class="sxs-lookup"><span data-stu-id="5d32f-164">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="5d32f-165">Dies gibt an, dass es sind keine weiteren Daten zum vorhandenen Status der Ressource zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="5d32f-165">This indicates there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="5d32f-166">Speichern und verwenden Sie die `deltaLink` URL, um zu lernen in die Ressource in der nächsten Runde geändert.</span><span class="sxs-lookup"><span data-stu-id="5d32f-166">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="5d32f-167">Sie haben die Wahl zum Angeben der `Prefer:return=minimal` -Header in der Antwort nur Werte für die Eigenschaften enthalten, die seit der Ausführung geändert wurden die `deltaLink` ausgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="5d32f-167">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="5d32f-168">Standard: zurückzugeben Sie, die gleichen Eigenschaften als erste Delta-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5d32f-168">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="5d32f-169">Standardmäßig fordert mithilfe einer `deltaLink` oder `nextLink` dieselben Eigenschaften wie in der ersten Delta-Abfrage ausgewählten folgendermaßen zurückgeben:</span><span class="sxs-lookup"><span data-stu-id="5d32f-169">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="5d32f-170">Zurückgeben Sie die Eigenschaft geändert wird, die Eigenschaft in die JSON-Antwort.</span><span class="sxs-lookup"><span data-stu-id="5d32f-170">If the property has changed, return the property in the JSON response.</span></span>
- <span data-ttu-id="5d32f-171">Wenn die Eigenschaft auf einen leeren Wert festgelegt wurde, zurückgeben Sie den Eigenschaftswert als null.</span><span class="sxs-lookup"><span data-stu-id="5d32f-171">If the property has been set to an empty value, return the property value as null.</span></span>
- <span data-ttu-id="5d32f-172">Wenn die Eigenschaft nicht geändert wurde, den Wert NULL zurück.</span><span class="sxs-lookup"><span data-stu-id="5d32f-172">If the property has not changed, return the value as null.</span></span>

> <span data-ttu-id="5d32f-173">**Hinweis:** Mit dem obigen Verhalten, es ist nicht möglich zur Unterscheidung zwischen einer Eigenschaft, die nicht geändert wurde und eine, die geändert hat eine `null` Wert.</span><span class="sxs-lookup"><span data-stu-id="5d32f-173">**Note:** With the above behavior, it is not possible to differentiate between a property that has not changed and one that has changed to a `null` value.</span></span> <span data-ttu-id="5d32f-174">Finden Sie im [zweiten Beispiel](#request-2) unten.</span><span class="sxs-lookup"><span data-stu-id="5d32f-174">See the [second example](#request-2) below.</span></span> <span data-ttu-id="5d32f-175">Wenn dieser Aspekt wichtig ist, sollten das alternative-Verhalten im nächsten Abschnitt beschrieben.</span><span class="sxs-lookup"><span data-stu-id="5d32f-175">If this is important, we recommend using the alternative behavior described in the next section.</span></span>

#### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="5d32f-176">Alternative: nur die geänderten Eigenschaften zurückgeben</span><span class="sxs-lookup"><span data-stu-id="5d32f-176">Alternative: return only the changed properties</span></span>

<span data-ttu-id="5d32f-177">Hinzufügen einer optionalen Anforderungsheader - `prefer:return=minimal` -führt das folgende Verhalten:</span><span class="sxs-lookup"><span data-stu-id="5d32f-177">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="5d32f-178">Zurückgeben Sie die Eigenschaft geändert wird, die Eigenschaft in die JSON-Antwort.</span><span class="sxs-lookup"><span data-stu-id="5d32f-178">If the property has changed, return the property in the JSON response.</span></span>
- <span data-ttu-id="5d32f-179">Wenn die Eigenschaft auf einen leeren Wert festgelegt wurde, zurückgeben Sie den Eigenschaftswert als null.</span><span class="sxs-lookup"><span data-stu-id="5d32f-179">If the property has been set to an empty value, return the property value as null.</span></span>
- <span data-ttu-id="5d32f-180">Wenn die Eigenschaft nicht geändert hat, nehmen Sie die Eigenschaft nicht in die JSON-Antwort.</span><span class="sxs-lookup"><span data-stu-id="5d32f-180">If the property has not changed, do not include the property in the JSON response.</span></span> <span data-ttu-id="5d32f-181">(Andere als das Standardverhalten).</span><span class="sxs-lookup"><span data-stu-id="5d32f-181">(Different from the default behavior.)</span></span>

> <span data-ttu-id="5d32f-182">**Hinweis:** Die Kopfzeile hinzugefügt werden kann einen `deltaLink` Anforderung an einer beliebigen Stelle in Zeit im Zyklus Delta.</span><span class="sxs-lookup"><span data-stu-id="5d32f-182">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="5d32f-183">Die Kopfzeile wirkt sich nur auf die Gruppe von Eigenschaften, die in der Antwort enthalten, und er hat keinen Einfluss auf wie die Delta-Abfrage ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="5d32f-183">The header only affects the set of properties included in the response and it does not affect how the delta query is executed.</span></span> <span data-ttu-id="5d32f-184">Finden Sie im [dritten Beispiel](#request-3) unten.</span><span class="sxs-lookup"><span data-stu-id="5d32f-184">See the [third example](#request-3) below.</span></span>

### <a name="example"></a><span data-ttu-id="5d32f-185">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5d32f-185">Example</span></span>

#### <a name="request-1"></a><span data-ttu-id="5d32f-186">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="5d32f-186">Request 1</span></span>

<span data-ttu-id="5d32f-187">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5d32f-187">The following is an example of the request.</span></span> <span data-ttu-id="5d32f-188">Es ist keine `$select` Parameter, damit ein Standardsatz Eigenschaften nachverfolgt und zurückgegeben wird.</span><span class="sxs-lookup"><span data-stu-id="5d32f-188">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/groups/delta
```

#### <a name="response-1"></a><span data-ttu-id="5d32f-189">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="5d32f-189">Response 1</span></span>

<span data-ttu-id="5d32f-190">Im folgenden ist ein Beispiel für die Antwort aus, wenn mit `deltaLink` von der Initialisierung Abfrage abgerufen.</span><span class="sxs-lookup"><span data-stu-id="5d32f-190">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span>

><span data-ttu-id="5d32f-191">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="5d32f-191">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5d32f-192">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="5d32f-192">All the properties will be returned from an actual call.</span></span>
>
> <span data-ttu-id="5d32f-193">Das Anwesenheitssymbol der *members@delta* -Eigenschaft umfasst die Ids der Member-Objekte in der Gruppe.</span><span class="sxs-lookup"><span data-stu-id="5d32f-193">Note the presence of the *members@delta* property which includes the ids of member objects in the group.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups","@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjvY1FSSc_",
  "value":[
    {
      "classification": "classification-value",
      "createdDateTime":"datetime-value",
      "description":"Test group 1",
      "displayName":"TestGroup1",
      "groupTypes": [
        "groupTypes-value"
      ],
      "mail": "mail-value",
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
    }
  ]
}
```

#### <a name="request-2"></a><span data-ttu-id="5d32f-194">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="5d32f-194">Request 2</span></span>

<span data-ttu-id="5d32f-195">Das nächste Beispiel veranschaulicht die erste Anforderung 3 Eigenschaften für nachverfolgen Antwort Standardverhalten auswählen:</span><span class="sxs-lookup"><span data-stu-id="5d32f-195">The next example shows the initial request selecting 3 properties for change tracking, with default response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description,mailNickname
```

#### <a name="response-2"></a><span data-ttu-id="5d32f-196">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="5d32f-196">Response 2</span></span>

<span data-ttu-id="5d32f-197">Im folgenden ist ein Beispiel für die Antwort aus, wenn mit `deltaLink` von der Initialisierung Abfrage abgerufen.</span><span class="sxs-lookup"><span data-stu-id="5d32f-197">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="5d32f-198">Beachten Sie, dass `description` und `mailNickname` den Wert der `null` , d. h., die sie möglicherweise nicht geändert oder auf einen leeren Wert festgelegt wurden.</span><span class="sxs-lookup"><span data-stu-id="5d32f-198">Note that `description` and `mailNickname` have the value of `null` which means that they may have not changed or have been set to an empty value.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "description": null,
      "mailNickname": null
    }
  ]
}
```

#### <a name="request-3"></a><span data-ttu-id="5d32f-199">Anforderung 3</span><span class="sxs-lookup"><span data-stu-id="5d32f-199">Request 3</span></span>

<span data-ttu-id="5d32f-200">Das nächste Beispiel veranschaulicht die erste Anforderung 3 Eigenschaften für nachverfolgen mit alternativen minimale Antwort Verhalten auswählen:</span><span class="sxs-lookup"><span data-stu-id="5d32f-200">The next example shows the initial request selecting 3 properties for change tracking, with alternative minimal response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description,mailNickname
Prefer: return=minimal
```

#### <a name="response-3"></a><span data-ttu-id="5d32f-201">Antwort 3</span><span class="sxs-lookup"><span data-stu-id="5d32f-201">Response 3</span></span>

<span data-ttu-id="5d32f-202">Im folgenden ist ein Beispiel für die Antwort aus, wenn mit `deltaLink` von der Initialisierung Abfrage abgerufen.</span><span class="sxs-lookup"><span data-stu-id="5d32f-202">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="5d32f-203">Beachten Sie, dass die `mailNickname` -Eigenschaft ist nicht enthalten, was bedeutet, dass wurde nicht geändert seit der letzten Delta-Abfrage; `displayName` und `description` sind enthalten, d. h., deren Werte geändert haben.</span><span class="sxs-lookup"><span data-stu-id="5d32f-203">Note that the `mailNickname` property is not included, which means it has not changed since the last delta query; `displayName` and `description` are included which means their values have changed.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "description": null
    }
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="5d32f-204">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="5d32f-204">See also</span></span>

- <span data-ttu-id="5d32f-205">[Delta-Abfrage zum Nachverfolgen von Änderungen in Microsoft Graph-Daten verwenden](../../../concepts/delta_query_overview.md).</span><span class="sxs-lookup"><span data-stu-id="5d32f-205">[Use delta query to track changes in Microsoft Graph data](../../../concepts/delta_query_overview.md).</span></span>
- <span data-ttu-id="5d32f-206">[Inkrementelle Änderungen für Gruppen erhalten möchten](../../../concepts/delta_query_groups.md).</span><span class="sxs-lookup"><span data-stu-id="5d32f-206">[Get incremental changes for groups](../../../concepts/delta_query_groups.md).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
