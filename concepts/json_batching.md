# <a name="combine-multiple-requests-in-one-http-call-using-json-batching-preview"></a><span data-ttu-id="4358f-101">Kombinieren von mehreren Anforderungen in einem HTTP-Aufruf unter Verwendung der JSON-Batchverarbeitung (Vorschau)</span><span class="sxs-lookup"><span data-stu-id="4358f-101">Combine multiple requests in one HTTP call using JSON batching (preview)</span></span>

<span data-ttu-id="4358f-p101">Die JSON-Batchverarbeitung ermöglicht es Ihnen, Ihre Anwendung durch Kombinieren von mehreren Anforderungen in einem einzigen JSON-Objekt zu optimieren. Ein Client möchte z. B. eine Ansicht aus nicht verbundenen Daten wie den folgenden zusammenstellen:</span><span class="sxs-lookup"><span data-stu-id="4358f-p101">JSON batching allows you to optimize your application by combining multiple requests into a single JSON object. For example, a client might want to compose a view of unrelated data such as:</span></span>

1. <span data-ttu-id="4358f-104">Ein in OneDrive gespeichertes Bild</span><span class="sxs-lookup"><span data-stu-id="4358f-104">An image stored in OneDrive</span></span>
2. <span data-ttu-id="4358f-105">Eine Liste von Planner-Aufgaben</span><span class="sxs-lookup"><span data-stu-id="4358f-105">A list of Planner tasks</span></span>
3. <span data-ttu-id="4358f-106">Der Kalender für eine Gruppe</span><span class="sxs-lookup"><span data-stu-id="4358f-106">The calendar for a group</span></span>

<span data-ttu-id="4358f-107">Indem Sie diese drei einzelnen Anforderungen in einer einzigen Batchanforderung kombinieren, können Sie die Netzwerklatenz der Anwendung erheblich reduzieren.</span><span class="sxs-lookup"><span data-stu-id="4358f-107">Combining these three individual requests into a single batch request can save the application significant network latency.</span></span>

## <a name="first-json-batch-request"></a><span data-ttu-id="4358f-108">Erste JSON-Batchanforderung</span><span class="sxs-lookup"><span data-stu-id="4358f-108">First JSON batch request</span></span>

<span data-ttu-id="4358f-p102">Zunächst erstellen Sie die JSON-Batchanforderung für das vorherige Beispiel. In diesem Szenario sind die einzelnen Anforderungen in keiner Weise voneinander abhängig und können daher in beliebiger Reihenfolge in der Batchanforderung platziert werden.</span><span class="sxs-lookup"><span data-stu-id="4358f-p102">First you construct the JSON batch request for the previous example. In this scenario, the individual requests are not interdependent in any way and therefore can be placed into the batch request in any order.</span></span>

```http
POST https://graph.microsoft.com/beta/$batch
Accept: application/json
Content-Type: application/json
```

```json
{
  "requests": [
    {
      "id": "1",
      "method": "GET",
      "url": "/me/drive/root:/{file}:/content"
    },
    {
      "id": "2",
      "method": "GET",
      "url": "/me/planner/tasks"
    },
    {
      "id": "3",
      "method": "GET",
      "url": "/groups/{id}/events"
    }
  ]
}
```

<span data-ttu-id="4358f-111">Antworten auf die zum Batch zusammengefassten Anforderungen werden möglicherweise in einer anderen Reihenfolge angezeigt.</span><span class="sxs-lookup"><span data-stu-id="4358f-111">Responses to the batched requests might appear in a different order. The  property can be used to correlate individual requests and responses.</span></span> <span data-ttu-id="4358f-112">Die `id`-Eigenschaft kann verwendet werden, um einzelne Anforderungen und Antworten zu korrelieren.</span><span class="sxs-lookup"><span data-stu-id="4358f-112">Responses to the batched requests might appear in a different order. The `id` property can be used to correlate individual requests and responses.</span></span>

```http
200 OK
Content-Type: application/json
```

```json
{
  "responses": [
    {
      "id": "1",
      "status": 302,
      "headers": {
        "location": "https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi"
      }
    },
    {
      "id": "3",
      "status": 401,
      "body": {
        "error": {
          "code": "Forbidden",
          "message": "..."
        }
      }
    },
    {
      "id": "2",
      "status": 200,
      "body": {
        "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.plannerTask)",
        "value": []
      }
    }
  ]
}
```

## <a name="request-format"></a><span data-ttu-id="4358f-113">Anforderungsformat</span><span class="sxs-lookup"><span data-stu-id="4358f-113">Request format</span></span>

