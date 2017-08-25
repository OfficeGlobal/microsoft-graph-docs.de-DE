# <a name="message-delta"></a><span data-ttu-id="3ce74-101">message: delta</span><span class="sxs-lookup"><span data-stu-id="3ce74-101">message: delta</span></span>

<span data-ttu-id="3ce74-102">Dient zum Abrufen eines Satzes von Nachrichten, die einem bestimmten Ordner hinzugefügt bzw. daraus gelöscht oder darin aktualisiert wurden.</span><span class="sxs-lookup"><span data-stu-id="3ce74-102">Get a set of messages that have been added, deleted, or updated in a specified folder.</span></span>

<span data-ttu-id="3ce74-p101">Ein **delta**-Funktionsaufruf für Nachrichten in einem Ordner ähnelt einer GET-Anforderung, mit der Ausnahme, dass durch entsprechende Anwendung von [Statustoken](../../../concepts/delta_query_overview.md) in einem oder mehreren dieser Aufrufe [inkrementelle Änderungen an den Nachrichten im betreffenden Ordner abgefragt](../../../concepts/delta_query_messages.md) werden können. Dies ermöglicht es Ihnen, einen lokalen Speicher der Nachrichten eines Benutzers zu pflegen und zu synchronisieren, ohne dass Sie jedes Mal den gesamten Satz Nachrichten vom Server abrufen müssen.</span><span class="sxs-lookup"><span data-stu-id="3ce74-p101">A **delta** function call for messages in a folder is similar to a GET request, except that by appropriately applying [state tokens](../../../concepts/delta_query_overview.md) in one or more of these calls, you can [query for incremental changes in the messages in that folder](../../../concepts/delta_query_messages.md). This allows you to maintain and synchronize a local store of a user's messages without having to fetch the entire set of messages from the server every time.</span></span>  

