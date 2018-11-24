# <a name="user-delta"></a><span data-ttu-id="e1c36-101">user: delta</span><span class="sxs-lookup"><span data-stu-id="e1c36-101">user: delta</span></span>

<span data-ttu-id="e1c36-102">Get neu erstellt, aktualisiert oder Benutzer ohne Durchführung ein alles Lesen der gesamten Benutzer-Auflistung gelöscht.</span><span class="sxs-lookup"><span data-stu-id="e1c36-102">Get newly created, updated, or deleted users without having to perform a full read of the entire user collection.</span></span> <span data-ttu-id="e1c36-103">Einzelheiten finden Sie unter [Nachverfolgen von Änderungen](../../../concepts/delta_query_overview.md) .</span><span class="sxs-lookup"><span data-stu-id="e1c36-103">See [Track changes](../../../concepts/delta_query_overview.md) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="e1c36-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e1c36-104">Permissions</span></span>

<span data-ttu-id="e1c36-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e1c36-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="e1c36-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e1c36-107">Permission type</span></span>      | <span data-ttu-id="e1c36-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e1c36-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1c36-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e1c36-109">Delegated (work or school account)</span></span> | <span data-ttu-id="e1c36-110">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e1c36-110">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e1c36-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e1c36-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1c36-112">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1c36-112">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="e1c36-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e1c36-113">Application</span></span> | <span data-ttu-id="e1c36-114">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1c36-114">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e1c36-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e1c36-115">HTTP request</span></span>

<span data-ttu-id="e1c36-116">Um Änderungen nachzuverfolgen, führen Sie zunächst eine Anforderung einschließlich der delta-Funktion für die Benutzerressource aus.</span><span class="sxs-lookup"><span data-stu-id="e1c36-116">To begin tracking changes, you make a request including the delta function on the users resource.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/delta
```

## <a name="query-parameters"></a><span data-ttu-id="e1c36-117">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e1c36-117">Query parameters</span></span>

<span data-ttu-id="e1c36-118">Nachverfolgen von Änderungen in Benutzer verursacht eine Rundung eine oder mehrere **Delta** Funktionsaufrufe.</span><span class="sxs-lookup"><span data-stu-id="e1c36-118">Tracking changes in users incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="e1c36-119">Wenn Sie eine beliebige Abfragezeichenfolgen-Parameter verwenden (außer `$deltatoken` und `$skiptoken`), müssen Sie es in die erste **Delta** -Anforderung angeben.</span><span class="sxs-lookup"><span data-stu-id="e1c36-119">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="e1c36-120">Microsoft Graph codiert angegebenen Parameter automatisch in den token Teil der `nextLink` oder `deltaLink` URL auf, die in der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e1c36-120">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="e1c36-121">Sie müssen alle gewünschten Abfrageparameter nur einmal im Vorfeld angeben.</span><span class="sxs-lookup"><span data-stu-id="e1c36-121">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="e1c36-122">In nachfolgenden Anforderungen können Sie die  `nextLink`- oder `deltaLink`-URL aus der vorherigen Antwort kopieren und anwenden, da diese URL bereits die codierten gewünschten Parameter enthält.</span><span class="sxs-lookup"><span data-stu-id="e1c36-122">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="e1c36-123">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e1c36-123">Query parameter</span></span>      | <span data-ttu-id="e1c36-124">Typ</span><span class="sxs-lookup"><span data-stu-id="e1c36-124">Type</span></span>   |<span data-ttu-id="e1c36-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e1c36-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e1c36-126">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="e1c36-126">$deltatoken</span></span> | <span data-ttu-id="e1c36-127">string</span><span class="sxs-lookup"><span data-stu-id="e1c36-127">string</span></span> | <span data-ttu-id="e1c36-p104">Ein [Statustoken](../../../concepts/delta_query_overview.md), das in der `deltaLink`-URL des vorhergehenden **delta**-Funktionsaufrufs für dieselbe Benutzersammlung zurückgegeben wird und den Abschluss dieser Runde der Änderungsnachverfolgung anzeigt. Speichern Sie die gesamte `deltaLink`-URL einschließlich dieses Tokens, und wenden Sie sie in der ersten Anforderung der nächsten Änderungsnachverfolgungsrunde für diese Sammlung an.</span><span class="sxs-lookup"><span data-stu-id="e1c36-p104">A [state token](../../../concepts/delta_query_overview.md) returned in the `deltaLink` URL of the previous **delta** function call for the same user collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="e1c36-130">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="e1c36-130">$skiptoken</span></span> | <span data-ttu-id="e1c36-131">string</span><span class="sxs-lookup"><span data-stu-id="e1c36-131">string</span></span> | <span data-ttu-id="e1c36-132">Ein [Statustoken](../../../concepts/delta_query_overview.md), das in der `nextLink`-URL des vorhergehenden **delta**-Funktionsaufrufs zurückgegeben wird und anzeigt, dass in derselben Benutzersammlung weitere Änderungen zum Nachverfolgen vorliegen.</span><span class="sxs-lookup"><span data-stu-id="e1c36-132">A [state token](../../../concepts/delta_query_overview.md) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same user collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="e1c36-133">OData-Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e1c36-133">OData query parameters</span></span>

<span data-ttu-id="e1c36-134">Diese Methode unterstützt optionale Parameter der OData-Abfrage, mit denen die Antwort anpassen.</span><span class="sxs-lookup"><span data-stu-id="e1c36-134">This method supports optional OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="e1c36-p105">Sie können wie bei jeder GET-Anforderung den Abfrageparameter `$select` verwenden, um zwecks Leistungsoptimierung nur die benötigten Eigenschaften anzugeben. Die Eigenschaft *id* wird immer zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e1c36-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The *id* property is always returned.</span></span>
- <span data-ttu-id="e1c36-137">Es ist eingeschränkte Unterstützung für `$filter`:</span><span class="sxs-lookup"><span data-stu-id="e1c36-137">There is limited support for `$filter`:</span></span>
  - <span data-ttu-id="e1c36-138">Der einzige unterstützte `$filter`-Ausdruck dient zum Nachverfolgen von Änderungen an einem bestimmten Objekt: `$filter=id+eq+{value}`.</span><span class="sxs-lookup"><span data-stu-id="e1c36-138">The only supported `$filter` expression is for tracking changes on a specific object: `$filter=id+eq+{value}`.</span></span> <span data-ttu-id="e1c36-139">Sie können mehrere Objekte filtern.</span><span class="sxs-lookup"><span data-stu-id="e1c36-139">You can filter multiple objects.</span></span> <span data-ttu-id="e1c36-140">Beispiel: `https://graph.microsoft.com/v1.0/users/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span><span class="sxs-lookup"><span data-stu-id="e1c36-140">For example, `https://graph.microsoft.com/v1.0/users/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`.</span></span> <span data-ttu-id="e1c36-141">Es gilt ein Grenzwert von 50 gefilterten Objekten.</span><span class="sxs-lookup"><span data-stu-id="e1c36-141">There is a limit of 50 filtered objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e1c36-142">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e1c36-142">Request headers</span></span>