<span data-ttu-id="4358f-114">Batchanforderungen werden immer mithilfe von `POST` an den Endpunkt `/$batch` gesendet.</span><span class="sxs-lookup"><span data-stu-id="4358f-114">Batch requests are always sent using `POST` to the `/$batch` endpoint.</span></span>

<span data-ttu-id="4358f-115">Der Textkörper einer JSON-Batchanforderung besteht aus einem einzelnen JSON-Objekt mit einer erforderlichen Eigenschaft: `requests`.</span><span class="sxs-lookup"><span data-stu-id="4358f-115">A JSON batch request body consists of a single JSON object with one required property: . The  property is an array of individual requests. For each individual request, the , , and  properties are required.</span></span> <span data-ttu-id="4358f-116">Die `requests`-Eigenschaft ist ein Array von einzelnen Anforderungen.</span><span class="sxs-lookup"><span data-stu-id="4358f-116">The `requests` property is an array of individual requests.</span></span> <span data-ttu-id="4358f-117">Für jede einzelne Anforderung sind die Eigenschaften `id`, `method` und `url` erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4358f-117">For each individual request, the `id`, `method`, and `url` properties are required.</span></span>

<span data-ttu-id="4358f-118">Die `id`-Eigenschaft dient in erster Linie als Korrelationswert zum Zuordnen einzelner Antworten zu Anforderungen.</span><span class="sxs-lookup"><span data-stu-id="4358f-118">The `id` property functions primarily as a correlation value to associate individual responses with requests. This allows the server to process requests in the batch in the most efficient order.</span></span> <span data-ttu-id="4358f-119">Dadurch kann der Server Anforderungen im Batch in der effizientesten Reihenfolge verarbeiten.</span><span class="sxs-lookup"><span data-stu-id="4358f-119">The  property functions primarily as a correlation value to associate individual responses with requests. This allows the server to process requests in the batch in the most efficient order.</span></span>

<span data-ttu-id="4358f-120">Die Eigenschaften `method` und `url` sind genau das, was Sie am Anfang jeder HTTP-Anforderung sehen.</span><span class="sxs-lookup"><span data-stu-id="4358f-120">The `method` and `url` properties are exactly what you would see at the start of any given HTTP request. The method is the HTTP method, and the URL is the resource URL the individual request would typically be sent to.</span></span> <span data-ttu-id="4358f-121">Die Methode ist die HTTP-Methode, und die URL ist die Ressourcen-URL, an die die einzelne Anforderung normalerweise gesendet wird.</span><span class="sxs-lookup"><span data-stu-id="4358f-121">The  and  properties are exactly what you would see at the start of any given HTTP request. The method is the HTTP method, and the URL is the resource URL the individual request would typically be sent to.</span></span>

<span data-ttu-id="4358f-122">Einzelne Anforderungen können optional auch eine `headers`- und eine `body`-Eigenschaft enthalten.</span><span class="sxs-lookup"><span data-stu-id="4358f-122">Individual requests can optionally also contain a `headers` property and a `body` property.</span></span> <span data-ttu-id="4358f-123">Beide Eigenschaften sind in der Regel JSON-Objekte.</span><span class="sxs-lookup"><span data-stu-id="4358f-123">Both of these properties are typically JSON objects.</span></span> <span data-ttu-id="4358f-124">In einigen Fällen ist die `body`-Eigenschaft möglicherweise ein base64-codierter URL-Wert anstelle eines JSON Objekts, beispielsweise wenn der Textkörper ein Bild ist.</span><span class="sxs-lookup"><span data-stu-id="4358f-124">In some cases, the `body` might be a base64 URL-encoded value rather than a JSON object - for example, when the body is an image.</span></span> <span data-ttu-id="4358f-125">Wenn ein `body` in der Anforderung enthalten ist, muss das `headers`-Objekt einen Wert für `content-type` enthalten.</span><span class="sxs-lookup"><span data-stu-id="4358f-125">When a `body` is included with the request, the `headers` object must contain a value for `content-type`.</span></span>

## <a name="response-format"></a><span data-ttu-id="4358f-126">Antwortformat</span><span class="sxs-lookup"><span data-stu-id="4358f-126">Response format</span></span>

<span data-ttu-id="4358f-p108">Das Antwortformat für JSON-Batchanforderungen ähnelt dem Anforderungsformat. Die wichtigsten Unterschiede sind folgende:</span><span class="sxs-lookup"><span data-stu-id="4358f-p108">The response format for JSON batch requests is similar to the request format. The following are the key differences:</span></span>