## <a name="permissions"></a><span data-ttu-id="3ce74-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3ce74-105">Permissions</span></span>
<span data-ttu-id="3ce74-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3ce74-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3ce74-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3ce74-108">Permission type</span></span>      | <span data-ttu-id="3ce74-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3ce74-109">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="3ce74-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3ce74-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3ce74-111">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3ce74-111">Mail.Read, Mail.ReadWrite</span></span>    | 
|<span data-ttu-id="3ce74-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3ce74-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ce74-113">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3ce74-113">Mail.Read, Mail.ReadWrite</span></span>    | 
|<span data-ttu-id="3ce74-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3ce74-114">Application</span></span> | <span data-ttu-id="3ce74-115">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3ce74-115">Mail.Read, Mail.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="3ce74-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3ce74-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages/delta
GET /users/<id>/mailFolders/{id}/messages/delta
```

### <a name="query-parameters"></a><span data-ttu-id="3ce74-117">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="3ce74-117">Query parameters</span></span>

<span data-ttu-id="3ce74-p103">Beim Nachverfolgen von Änderungen in Nachrichten wird eine Runde von einem oder mehreren **delta**-Funktionsaufrufen ausgeführt. Wenn Sie Abfrageparameter (außer `$deltatoken` und `$skiptoken`) verwenden, müssen Sie sie in der ursprünglichen **delta**-Anforderung angeben. Microsoft Graph codiert automatisch alle angegebenen Parameter in den Tokenteil der in der Antwort enthaltenen `nextLink`- oder `deltaLink`-URL. Sie müssen alle gewünschten Abfrageparameter nur einmal im Vorfeld angeben. In nachfolgenden Anforderungen können Sie die `nextLink`- oder `deltaLink`-URL einfach aus der vorherigen Antwort kopieren und anwenden, da diese URL bereits die codierten gewünschten Parameter enthält.</span><span class="sxs-lookup"><span data-stu-id="3ce74-p103">Tracking changes in messages incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response. You only need to specify any desired query parameters once upfront. In subsequent requests, simply copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="3ce74-123">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="3ce74-123">Query parameter</span></span>      | <span data-ttu-id="3ce74-124">Typ</span><span class="sxs-lookup"><span data-stu-id="3ce74-124">Type</span></span>   |<span data-ttu-id="3ce74-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3ce74-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3ce74-126">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="3ce74-126">$deltatoken</span></span> | <span data-ttu-id="3ce74-127">string</span><span class="sxs-lookup"><span data-stu-id="3ce74-127">string</span></span> | <span data-ttu-id="3ce74-p104">Ein [Statustoken](../../../concepts/delta_query_overview.md), das in der `deltaLink`-URL des vorhergehenden **delta**-Funktionsaufrufs für dieselbe Nachrichtensammlung zurückgegeben wird und den Abschluss dieser Runde der Änderungsnachverfolgung anzeigt. Speichern Sie die gesamte `deltaLink`-URL einschließlich dieses Tokens, und wenden Sie sie in der ersten Anforderung der nächsten Änderungsnachverfolgungsrunde für diese Sammlung an.</span><span class="sxs-lookup"><span data-stu-id="3ce74-p104">A [state token](../../../concepts/delta_query_overview.md) returned in the `deltaLink` URL of the previous **delta** function call for the same message collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="3ce74-130">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="3ce74-130">$skiptoken</span></span> | <span data-ttu-id="3ce74-131">string</span><span class="sxs-lookup"><span data-stu-id="3ce74-131">string</span></span> | <span data-ttu-id="3ce74-132">Ein [Statustoken](../../../concepts/delta_query_overview.md), das in der `nextLink`-URL des vorhergehenden **delta**-Funktionsaufrufs zurückgegeben wird und anzeigt, dass in derselben Nachrichtensammlung weitere Änderungen zum Nachverfolgen vorliegen.</span><span class="sxs-lookup"><span data-stu-id="3ce74-132">A [state token](../../../concepts/delta_query_overview.md) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same message collection.</span></span> |


#### <a name="odata-query-parameters"></a><span data-ttu-id="3ce74-133">OData-Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="3ce74-133">OData query parameters</span></span>

- <span data-ttu-id="3ce74-p105">Sie können wie bei jeder GET-Anforderung den Abfrageparameter `$select` verwenden, um zwecks Leistungsoptimierung nur die benötigten Eigenschaften anzugeben. Die Eigenschaft _id_ wird immer zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3ce74-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 
- <span data-ttu-id="3ce74-136">Die Delta-Abfrage unterstützt `$select`, `$top` und `$expand` für Nachrichten.</span><span class="sxs-lookup"><span data-stu-id="3ce74-136">Delta query support `$select`, `$top`, and `$expand` for messages.</span></span> 
- <span data-ttu-id="3ce74-137">Es besteht eingeschränkte Unterstützung für `$filter` und `$orderby`:</span><span class="sxs-lookup"><span data-stu-id="3ce74-137">There is limited support for `$filter` and `$orderby`:</span></span>
  * <span data-ttu-id="3ce74-138">Es werden nur die `$filter`-Ausdrücke `$filter=receivedDateTime+ge+{value}` oder `$filter=receivedDateTime+gt+{value}` unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3ce74-138">The only supported `$filter` expresssions are `$filter=receivedDateTime+ge+{value}` or `$filter=receivedDateTime+gt+{value}`.</span></span>
  * <span data-ttu-id="3ce74-p106">Es wird nur der `$orderby`-Ausdruck `$orderby=receivedDateTime+desc` unterstützt. Wenn Sie keinen `$orderby`-Ausdruck einschließen, ist die Rückgabereihenfolge nicht gewährleistet.</span><span class="sxs-lookup"><span data-stu-id="3ce74-p106">The only supported `$orderby` expression is `$orderby=receivedDateTime+desc`. If you do not include an `$orderby` expression, the return order is not guaranteed.</span></span> 
- <span data-ttu-id="3ce74-141">`$search` wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3ce74-141">There is no support for `$search`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3ce74-142">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3ce74-142">Request headers</span></span>
| <span data-ttu-id="3ce74-143">Name</span><span class="sxs-lookup"><span data-stu-id="3ce74-143">Name</span></span>       | <span data-ttu-id="3ce74-144">Typ</span><span class="sxs-lookup"><span data-stu-id="3ce74-144">Type</span></span> | <span data-ttu-id="3ce74-145">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3ce74-145">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="3ce74-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ce74-146">Authorization</span></span>  | <span data-ttu-id="3ce74-147">string</span><span class="sxs-lookup"><span data-stu-id="3ce74-147">string</span></span>  | <span data-ttu-id="3ce74-p107">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3ce74-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3ce74-150">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3ce74-150">Content-Type</span></span>  | <span data-ttu-id="3ce74-151">string</span><span class="sxs-lookup"><span data-stu-id="3ce74-151">string</span></span>  | <span data-ttu-id="3ce74-p108">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="3ce74-p108">application/json. Required.</span></span> |
| <span data-ttu-id="3ce74-154">Prefer</span><span class="sxs-lookup"><span data-stu-id="3ce74-154">Prefer</span></span> | <span data-ttu-id="3ce74-155">string</span><span class="sxs-lookup"><span data-stu-id="3ce74-155">string</span></span>  | <span data-ttu-id="3ce74-p109">odata.maxpagesize={x}. Optional.</span><span class="sxs-lookup"><span data-stu-id="3ce74-p109">odata.maxpagesize={x}. Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="3ce74-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="3ce74-158">Response</span></span>

<span data-ttu-id="3ce74-159">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200, OK` und das [message](../resources/message.md)-Sammlungsobjekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3ce74-159">If successful, this method returns a `200, OK` response code and [message](../resources/message.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ce74-160">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3ce74-160">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3ce74-161">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3ce74-161">Request</span></span>
<span data-ttu-id="3ce74-162">Das folgende Beispiel zeigt, wie Sie einen einzelnen **delta**-Funktionsaufruf ausführen und die maximale Anzahl von Nachrichten im Textkörper der Antwort auf 2 beschränken.</span><span class="sxs-lookup"><span data-stu-id="3ce74-162">The following example shows how to make a single **delta** function call, and limit the maximum number of messages in the response body to 2.</span></span>