| <span data-ttu-id="e1c36-143">Name</span><span class="sxs-lookup"><span data-stu-id="e1c36-143">Name</span></span>       | <span data-ttu-id="e1c36-144">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e1c36-144">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e1c36-145">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1c36-145">Authorization</span></span>  | <span data-ttu-id="e1c36-146">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="e1c36-146">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="e1c36-147">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e1c36-147">Content-Type</span></span>  | <span data-ttu-id="e1c36-148">application/json</span><span class="sxs-lookup"><span data-stu-id="e1c36-148">application/json</span></span> |
| <span data-ttu-id="e1c36-149">Prefer</span><span class="sxs-lookup"><span data-stu-id="e1c36-149">Prefer</span></span> | <span data-ttu-id="e1c36-150">zurückgeben = minimal</span><span class="sxs-lookup"><span data-stu-id="e1c36-150">return=minimal</span></span> <br><br><span data-ttu-id="e1c36-151">Angabe dieser Header mit einer Anforderung, die verwendet eine `deltaLink` würde zurückgeben nur die Eigenschaften des Objekts, die seit der letzten Round geändert wurden.</span><span class="sxs-lookup"><span data-stu-id="e1c36-151">Specifying this header with a request that uses a `deltaLink` would return only the object properties that have changed since the last round.</span></span> <span data-ttu-id="e1c36-152">Optional.</span><span class="sxs-lookup"><span data-stu-id="e1c36-152">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e1c36-153">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e1c36-153">Request body</span></span>
<span data-ttu-id="e1c36-154">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e1c36-154">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="e1c36-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="e1c36-155">Response</span></span>