* <span data-ttu-id="4358f-129">Die Eigenschaft im JSON-Hauptobjekt heißt `responses`, im Gegensatz zu `requests`.</span><span class="sxs-lookup"><span data-stu-id="4358f-129">The property in the main JSON object is named `responses` as opposed to `requests`.</span></span>
* <span data-ttu-id="4358f-130">Einzelne Antworten werden möglicherweise in einer anderen Reihenfolge angezeigt als die Anforderungen.</span><span class="sxs-lookup"><span data-stu-id="4358f-130">Individual responses might appear in a different order than the requests.</span></span>
* <span data-ttu-id="4358f-131">Anstelle von `method` und `url` verfügen einzelne Antworten über eine `status`-Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="4358f-131">Rather than `method` and `url`, individual responses have a `status` property.</span></span> <span data-ttu-id="4358f-132">Der Wert von `status` ist eine Zahl, die den HTTP-Statuscode darstellt.</span><span class="sxs-lookup"><span data-stu-id="4358f-132">Rather than  and , individual responses have a  property. The value of `status` is a number that represents the HTTP status code.</span></span>

<span data-ttu-id="4358f-133">Der Statuscode einer Batchantwort lautet in der Regel `200` oder `400`.</span><span class="sxs-lookup"><span data-stu-id="4358f-133">The status code on a batch response is typically `200` or `400`.</span></span> <span data-ttu-id="4358f-134">Wenn die Batchanforderung selbst falsch formatiert ist, lautet der Statuscode `400`.</span><span class="sxs-lookup"><span data-stu-id="4358f-134">If the batch request itself is malformed, the status code is `400`.</span></span> <span data-ttu-id="4358f-135">Wenn die Batchanforderung analysierbar ist, lautet der Statuscode `200`.</span><span class="sxs-lookup"><span data-stu-id="4358f-135">If the batch request is parseable, the status code is `200`.</span></span> <span data-ttu-id="4358f-136">Ein Statuscode `200` in der Batchantwort besagt nicht, dass die einzelnen Anforderungen innerhalb des Batches erfolgreich waren.</span><span class="sxs-lookup"><span data-stu-id="4358f-136">A `200` status code on the batch response does not indicate that the individual requests inside the batch succeeded.</span></span> <span data-ttu-id="4358f-137">Aus diesem Grund hat jede einzelne Antwort in der `responses`-Eigenschaft einen Statuscode.</span><span class="sxs-lookup"><span data-stu-id="4358f-137">This is why each individual response in the `responses` property has a status code.</span></span>

<span data-ttu-id="4358f-138">Zusätzlich zur `responses`-Eigenschaft kann auch eine `nextLink`-Eigenschaft in der Batchantwort enthalten sein.</span><span class="sxs-lookup"><span data-stu-id="4358f-138">In addition to the `responses` property, there might be a `nextLink` property in the batch response.</span></span> <span data-ttu-id="4358f-139">Diese ermöglicht es Microsoft Graph, eine Batchantwort zurückzugeben, sobald eine der einzelnen Anforderungen abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="4358f-139">This allows Microsoft Graph to return a batch response as soon as any of the individual requests has completed.</span></span> <span data-ttu-id="4358f-140">Um sicherzustellen, dass alle einzelnen Antworten empfangen wurden, folgen Sie weiterhin dem `nextLink`, solange er vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="4358f-140">To ensure that all individual responses have been received, continue to follow the `nextLink` as long as it exists.</span></span>

## <a name="sequencing-requests-with-the-dependson-property"></a><span data-ttu-id="4358f-141">Sequenzieren von Anforderungen mit der dependsOn-Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4358f-141">Sequencing requests with the dependsOn property</span></span>

<span data-ttu-id="4358f-142">Einzelne Anforderungen können mithilfe der `dependsOn`-Eigenschaft in einer bestimmten Reihenfolge ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="4358f-142">Individual requests can be executed in a specified order by using the `dependsOn` property.</span></span> <span data-ttu-id="4358f-143">Diese Eigenschaft ist ein Array von Zeichenfolgen, die auf die `id` einer anderen einzelnen Anforderung verweisen.</span><span class="sxs-lookup"><span data-stu-id="4358f-143">This property is an array of strings that reference the `id` of a different individual request.</span></span> <span data-ttu-id="4358f-144">Aus diesem Grund müssen die Werte für `id` eindeutig sein.</span><span class="sxs-lookup"><span data-stu-id="4358f-144">For this reason, the values for `id` must be unique.</span></span> <span data-ttu-id="4358f-145">In der folgenden Anforderung gibt der Client beispielsweise an, dass die Anforderungen 1 und 3 zuerst ausgeführt werden sollen, dann Anforderung 2 und dann Anforderung 4.</span><span class="sxs-lookup"><span data-stu-id="4358f-145">For example, in the following request, the client is specifying that requests 1 and 3 should be run first, then request 2, then request 4.</span></span>

