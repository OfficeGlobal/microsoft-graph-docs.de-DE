# <a name="get-incremental-changes-to-messages-in-a-folder"></a><span data-ttu-id="3b9bb-101">Inkrementelle Änderungen an Nachrichten in einem Ordner abrufen</span><span class="sxs-lookup"><span data-stu-id="3b9bb-101">Get incremental changes to messages in a folder</span></span> 

<span data-ttu-id="3b9bb-p101">Mit der Delta-Abfrage können Sie Ergänzungen, Löschungen oder Aktualisierungen an Nachrichten in einem Ordner anhand einer Serie von [Delta](../api-reference/v1.0/api/message_delta.md)-Funktionsaufrufen abfragen. Mit Delta-Daten können Sie einen lokalen Speicher für Nachrichten eines Benutzers pflegen und synchronisieren, ohne dass Sie jedes Mal den gesamten Nachrichtensatz vom Server abrufen müssen.</span><span class="sxs-lookup"><span data-stu-id="3b9bb-p101">Delta query lets you query for additions, deletions, or updates to messages in a folder, by way of a series of [delta](../api-reference/v1.0/api/message_delta.md) function calls. Delta data enables you to maintain and synchronize a local store of a user's messages, without having to fetch the entire set of the user's messages from the server every time.</span></span>