<span data-ttu-id="e1c36-156">Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwort Code und [Benutzer](../resources/user.md) -Auflistungsobjekt in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="e1c36-156">If successful, this method returns `200 OK` response code and [user](../resources/user.md) collection object in the response body.</span></span> <span data-ttu-id="e1c36-157">Die Antwort enthält außerdem eine `nextLink` URL oder eine `deltaLink` URL.</span><span class="sxs-lookup"><span data-stu-id="e1c36-157">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="e1c36-158">Wenn ein `nextLink` URL zurückgegeben wird:</span><span class="sxs-lookup"><span data-stu-id="e1c36-158">If a `nextLink` URL is returned:</span></span>
  - <span data-ttu-id="e1c36-159">Dies gibt an, dass es sind zusätzliche Seiten mit Daten aus der Sitzung abgerufen werden sollen.</span><span class="sxs-lookup"><span data-stu-id="e1c36-159">This indicates there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="e1c36-160">Die Anwendung weiterhin tätigen Anforderungen mithilfe der `nextLink` URL bis eine `deltaLink` URL in der Antwort enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="e1c36-160">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
  - <span data-ttu-id="e1c36-161">Die Antwort enthält den gleichen Satz an Eigenschaften wie in der ersten Delta abfrageanforderung.</span><span class="sxs-lookup"><span data-stu-id="e1c36-161">The response includes the same set of properties as in the initial delta query request.</span></span> <span data-ttu-id="e1c36-162">Dadurch können Sie den vollständigen aktuellen Status der Objekte erfasst werden, wenn den Delta-Zyklus zu initiieren.</span><span class="sxs-lookup"><span data-stu-id="e1c36-162">This allows you to capture the full current state of the objects when initiating the delta cycle.</span></span>

- <span data-ttu-id="e1c36-163">Wenn ein `deltaLink` URL zurückgegeben wird:</span><span class="sxs-lookup"><span data-stu-id="e1c36-163">If a `deltaLink` URL is returned:</span></span>
  - <span data-ttu-id="e1c36-164">Dies gibt an, dass es sind keine weiteren Daten zum vorhandenen Status der Ressource zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="e1c36-164">This indicates there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="e1c36-165">Speichern und verwenden Sie die `deltaLink` URL, um zu lernen in die Ressource in der nächsten Runde geändert.</span><span class="sxs-lookup"><span data-stu-id="e1c36-165">Save and use the `deltaLink` URL to learn about changes to the resource in the next round.</span></span>
  - <span data-ttu-id="e1c36-166">Sie haben die Wahl zum Angeben der `Prefer:return=minimal` -Header in der Antwort nur Werte für die Eigenschaften enthalten, die seit der Ausführung geändert wurden die `deltaLink` ausgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="e1c36-166">You have a choice to specify the `Prefer:return=minimal` header, to include in the response values for only the properties that have changed since the time the `deltaLink` was issued.</span></span>

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a><span data-ttu-id="e1c36-167">Standard: zurückzugeben Sie, die gleichen Eigenschaften als erste Delta-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e1c36-167">Default: return the same properties as initial delta request</span></span>

<span data-ttu-id="e1c36-168">Standardmäßig fordert mithilfe einer `deltaLink` oder `nextLink` dieselben Eigenschaften wie in der ersten Delta-Abfrage ausgewählten folgendermaßen zurückgeben:</span><span class="sxs-lookup"><span data-stu-id="e1c36-168">By default, requests using a `deltaLink` or `nextLink` return the same properties as selected in the initial delta query in the following ways:</span></span>

- <span data-ttu-id="e1c36-169">Zurückgeben Sie die Eigenschaft geändert wird, die Eigenschaft in die JSON-Antwort.</span><span class="sxs-lookup"><span data-stu-id="e1c36-169">If the property has changed, return the property in the JSON response.</span></span>
- <span data-ttu-id="e1c36-170">Wenn die Eigenschaft auf einen leeren Wert festgelegt wurde, zurückgeben Sie den Eigenschaftswert als null.</span><span class="sxs-lookup"><span data-stu-id="e1c36-170">If the property has been set to an empty value, return the property value as null.</span></span>
- <span data-ttu-id="e1c36-171">Wenn die Eigenschaft nicht geändert wurde, den Wert NULL zurück.</span><span class="sxs-lookup"><span data-stu-id="e1c36-171">If the property has not changed, return the value as null.</span></span>