```json
{
  "requests": [
    {
      "id": "1",
      "method": "GET",
      "url": "..."
    },
    {
      "id": "2",
      "dependsOn": [ "1" ],
      "method": "GET",
      "url": "..."
    },
    {
      "id": "3",
      "method": "GET",
      "url": "..."
    },
    {
      "id": "4",
      "dependsOn": [ "2" ],
      "method": "GET",
      "url": "..."
    }
  ]
}
```

<span data-ttu-id="4358f-146">Wenn beim Ausführen einer einzelnen Anforderung ein Fehler auftritt, tritt bei allen Anforderungen, die von der betreffenden Anforderung abhängen, ein Fehler mit dem Statuscode `424` (Abhängigkeitsfehler) auf.</span><span class="sxs-lookup"><span data-stu-id="4358f-146">If an individual request fails, any request that depends on that request fails with status code `424` (Failed Dependency).</span></span>

## <a name="bypassing-url-length-limitations-with-batching"></a><span data-ttu-id="4358f-147">Umgehen von URL-Längenbeschränkungen durch Batchverarbeitung</span><span class="sxs-lookup"><span data-stu-id="4358f-147">Bypassing URL length limitations with batching</span></span>

<span data-ttu-id="4358f-p113">Ein weiterer Anwendungsfall für die JSON-Batchverarbeitung ist die Umgehung von URL-Längenbeschränkungen. Im Fall einer komplexen Filterklausel kann es passieren, dass die URL die in Browsern oder anderen HTTP-Clients integrierten Längenbeschränkungen nicht einhält. Sie können die JSON-Batchverarbeitung als Problemumgehung zum Ausführen dieser Anforderungen verwenden, da die lange URL einfach Teil der Anforderungsnutzlast wird.</span><span class="sxs-lookup"><span data-stu-id="4358f-p113">An additional use case for JSON batching is to bypass URL length limitations. In cases where the filter clause is complex, the URL length might surpass limitations built into browsers or other HTTP clients. You can use JSON batching as a workaround for running these requests because the lengthy URL simply becomes part of the request payload.</span></span>

## <a name="known-issues"></a><span data-ttu-id="4358f-151">Bekannte Probleme</span><span class="sxs-lookup"><span data-stu-id="4358f-151">Known issues</span></span>

<span data-ttu-id="4358f-152">Eine Liste von aktuellen Beschränkungen im Zusammenhang mit der Batchverarbeitung finden Sie unter [bekannte Probleme][batching-known-issues].</span><span class="sxs-lookup"><span data-stu-id="4358f-152">For a list of current limitations related to batching, see [known issues][batching-known-issues].</span></span>

[batching-known-issues]: https://developer.microsoft.com/en-us/graph/docs/concepts/known_issues#json-batching
[odata-4.01-json]: https://www.oasis-open.org/committees/download.php/60365/odata-json-format-v4.01-wd02-2017-03-24.docx


## <a name="see-also"></a><span data-ttu-id="4358f-153">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="4358f-153">See also</span></span>

<span data-ttu-id="4358f-154">Weitere Informationen zum Format von JSON-Batchanforderungen/-antworten finden Sie in der [OData JSON-Formatspezifikation Version 4.01][odata-4.01-json], Abschnitt 18.</span><span class="sxs-lookup"><span data-stu-id="4358f-154">For more information about the JSON batch request/response format, see the [OData JSON Format Version 4.01 specification][odata-4.01-json], section 18. Note that this specification is currently in a draft version, but is not expected to change.</span></span> <span data-ttu-id="4358f-155">Beachten Sie, dass diese Spezifikation derzeit eine Entwurfsversion ist, eine Änderung wird jedoch nicht erwartet.</span><span class="sxs-lookup"><span data-stu-id="4358f-155">For more information about the JSON batch request/response format, see the OData JSON Format Version 4.01 specification, section 18. Note that this specification is currently in a draft version, but is not expected to change.</span></span>

