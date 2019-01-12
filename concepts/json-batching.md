---
title: Kombinieren von mehreren Anforderungen in einem HTTP-Aufruf unter Verwendung der JSON-Batchverarbeitung
description: 'Die JSON-Batchverarbeitung ermöglicht es Ihnen, Ihre Anwendung durch Kombinieren von mehreren Anforderungen in einem einzigen JSON-Objekt zu optimieren. Ein Client möchte z. B. eine Ansicht aus nicht verbundenen Daten wie den folgenden zusammenstellen:'
author: piotrci
localization_priority: Priority
ms.openlocfilehash: f36cc1c8e8ccc016078eab52c4c7f3874892d000
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885183"
---
# <a name="combine-multiple-requests-in-one-http-call-using-json-batching"></a><span data-ttu-id="4fd24-104">Kombinieren von mehreren Anforderungen in einem HTTP-Aufruf unter Verwendung der JSON-Batchverarbeitung</span><span class="sxs-lookup"><span data-stu-id="4fd24-104">Combine multiple requests in one HTTP call using JSON batching</span></span>

<span data-ttu-id="4fd24-p102">Die JSON-Batchverarbeitung ermöglicht es Ihnen, Ihre Anwendung durch Kombinieren von mehreren Anforderungen in einem einzigen JSON-Objekt zu optimieren. Ein Client möchte z. B. eine Ansicht aus nicht verbundenen Daten wie den folgenden zusammenstellen:</span><span class="sxs-lookup"><span data-stu-id="4fd24-p102">JSON batching allows you to optimize your application by combining multiple requests into a single JSON object. For example, a client might want to compose a view of unrelated data such as:</span></span>

1. <span data-ttu-id="4fd24-107">Ein in OneDrive gespeichertes Bild</span><span class="sxs-lookup"><span data-stu-id="4fd24-107">An image stored in OneDrive</span></span>
2. <span data-ttu-id="4fd24-108">Eine Liste von Planner-Aufgaben</span><span class="sxs-lookup"><span data-stu-id="4fd24-108">A list of Planner tasks</span></span>
3. <span data-ttu-id="4fd24-109">Der Kalender für eine Gruppe</span><span class="sxs-lookup"><span data-stu-id="4fd24-109">The calendar for a group</span></span>

<span data-ttu-id="4fd24-110">Indem Sie diese drei einzelnen Anforderungen in einer einzigen Batchanforderung kombinieren, können Sie die Netzwerklatenz der Anwendung erheblich reduzieren.</span><span class="sxs-lookup"><span data-stu-id="4fd24-110">Combining these three individual requests into a single batch request can save the application significant network latency.</span></span>

## <a name="first-json-batch-request"></a><span data-ttu-id="4fd24-111">Erste JSON-Batchanforderung</span><span class="sxs-lookup"><span data-stu-id="4fd24-111">First JSON batch request</span></span>

<span data-ttu-id="4fd24-p103">Zunächst erstellen Sie die JSON-Batchanforderung für das vorherige Beispiel. In diesem Szenario sind die einzelnen Anforderungen in keiner Weise voneinander abhängig und können daher in beliebiger Reihenfolge in der Batchanforderung platziert werden.</span><span class="sxs-lookup"><span data-stu-id="4fd24-p103">First you construct the JSON batch request for the previous example. In this scenario, the individual requests are not interdependent in any way and therefore can be placed into the batch request in any order.</span></span>

```http
POST https://graph.microsoft.com/v1.0/$batch
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
    },
    {
      "id": "4",
      "url": "/me",
      "method": "PATCH",
      "body": {
        "city" : "Redmond"
      },
      "headers": {
        "Content-Type": "application/json"
      }
    }
  ]
}
```