> <span data-ttu-id="e1c36-172">**Hinweis:** Mit dem obigen Verhalten, es ist nicht möglich zur Unterscheidung zwischen einer Eigenschaft, die nicht geändert wurde und eine, die geändert hat eine `null` Wert.</span><span class="sxs-lookup"><span data-stu-id="e1c36-172">**Note:** With the above behavior, it is not possible to differentiate between a property that has not changed and one that has changed to a `null` value.</span></span> <span data-ttu-id="e1c36-173">Finden Sie im [zweiten Beispiel](#request-2) unten.</span><span class="sxs-lookup"><span data-stu-id="e1c36-173">See the [second example](#request-2) below.</span></span> <span data-ttu-id="e1c36-174">Wenn dieser Aspekt wichtig ist, sollten das alternative-Verhalten im nächsten Abschnitt beschrieben.</span><span class="sxs-lookup"><span data-stu-id="e1c36-174">If this is important, we recommend using the alternative behavior described in the next section.</span></span>

#### <a name="alternative-return-only-the-changed-properties"></a><span data-ttu-id="e1c36-175">Alternative: nur die geänderten Eigenschaften zurückgeben</span><span class="sxs-lookup"><span data-stu-id="e1c36-175">Alternative: return only the changed properties</span></span>

<span data-ttu-id="e1c36-176">Hinzufügen einer optionalen Anforderungsheader - `prefer:return=minimal` -führt das folgende Verhalten:</span><span class="sxs-lookup"><span data-stu-id="e1c36-176">Adding an optional request header - `prefer:return=minimal` - results in the following behavior:</span></span>

- <span data-ttu-id="e1c36-177">Zurückgeben Sie die Eigenschaft geändert wird, die Eigenschaft in die JSON-Antwort.</span><span class="sxs-lookup"><span data-stu-id="e1c36-177">If the property has changed, return the property in the JSON response.</span></span>
- <span data-ttu-id="e1c36-178">Wenn die Eigenschaft auf einen leeren Wert festgelegt wurde, zurückgeben Sie den Eigenschaftswert als null.</span><span class="sxs-lookup"><span data-stu-id="e1c36-178">If the property has been set to an empty value, return the property value as null.</span></span>
- <span data-ttu-id="e1c36-179">Wenn die Eigenschaft nicht geändert hat, nehmen Sie die Eigenschaft nicht in die JSON-Antwort.</span><span class="sxs-lookup"><span data-stu-id="e1c36-179">If the property has not changed, do not include the property in the JSON response.</span></span> <span data-ttu-id="e1c36-180">(Andere als das Standardverhalten).</span><span class="sxs-lookup"><span data-stu-id="e1c36-180">(Different from the default behavior.)</span></span>

> <span data-ttu-id="e1c36-181">**Hinweis:** Die Kopfzeile hinzugefügt werden kann einen `deltaLink` Anforderung an einer beliebigen Stelle in Zeit im Zyklus Delta.</span><span class="sxs-lookup"><span data-stu-id="e1c36-181">**Note:** The header can be added to a `deltaLink` request at any point in time in the delta cycle.</span></span> <span data-ttu-id="e1c36-182">Die Kopfzeile wirkt sich nur auf die Gruppe von Eigenschaften, die in der Antwort enthalten, und er hat keinen Einfluss auf wie die Delta-Abfrage ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="e1c36-182">The header only affects the set of properties included in the response and it does not affect how the delta query is executed.</span></span> <span data-ttu-id="e1c36-183">Finden Sie im [dritten Beispiel](#request-3) unten.</span><span class="sxs-lookup"><span data-stu-id="e1c36-183">See the [third example](#request-3) below.</span></span>

### <a name="example"></a><span data-ttu-id="e1c36-184">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e1c36-184">Example</span></span>

#### <a name="request-1"></a><span data-ttu-id="e1c36-185">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="e1c36-185">Request 1</span></span>

<span data-ttu-id="e1c36-186">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e1c36-186">The following is an example of the request.</span></span> <span data-ttu-id="e1c36-187">Es ist keine `$select` Parameter, damit ein Standardsatz Eigenschaften nachverfolgt und zurückgegeben wird.</span><span class="sxs-lookup"><span data-stu-id="e1c36-187">There is no `$select` parameter, so a default set of properties is tracked and returned.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/users/delta
```

#### <a name="response-1"></a><span data-ttu-id="e1c36-188">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="e1c36-188">Response 1</span></span>

<span data-ttu-id="e1c36-189">Im folgenden ist ein Beispiel für die Antwort aus, wenn mit `deltaLink` von der Initialisierung Abfrage abgerufen.</span><span class="sxs-lookup"><span data-stu-id="e1c36-189">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span>

><span data-ttu-id="e1c36-p116">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="e1c36-p116">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "businessPhones": [
          "businessPhones-value"
      ],
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "jobTitle": "jobTitle-value",
      "mail": "mail-value",
      "mobilePhone": "mobilePhone-value",
      "officeLocation": "officeLocation-value",
      "preferredLanguage": "preferredLanguage-value",
      "surname": "surname-value",
      "userPrincipalName": "userPrincipalName-value",
      "id": "id-value"
    }
  ]
}
```

#### <a name="request-2"></a><span data-ttu-id="e1c36-192">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="e1c36-192">Request 2</span></span>

<span data-ttu-id="e1c36-193">Das nächste Beispiel veranschaulicht die erste Anforderung 3 Eigenschaften für nachverfolgen Antwort Standardverhalten auswählen:</span><span class="sxs-lookup"><span data-stu-id="e1c36-193">The next example shows the initial request selecting 3 properties for change tracking, with default response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/users/delta?$select=displayName,jobTitle,mobilePhone
```

#### <a name="response-2"></a><span data-ttu-id="e1c36-194">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="e1c36-194">Response 2</span></span>

<span data-ttu-id="e1c36-195">Im folgenden ist ein Beispiel für die Antwort aus, wenn mit `deltaLink` von der Initialisierung Abfrage abgerufen.</span><span class="sxs-lookup"><span data-stu-id="e1c36-195">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="e1c36-196">Beachten Sie, dass `jobTitle` und `mobilePhone` den Wert der `null` , d. h., die sie möglicherweise nicht geändert oder auf einen leeren Wert festgelegt wurden.</span><span class="sxs-lookup"><span data-stu-id="e1c36-196">Note that `jobTitle` and `mobilePhone` have the value of `null` which means that they may have not changed or have been set to an empty value.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "jobTitle": null,
      "mobilePhone": null
    }
  ]
}
```

#### <a name="request-3"></a><span data-ttu-id="e1c36-197">Anforderung 3</span><span class="sxs-lookup"><span data-stu-id="e1c36-197">Request 3</span></span>

<span data-ttu-id="e1c36-198">Das nächste Beispiel veranschaulicht die erste Anforderung 3 Eigenschaften für nachverfolgen mit alternativen minimale Antwort Verhalten auswählen:</span><span class="sxs-lookup"><span data-stu-id="e1c36-198">The next example shows the initial request selecting 3 properties for change tracking, with alternative minimal response behavior:</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/users/delta?$select=displayName,jobTitle,mobilePhone
Prefer: return=minimal
```

#### <a name="response-3"></a><span data-ttu-id="e1c36-199">Antwort 3</span><span class="sxs-lookup"><span data-stu-id="e1c36-199">Response 3</span></span>

<span data-ttu-id="e1c36-200">Im folgenden ist ein Beispiel für die Antwort aus, wenn mit `deltaLink` von der Initialisierung Abfrage abgerufen.</span><span class="sxs-lookup"><span data-stu-id="e1c36-200">The following is an example of the response when using `deltaLink` obtained from the query initialization.</span></span> <span data-ttu-id="e1c36-201">Beachten Sie, dass die `mobilePhone` -Eigenschaft ist nicht enthalten, was bedeutet, dass wurde nicht geändert seit der letzten Delta-Abfrage; `displayName` und `jobTitle` sind enthalten, d. h., deren Werte geändert haben.</span><span class="sxs-lookup"><span data-stu-id="e1c36-201">Note that the `mobilePhone` property is not included, which means it has not changed since the last delta query; `displayName` and `jobTitle` are included which means their values have changed.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "jobTitle": null
    }
  ]
}
```

- <span data-ttu-id="e1c36-202">[Delta-Abfrage zum Nachverfolgen von Änderungen in Microsoft Graph-Daten verwenden](../../../concepts/delta_query_overview.md).</span><span class="sxs-lookup"><span data-stu-id="e1c36-202">[Use delta query to track changes in Microsoft Graph data](../../../concepts/delta_query_overview.md).</span></span>
- <span data-ttu-id="e1c36-203">[Inkrementelle Änderungen für Benutzer erhalten möchten](../../../concepts/delta_query_users.md).</span><span class="sxs-lookup"><span data-stu-id="e1c36-203">[Get incremental changes for users](../../../concepts/delta_query_users.md).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->