<span data-ttu-id="3ce74-p110">Zum Nachverfolgen von Änderungen in den Nachrichten eines Ordners führen Sie einen oder mehrere **delta**-Funktionsaufrufe aus, um den Satz der inkrementellen Änderungen seit der letzten Delta-Abfrage abzurufen. Ein Beispiel für eine Runde von Delta-Abfrageaufrufen finden Sie unter [Inkrementelle Änderungen an Nachrichten in einem Ordner abrufen](../../../concepts/delta_query_messages.md).</span><span class="sxs-lookup"><span data-stu-id="3ce74-p110">To track changes in the messages in a folder, you would make one or more **delta** function calls to get the set of incremental changes since the last delta query. For an example that shows a round of delta query calls, see [Get incremental changes to messages in a folder](../../../concepts/delta_query_messages.md).</span></span>
 
<!-- {
  "blockType": "request",
  "name": "message_delta"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/messages/delta

Prefer: odata.maxpagesize=2
```

##### <a name="response"></a><span data-ttu-id="3ce74-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="3ce74-165">Response</span></span>
<span data-ttu-id="3ce74-166">Wenn die Anforderung erfolgreich ist, enthält die Antwort ein Statustoken, entweder ein _skipToken_</span><span class="sxs-lookup"><span data-stu-id="3ce74-166">If the request is successful, the response would include a state token, which is either a _skipToken_</span></span>  
<span data-ttu-id="3ce74-p111">(in einem _@odata.nextLink_-Antwortheader) oder ein _deltaToken_ (in einem _@odata.deltaLink_-Antwortheader). Diese geben an, ob Sie mit der Runde fortfahren sollten oder ob alle Änderungen für diese Runde abgerufen wurden.</span><span class="sxs-lookup"><span data-stu-id="3ce74-p111">(in an _@odata.nextLink_ response header) or a _deltaToken_ (in an _@odata.deltaLink_ response header). Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="3ce74-169">Die Antwort unten zeigt ein _skipToken_ in einem _@odata.nextLink_-Antwortheader.</span><span class="sxs-lookup"><span data-stu-id="3ce74-169">The response below shows a _skipToken_ in an _@odata.nextLink_ response header.</span></span>

<span data-ttu-id="3ce74-p112">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3ce74-p112">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 337

{
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/me/mailfolders('{id}')/messages/delta?$skiptoken={_skipToken_}",
  "value": [
    {
      "receivedDateTime": "datetime-value",
      "sentDateTime": "datetime-value",
      "hasAttachments": true,
      "internetMessageId": "internetMessageId-value",
      "subject": "subject-value",
      "body": {
        "contentType": "contentType-value",
        "content": "content-value"
      }
    }
  ]
}
```

### <a name="see-also"></a><span data-ttu-id="3ce74-172">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="3ce74-172">See also</span></span>

- [<span data-ttu-id="3ce74-173">Verwenden einer Delta-Abfrage zum Nachverfolgen von Änderungen in Microsoft Graph-Daten</span><span class="sxs-lookup"><span data-stu-id="3ce74-173">Use delta query to track changes in Microsoft Graph data</span></span>](../../../concepts/delta_query_overview.md)
- [<span data-ttu-id="3ce74-174">Inkrementelle Änderungen an Nachrichten in einem Ordner abrufen</span><span class="sxs-lookup"><span data-stu-id="3ce74-174">Get incremental changes to messages in a folder</span></span>](../../../concepts/delta_query_messages.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->