<span data-ttu-id="4fd24-p104">Antworten auf die zum Batch zusammengefassten Anforderungen werden möglicherweise in einer anderen Reihenfolge angezeigt. Die `id`-Eigenschaft kann verwendet werden, um einzelne Anforderungen und Antworten zu korrelieren.</span><span class="sxs-lookup"><span data-stu-id="4fd24-p104">Responses to the batched requests might appear in a different order. The `id` property can be used to correlate individual requests and responses.</span></span>

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
        "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.plannerTask)",
        "value": []
      }
    },
    {
      "id": "4",
      "status": 204,
      "body": null
    }
  ]
}
```

## <a name="request-format"></a><span data-ttu-id="4fd24-116">Anforderungsformat</span><span class="sxs-lookup"><span data-stu-id="4fd24-116">Request format</span></span>

<span data-ttu-id="4fd24-117">Batchanforderungen werden immer mithilfe von `POST` an den Endpunkt `/$batch` gesendet.</span><span class="sxs-lookup"><span data-stu-id="4fd24-117">Batch requests are always sent using `POST` to the `/$batch` endpoint.</span></span>

<span data-ttu-id="4fd24-p105">Der Textkörper einer JSON-Batchanforderung besteht aus einem einzelnen JSON-Objekt mit einer erforderlichen Eigenschaft: `requests`. Die `requests`-Eigenschaft ist ein Array von einzelnen Anforderungen. Für jede einzelne Anforderung sind die Eigenschaften `id`, `method` und `url` erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4fd24-p105">A JSON batch request body consists of a single JSON object with one required property: `requests`. The `requests` property is an array of individual requests. For each individual request, the `id`, `method`, and `url` properties are required.</span></span>

<span data-ttu-id="4fd24-p106">Die `id`-Eigenschaft dient in erster Linie als Korrelationswert zum Zuordnen einzelner Antworten zu Anforderungen. Dadurch kann der Server Anforderungen im Batch in der effizientesten Reihenfolge verarbeiten.</span><span class="sxs-lookup"><span data-stu-id="4fd24-p106">The `id` property functions primarily as a correlation value to associate individual responses with requests. This allows the server to process requests in the batch in the most efficient order.</span></span>

<span data-ttu-id="4fd24-p107">Die Eigenschaften `method` und `url` sind genau das, was Sie am Anfang jeder HTTP-Anforderung sehen. Die Methode ist die HTTP-Methode, und die URL ist die Ressourcen-URL, an die die einzelne Anforderung normalerweise gesendet wird.</span><span class="sxs-lookup"><span data-stu-id="4fd24-p107">The `method` and `url` properties are exactly what you would see at the start of any given HTTP request. The method is the HTTP method, and the URL is the resource URL the individual request would typically be sent to.</span></span>

<span data-ttu-id="4fd24-125">Einzelne Anforderungen können optional auch eine `headers`- und eine `body`-Eigenschaft enthalten.</span><span class="sxs-lookup"><span data-stu-id="4fd24-125">Individual requests can optionally also contain a `headers` property and a `body` property.</span></span> <span data-ttu-id="4fd24-126">Beide Eigenschaften sind in der Regel JSON-Objekte, wie im vorherigen Beispiel gezeigt.</span><span class="sxs-lookup"><span data-stu-id="4fd24-126">Both of these properties are typically JSON objects, as shown in the previous example.</span></span> <span data-ttu-id="4fd24-127">In einigen Fällen ist die `body`-Eigenschaft möglicherweise ein base64-codierter URL-Wert anstelle eines JSON Objekts, beispielsweise wenn der Textkörper ein Bild ist.</span><span class="sxs-lookup"><span data-stu-id="4fd24-127">In some cases, the `body` might be a base64 URL-encoded value rather than a JSON object - for example, when the body is an image.</span></span> <span data-ttu-id="4fd24-128">Wenn ein `body` in der Anforderung enthalten ist, muss das `headers`-Objekt einen Wert für `Content-Type` enthalten.</span><span class="sxs-lookup"><span data-stu-id="4fd24-128">When a `body` is included with the request, the `headers` object must contain a value for `Content-Type`.</span></span>

## <a name="response-format"></a><span data-ttu-id="4fd24-129">Antwortformat</span><span class="sxs-lookup"><span data-stu-id="4fd24-129">Response format</span></span>

<span data-ttu-id="4fd24-p109">Das Antwortformat für JSON-Batchanforderungen ähnelt dem Anforderungsformat. Die wichtigsten Unterschiede sind folgende:</span><span class="sxs-lookup"><span data-stu-id="4fd24-p109">The response format for JSON batch requests is similar to the request format. The following are the key differences:</span></span>

* <span data-ttu-id="4fd24-132">Die Eigenschaft im JSON-Hauptobjekt heißt `responses`, im Gegensatz zu `requests`.</span><span class="sxs-lookup"><span data-stu-id="4fd24-132">The property in the main JSON object is named `responses` as opposed to `requests`.</span></span>
* <span data-ttu-id="4fd24-133">Einzelne Antworten werden möglicherweise in einer anderen Reihenfolge angezeigt als die Anforderungen.</span><span class="sxs-lookup"><span data-stu-id="4fd24-133">Individual responses might appear in a different order than the requests.</span></span>
* <span data-ttu-id="4fd24-p110">Anstelle von `method` und `url` verfügen einzelne Antworten über eine `status`-Eigenschaft. Der Wert von `status` ist eine Zahl, die den HTTP-Statuscode darstellt.</span><span class="sxs-lookup"><span data-stu-id="4fd24-p110">Rather than `method` and `url`, individual responses have a `status` property. The value of `status` is a number that represents the HTTP status code.</span></span>

<span data-ttu-id="4fd24-p111">Der Statuscode einer Batchantwort lautet in der Regel `200` oder `400`. Wenn die Batchanforderung selbst falsch formatiert ist, lautet der Statuscode `400`. Wenn die Batchanforderung analysierbar ist, lautet der Statuscode `200`. Ein Statuscode `200` in der Batchantwort besagt nicht, dass die einzelnen Anforderungen innerhalb des Batches erfolgreich waren. Aus diesem Grund hat jede einzelne Antwort in der `responses`-Eigenschaft einen Statuscode.</span><span class="sxs-lookup"><span data-stu-id="4fd24-p111">The status code on a batch response is typically `200` or `400`. If the batch request itself is malformed, the status code is `400`. If the batch request is parseable, the status code is `200`. A `200` status code on the batch response does not indicate that the individual requests inside the batch succeeded. This is why each individual response in the `responses` property has a status code.</span></span>

<span data-ttu-id="4fd24-p112">Zusätzlich zur `responses`-Eigenschaft kann auch eine `nextLink`-Eigenschaft in der Batchantwort enthalten sein. Diese ermöglicht es Microsoft Graph, eine Batchantwort zurückzugeben, sobald eine der einzelnen Anforderungen abgeschlossen ist. Um sicherzustellen, dass alle einzelnen Antworten empfangen wurden, folgen Sie weiterhin dem `nextLink`, solange er vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="4fd24-p112">In addition to the `responses` property, there might be a `nextLink` property in the batch response. This allows Microsoft Graph to return a batch response as soon as any of the individual requests has completed. To ensure that all individual responses have been received, continue to follow the `nextLink` as long as it exists.</span></span>

## <a name="sequencing-requests-with-the-dependson-property"></a><span data-ttu-id="4fd24-144">Sequenzieren von Anforderungen mit der dependsOn-Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4fd24-144">Sequencing requests with the dependsOn property</span></span>

<span data-ttu-id="4fd24-p113">Einzelne Anforderungen können mithilfe der `dependsOn`-Eigenschaft in einer bestimmten Reihenfolge ausgeführt werden. Diese Eigenschaft ist ein Array von Zeichenfolgen, die auf die `id` einer anderen einzelnen Anforderung verweisen. Aus diesem Grund müssen die Werte für `id` eindeutig sein. In der folgenden Anforderung gibt der Client beispielsweise an, dass die Anforderungen 1 und 3 zuerst ausgeführt werden sollen, dann Anforderung 2 und dann Anforderung 4.</span><span class="sxs-lookup"><span data-stu-id="4fd24-p113">Individual requests can be executed in a specified order by using the `dependsOn` property. This property is an array of strings that reference the `id` of a different individual request. For this reason, the values for `id` must be unique. For example, in the following request, the client is specifying that requests 1 and 3 should be run first, then request 2, then request 4.</span></span>

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

<span data-ttu-id="4fd24-149">Wenn beim Ausführen einer einzelnen Anforderung ein Fehler auftritt, tritt bei allen Anforderungen, die von der betreffenden Anforderung abhängen, ein Fehler mit dem Statuscode `424` (Abhängigkeitsfehler) auf.</span><span class="sxs-lookup"><span data-stu-id="4fd24-149">If an individual request fails, any request that depends on that request fails with status code `424` (Failed Dependency).</span></span>

## <a name="bypassing-url-length-limitations-with-batching"></a><span data-ttu-id="4fd24-150">Umgehen von URL-Längenbeschränkungen durch Batchverarbeitung</span><span class="sxs-lookup"><span data-stu-id="4fd24-150">Bypassing URL length limitations with batching</span></span>

<span data-ttu-id="4fd24-p114">Ein weiterer Anwendungsfall für die JSON-Batchverarbeitung ist die Umgehung von URL-Längenbeschränkungen. Im Fall einer komplexen Filterklausel kann es passieren, dass die URL die in Browsern oder anderen HTTP-Clients integrierten Längenbeschränkungen nicht einhält. Sie können die JSON-Batchverarbeitung als Problemumgehung zum Ausführen dieser Anforderungen verwenden, da die lange URL einfach Teil der Anforderungsnutzlast wird.</span><span class="sxs-lookup"><span data-stu-id="4fd24-p114">An additional use case for JSON batching is to bypass URL length limitations. In cases where the filter clause is complex, the URL length might surpass limitations built into browsers or other HTTP clients. You can use JSON batching as a workaround for running these requests because the lengthy URL simply becomes part of the request payload.</span></span>

## <a name="known-issues"></a><span data-ttu-id="4fd24-154">Bekannte Probleme</span><span class="sxs-lookup"><span data-stu-id="4fd24-154">Known issues</span></span>

<span data-ttu-id="4fd24-155">Eine Liste von aktuellen Beschränkungen im Zusammenhang mit der Batchverarbeitung finden Sie unter [bekannte Probleme][batching-known-issues].</span><span class="sxs-lookup"><span data-stu-id="4fd24-155">For a list of current limitations related to batching, see [known issues][batching-known-issues].</span></span>

[batching-known-issues]: known-issues.md#json-batching
[odata-4.01-json]: https://www.oasis-open.org/committees/download.php/60365/odata-json-format-v4.01-wd02-2017-03-24.docx


## <a name="see-also"></a><span data-ttu-id="4fd24-156">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="4fd24-156">See also</span></span>

<span data-ttu-id="4fd24-p115">Weitere Informationen zum Format von JSON-Batchanforderungen/-antworten finden Sie in der [OData JSON-Formatspezifikation Version 4.01][odata-4.01-json], Abschnitt 18. Beachten Sie, dass diese Spezifikation derzeit eine Entwurfsversion ist, eine Änderung wird jedoch nicht erwartet.</span><span class="sxs-lookup"><span data-stu-id="4fd24-p115">For more information about the JSON batch request/response format, see the [OData JSON Format Version 4.01 specification][odata-4.01-json], section 18. Note that this specification is currently in a draft version, but is not expected to change.</span></span>