<span data-ttu-id="3b9bb-p102">Die Delta-Abfrage unterstützt die vollständige Synchronisierung, die alle Nachrichten in einem Ordner abruft (z. B. im Posteingang des Benutzers), und die inkrementelle Synchronisierung, die alle Nachrichten abruft, die seit der letzten Synchronisierung in diesem Ordner geändert wurden. In der Regel führen Sie erst eine vollständige Synchronisierung aller Nachrichten in einem Ordner durch und rufen anschließend regelmäßig inkrementelle Änderungen an dem Ordner ab.</span><span class="sxs-lookup"><span data-stu-id="3b9bb-p102">Delta query supports both full synchronization that retrieves all of the messages in a folder (for example, the user's Inbox), and incremental synchronization that retrieves all of the messages that have changed in that folder since the last synchronization. Typically, you would do an initial full synchronization of all the messages in a folder, and subsequently, get incremental changes to that folder periodically.</span></span> 

## <a name="track-message-changes-in-a-folder"></a><span data-ttu-id="3b9bb-106">Nachverfolgen von Nachrichtenänderungen in einem Ordner</span><span class="sxs-lookup"><span data-stu-id="3b9bb-106">Track message changes in a folder</span></span>

<span data-ttu-id="3b9bb-p103">Die Delta-Abfrage wird jeweils für einen Ordner durchgeführt. Um die Änderungen der Nachrichten in einer Ordnerhierarchie nachzuverfolgen, müssen Sie jeden Ordner einzeln nachverfolgen.</span><span class="sxs-lookup"><span data-stu-id="3b9bb-p103">Delta query is a per-folder operation. To track the changes of the messages in a folder hierarchy, you need to track each folder individually.</span></span> 

<span data-ttu-id="3b9bb-p104">Das Nachverfolgen von Nachrichtenänderungen in einem Ordner ist in der Regel eine Runde aus einer oder mehreren GET-Anforderungen mit der **Delta**-Funktion. Die ursprüngliche GET-Anforderung wird ähnlich wie das [Abrufen von Nachrichten](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/user_list_messages) durchgeführt, außer dass die folgende **delta**-Funktion eingeschlossen wird:</span><span class="sxs-lookup"><span data-stu-id="3b9bb-p104">Tracking message changes in a mail folder typically is a round of one or more GET requests with the **delta** function. The initial GET request is very much like the way you [get messages](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/user_list_messages), except that you include the **delta** function:</span></span>

```
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/messages/delta
```

<span data-ttu-id="3b9bb-111">Eine GET-Anforderung mit der **delta**-Funktion gibt Folgendes zurück:</span><span class="sxs-lookup"><span data-stu-id="3b9bb-111">A GET request with the **delta** function returns either:</span></span>

- <span data-ttu-id="3b9bb-112">`nextLink` (mit einer URL mit einem **delta**-Funktionsaufruf und einem _skipToken_) oder</span><span class="sxs-lookup"><span data-stu-id="3b9bb-112">A `nextLink` (that contains a URL with a **delta** function call and a _skipToken_), or</span></span> 
- <span data-ttu-id="3b9bb-113">`deltaLink` (mit einer URL mit einem **delta**-Funktionsaufruf und einem _deltaToken_).</span><span class="sxs-lookup"><span data-stu-id="3b9bb-113">A `deltaLink` (that contains a URL with a **delta** function call and _deltaToken_).</span></span>

<span data-ttu-id="3b9bb-p105">Diese Token sind [Statustoken](delta_query_overview.md#state-tokens), die für den Client nicht transparent sind. Um mit einer Änderungsnachverfolgung fortzufahren, kopieren Sie die von der letzten GET-Anforderung zurückgegebene URL einfach und wenden sie auf den nächsten **delta**-Funktionsaufruf für denselben Ordner an.  `deltaLink` (in einer Antwort zurückgegeben), bedeutet, dass die aktuelle Runde der Änderungsnachverfolgung abgeschlossen ist. Sie können die `deltaLink`-URL für die nächste Runde speichern und verwenden.</span><span class="sxs-lookup"><span data-stu-id="3b9bb-p105">These tokens are [state tokens](delta_query_overview.md#state-tokens) that are completely opaque to the client. To proceed with a round of change tracking, simply copy and apply the URL returned from the last GET request to the next **delta** function call for the same folder. A `deltaLink` returned in a response signifies that the current round of change tracking is complete. You can save and use the `deltaLink` URL when you begin the next round.</span></span>

<span data-ttu-id="3b9bb-118">Im [Beispiel](#example-to-synchronize-messages-in-a-folder) unten finden Sie Informationen zur Verwendung der `nextLink`- und `deltaLink`-URLs.</span><span class="sxs-lookup"><span data-stu-id="3b9bb-118">See the [example](#example-to-synchronize-messages-in-a-folder) below to learn how to use the `nextLink` and `deltaLink` URLs.</span></span>

### <a name="use-query-parameters-in-a-delta-query-for-messages"></a><span data-ttu-id="3b9bb-119">Verwenden von Abfrageparametern in einer Delta-Abfrage für Nachrichten</span><span class="sxs-lookup"><span data-stu-id="3b9bb-119">Use query parameters in a delta query for messages</span></span>

- <span data-ttu-id="3b9bb-p106">Sie können wie bei jeder GET-Anforderung den Abfrageparameter `$select` verwenden, um zwecks Leistungsoptimierung nur die benötigten Eigenschaften anzugeben. Die Eigenschaft _id_ wird immer zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3b9bb-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 
- <span data-ttu-id="3b9bb-122">Die Delta-Abfrage unterstützt `$select`, `$top` und `$expand` für Nachrichten.</span><span class="sxs-lookup"><span data-stu-id="3b9bb-122">Delta query support `$select`, `$top`, and `$expand` for messages.</span></span> 
- <span data-ttu-id="3b9bb-123">Es besteht eingeschränkte Unterstützung für `$filter` und `$orderby`:</span><span class="sxs-lookup"><span data-stu-id="3b9bb-123">There is limited support for `$filter` and `$orderby`:</span></span>
  * <span data-ttu-id="3b9bb-124">Es werden nur die `$filter`-Ausdrücke `$filter=receivedDateTime+ge+{value}` oder `$filter=receivedDateTime+gt+{value}` unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3b9bb-124">The only supported `$filter` expresssions are `$filter=receivedDateTime+ge+{value}` or `$filter=receivedDateTime+gt+{value}`.</span></span>
  * <span data-ttu-id="3b9bb-p107">Es wird nur der `$orderby`-Ausdruck `$orderby=receivedDateTime+desc` unterstützt. Wenn Sie keinen `$orderby`-Ausdruck einschließen, ist die Rückgabereihenfolge nicht gewährleistet.</span><span class="sxs-lookup"><span data-stu-id="3b9bb-p107">The only supported `$orderby` expression is `$orderby=receivedDateTime+desc`. If you do not include an `$orderby` expression, the return order is not guaranteed.</span></span> 
- <span data-ttu-id="3b9bb-127">`$search` wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3b9bb-127">There is no support for `$search`.</span></span>


### <a name="optional-request-header"></a><span data-ttu-id="3b9bb-128">Optionaler Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3b9bb-128">Optional request header</span></span>

<span data-ttu-id="3b9bb-p108">Jede GET-Anforderung der Delta-Abfrage gibt eine Sammlung aus einer oder mehreren Nachrichten in der Antwort zurück. Sie können optional den Anforderungsheader, _Prefer: odata.maxpagesize={x}_, angeben, um die maximale Anzahl an Nachrichten in einer Antwort festzulegen.</span><span class="sxs-lookup"><span data-stu-id="3b9bb-p108">Each delta query GET request returns a collection of one or more messages in the response. You can optionally specify the request header, _Prefer: odata.maxpagesize={x}_, to set the maximum number of messages in a response.</span></span>

<!--
### Iterative process 

A typical round to track message changes goes like this:

1. Make the initial GET request with the mandatory _Prefer: odata.track-changes_ header. If this is your very first delta query 
for messages in that folder, don't provide any state token. If the messages support tracking changes, following the iterative 
process (steps 2-6) described below will return the entire set of messages in that folder. 

2. Check if the first response returns the _Preference-Applied: odata.track-changes_ header, 
which confirms your resource supports tracking changes. Stop if you don't receive the response header.

3. If you receive a _skipToken_ (in an _@odata.nextLink_ response header) in the response, you should continue to track the
   additional messages that have changed (added, deleted, or updated). Make a second GET request, using the URL returned 
   in _@odata.nextLink_, which includes a _skipToken_. 

4. The second request will return additional messages that have changed, and either a _skipToken_ if there are more changed messages, 
  or a _deltaToken_ if all the changed messages have been returned.

5. If you receive a _skipToken_ from the last GET request, continue getting the changes by sending a next GET call, similar to step 3. 

6. When you eventually receive a _detlaToken (in an _@odata.deltaLink_ response header) in the response from a GET, stop. This 
round of change tracking is complete. 

7. Save the _deltaToken_. The next time you track changes for the same folder, make a GET request 
similar to step 1, except that now you can use this _deltaToken_ to get just the delta data (messages that have been added, deleted or updated) 
since the completion of the very first round.

-->

## <a name="example-to-synchronize-messages-in-a-folder"></a><span data-ttu-id="3b9bb-131">Beispiel für die Synchronisierung von Nachrichten in einem Ordner</span><span class="sxs-lookup"><span data-stu-id="3b9bb-131">Example to synchronize messages in a folder</span></span>

<span data-ttu-id="3b9bb-132">Das folgende Beispiel zeigt eine Reihe von 3 Anforderungen zum Synchronisieren eines bestimmten Ordners, der 5 Nachrichten enthält:</span><span class="sxs-lookup"><span data-stu-id="3b9bb-132">The following example shows a series of 3 requests to synchronize a specific folder which contains 5 messages:</span></span>

- <span data-ttu-id="3b9bb-133">[Beispiel für ursprüngliche Anforderung](#sample-initial-request) und [Antwort](#sample-initial-response)</span><span class="sxs-lookup"><span data-stu-id="3b9bb-133">[Sample initial request](#sample-initial-request) and [response](#sample-initial-response)</span></span>
- <span data-ttu-id="3b9bb-134">[Beispiel für zweite Anforderung](#sample-second-request) und [Antwort](#sample-second-response)</span><span class="sxs-lookup"><span data-stu-id="3b9bb-134">[Sample second request](#sample-second-request) and [response](#sample-second-response)</span></span>
- <span data-ttu-id="3b9bb-135">[Beispiel für dritte Anforderung](#sample-third-request) und [letzte Antwort](#sample-third-and-final-response)</span><span class="sxs-lookup"><span data-stu-id="3b9bb-135">[Sample third request](#sample-third-request) and [final response](#sample-third-and-final-response)</span></span>

<span data-ttu-id="3b9bb-136">Sehen Sie sich auch an, was Sie in der [nächsten Runde](#the-next-round) tun werden.</span><span class="sxs-lookup"><span data-stu-id="3b9bb-136">See also what you'll do in the [next round](#the-next-round).</span></span>


### <a name="sample-initial-request"></a><span data-ttu-id="3b9bb-137">Beispiel für ursprüngliche Anforderung</span><span class="sxs-lookup"><span data-stu-id="3b9bb-137">Sample initial request</span></span>

<span data-ttu-id="3b9bb-p109">In diesem Beispiel wird der angegebene Ordner zum ersten Mal synchronisiert, sodass die ursprüngliche Synchronisierungsanforderung kein Statustoken enthält. In dieser Runde werden alle Nachrichten in diesem Ordner zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3b9bb-p109">In this example, the specified folder is being synchronized for the first time, so the initial sync request does not include any state token. This round will return all the messages in that folder.</span></span>

<span data-ttu-id="3b9bb-140">Die erste Anforderung gibt Folgendes an:</span><span class="sxs-lookup"><span data-stu-id="3b9bb-140">The first request specifies the following:</span></span>

- <span data-ttu-id="3b9bb-141">Einen Parameter `$select` zum Zurückgeben der Eigenschaften **Subject** und **Sender** für jede Nachricht in der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3b9bb-141">A `$select` parameter to return the **Subject** and **Sender** properties for each message in the response.</span></span>
- <span data-ttu-id="3b9bb-142">Den [optionalen Anforderungsheader](#optional-request-header), _odata.maxpagesize_, der gleichzeitig 2 Nachrichten zurückgibt.</span><span class="sxs-lookup"><span data-stu-id="3b9bb-142">The [optional request header](#optional-request-header), _odata.maxpagesize_, returning 2 messages at a time.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_messages_delta_1"
}-->
```
GET https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$select=Subject,Sender HTTP/1.1
Prefer: odata.maxpagesize=2
```


### <a name="sample-initial-response"></a><span data-ttu-id="3b9bb-143">Beispiel für ursprüngliche Antwort</span><span class="sxs-lookup"><span data-stu-id="3b9bb-143">Sample initial response</span></span>

<span data-ttu-id="3b9bb-p110">Die Antwort enthält zwei Nachrichten und einen `@odata.nextLink`-Antwortheader. Die `nextLink`-URL zeigt an, dass weitere abzurufende Nachrichten in dem Ordner vorhanden sind.</span><span class="sxs-lookup"><span data-stu-id="3b9bb-p110">The response includes two messages and an `@odata.nextLink` response header. The `nextLink` URL indicates there are more messages in the folder to get.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```
{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(message)",
    "@odata.nextLink":"https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$skiptoken=GwcBoTmPuoTQWfcsAbkYM",
    "value":[
        {
            "@odata.type":"#microsoft.graph.message",
            "@odata.etag":"W/\"CQAAABYAAAARn2vdzPFjSbaPPxzjlzOTAAASsKZz\"",
            "subject":"Holiday hours update",
            "sender":{
                "emailAddress":{
                    "name":"Dana Swope",
                    "address":"danas@contoso.onmicrosoft.com"
                }
            },
            "id":"AAMkADNkNAAASq35xAAA="
        },
        {
            "@odata.type":"#microsoft.graph.message",
            "@odata.etag":"W/\"CQAAABYAAAARn2vdzPFjSbaPPxzjlzOTAAAEfYB/\"",
            "subject":"Holiday promotion sale",
            "sender":{
                "emailAddress":{
                    "name":"Samantha Booth",
                    "address":"samanthab@contoso.onmicrosoft.com"
                }
            },
            "id":"AQMkADNkNAAAVRMKAAAAA=="
        }
    ]
}
```

### <a name="sample-second-request"></a><span data-ttu-id="3b9bb-146">Beispiel für zweite Anforderung</span><span class="sxs-lookup"><span data-stu-id="3b9bb-146">Sample second request</span></span>

<span data-ttu-id="3b9bb-p111">Die zweite Anforderung gibt die aus der vorherigen Antwort zurückgegebene `nextLink`-URL an. Beachten Sie, dass sie nicht denselben Parameter `$select` wie in der ursprünglichen Anforderung angeben muss, da das `skipToken` in der `nextLink`-URL es codiert und einschließt.</span><span class="sxs-lookup"><span data-stu-id="3b9bb-p111">The second request specifies the `nextLink` URL returned from the previous response. Notice that it no longer has to specify the same `$select` parameter as in the initial request, as the `skipToken` in the `nextLink` URL encodes and includes it.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_messages_delta_2"
}-->
```
GET https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$skiptoken=GwcBoTmPuoTQWfcsAbkYM HTTP/1.1
Prefer: odata.maxpagesize=2
```

### <a name="sample-second-response"></a><span data-ttu-id="3b9bb-149">Beispiel für zweite Antwort</span><span class="sxs-lookup"><span data-stu-id="3b9bb-149">Sample second response</span></span> 

<span data-ttu-id="3b9bb-150">Die zweite Antwort gibt die nächsten 2 Nachrichten in dem Ordner zurück und ein weiteres `nextLink`, was bedeutet, dass weitere abzurufende Nachrichten in dem Ordner vorhanden sind.</span><span class="sxs-lookup"><span data-stu-id="3b9bb-150">The second response returns the next 2 messages in the folder and another `nextLink`, indicating there are more messages to get from the folder.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```
{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(message)",
    "@odata.nextLink":"https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$skiptoken=GwcBoTmPKILK4jLH7mAd1lLU",
    "value":[
        {
            "@odata.type":"#microsoft.graph.message",
            "@odata.etag":"W/\"CQAAABYAAAARn2vdzPFjSbaPPxzjlzOTAAAEfYB+\"",
            "subject":"New or modified user account information",
            "sender":{
                "emailAddress":{
                    "name":"Randi Welch",
                    "address":"randiw@contoso.onmicrosoft.com"
                }
            },
            "id":"AQMkADNkNAAAgWJAAAA"
        },
        {
            "@odata.type":"#microsoft.graph.message",
            "@odata.etag":"W/\"CQAAABYAAAARn2vdzPFjSbaPPxzjlzOTAAAEfYB9\"",
            "subject":"New or modified user account information",
            "sender":{
                "emailAddress":{
                    "name":"Randi Welch",
                    "address":"randiw@contoso.onmicrosoft.com"
                }
            },
            "id":"AQMkADNkNAAAgWHAAAA"
        }
    ]
}
```


### <a name="sample-third-request"></a><span data-ttu-id="3b9bb-151">Beispiel für dritte Anforderung</span><span class="sxs-lookup"><span data-stu-id="3b9bb-151">Sample third request</span></span>

<span data-ttu-id="3b9bb-152">Die dritte Anforderung verwendet weiterhin die neueste aus der letzten Synchronisierungsanforderung zurückgegebene `nextLink`-URL.</span><span class="sxs-lookup"><span data-stu-id="3b9bb-152">The third request continues to use the latest `nextLink` URL returned from the last sync request.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_messages_delta_3"
}-->
```
GET https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$skiptoken=GwcBoTmPKILK4jLH7mAd1lLU HTTP/1.1
Prefer: odata.maxpagesize=2
```

### <a name="sample-third-and-final-response"></a><span data-ttu-id="3b9bb-153">Beispiel für dritte und letzte Antwort</span><span class="sxs-lookup"><span data-stu-id="3b9bb-153">Sample third and final response</span></span>

<span data-ttu-id="3b9bb-p112">Die dritte Antwort gibt die einzige in dem Ordner verbleibende Nachricht zurück sowie eine `deltaLink`-URL zurück, was bedeutet, dass die Synchronisierung für diesen Ordner momentan abgeschlossen ist. Speichern und verwenden Sie die `deltaLink`-URL, um [den gleichen Ordner in der nächsten Runde zu synchronisieren](#the-next-round).</span><span class="sxs-lookup"><span data-stu-id="3b9bb-p112">The third response returns the only remaining message in the folder, and a `deltaLink` URL which indicates synchronization is complete for the time being for this folder. Save and use the `deltaLink` URL to [synchronize the same folder in the next round](#the-next-round).</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```
{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(message)",
    "@odata.deltaLink":"https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$deltatoken=GwcBoTmPuoGNlgXgF1nyUNMXY",
    "value":[
        {
            "@odata.type":"#microsoft.graph.message",
            "@odata.etag":"W/\"CQAAABYAAAARn2vdzPFjSbaPPxzjlzOTAAAEfYB8\"",
            "subject":"You've joined the Customer Manager group",
            "sender":{
                "emailAddress":{
                    "name":"Customer Managers team",
                    "address":"customer_managers@contoso.onmicrosoft.com"
                }
            },
            "id":"AQMkADNkNAAAgWFAAAA"
        }
    ]
}
```


### <a name="the-next-round"></a><span data-ttu-id="3b9bb-156">Die nächste Runde</span><span class="sxs-lookup"><span data-stu-id="3b9bb-156">The next round</span></span>

<span data-ttu-id="3b9bb-p113">Mit dem `deltaLink` aus der [letzten Anforderung](#sample-third-request) in der letzten Runde können Sie nur die Nachrichten abrufen, die sich seitdem in diesem Ordner geändert haben (durch Hinzufügung, Löschung oder Aktualisierung). Ihre erste Anforderung in der nächsten Runde sieht folgendermaßen aus, sofern Sie die gleiche maximale Seitengröße in der Antwort beibehalten möchten:</span><span class="sxs-lookup"><span data-stu-id="3b9bb-p113">Using the `deltaLink` from the [last request](#sample-third-request) in the last round, you will be able to get only those messages that have changed (by being added, deleted, or updated) in that folder since then. Your first request in the next round will look like the following, assuming you prefer to keep the same maximum page size in the response:</span></span>

<!-- {
  "blockType": "request",
  "name": "get_messages_delta_next"
}-->
```
GET https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$deltatoken=GwcBoTmPuoGNlgXgF1nyUNMXY HTTP/1.1
Prefer: odata.maxpagesize=2
```



## <a name="see-also"></a><span data-ttu-id="3b9bb-159">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="3b9bb-159">See also</span></span>

- [<span data-ttu-id="3b9bb-160">Microsoft Graph-Delta-Abfrage</span><span class="sxs-lookup"><span data-stu-id="3b9bb-160">Microsoft Graph delta query</span></span>](../Concepts/delta_query_overview.md)
- [<span data-ttu-id="3b9bb-161">Inkrementelle Änderungen an Ereignissen in einer Kalenderansicht abrufen</span><span class="sxs-lookup"><span data-stu-id="3b9bb-161">Get incremental changes to events in a calendar view</span></span>](../Concepts/delta_query_events.md)
- [<span data-ttu-id="3b9bb-162">Inkrementelle Änderungen an Gruppen abrufen</span><span class="sxs-lookup"><span data-stu-id="3b9bb-162">Get incremental changes to groups</span></span>](../Concepts/delta_query_groups.md)
- [<span data-ttu-id="3b9bb-163">Inkrementelle Änderungen an Benutzern abrufen</span><span class="sxs-lookup"><span data-stu-id="3b9bb-163">Get incremental changes to users</span></span>](../Concepts/delta_query_users.md)
