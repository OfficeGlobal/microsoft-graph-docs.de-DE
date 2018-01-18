# <a name="group-delta"></a><span data-ttu-id="f25a9-101">group: delta</span><span class="sxs-lookup"><span data-stu-id="f25a9-101">group: delta</span></span>
<span data-ttu-id="f25a9-p101">Mit einer [Delta-Abfrage](../../../concepts/delta_query_overview.md) können Anwendungen neu erstellte, aktualisierte oder gelöschte Entitäten ermitteln, ohne die Zielressource bei jeder Anforderung vollständig lesen zu müssen. Um Änderungen an Gruppen zu ermitteln, führen Sie eine Anforderung unter Verwendung der *delta*-Funktion aus. Weitere Informationen finden Sie unter [Verwenden einer Delta-Abfrage](../../../concepts/delta_query_overview.md).</span><span class="sxs-lookup"><span data-stu-id="f25a9-p101">[Delta query](../../../concepts/delta_query_overview.md) enables applications to discover newly created, updated, or deleted entities without performing a full read of the target resource with every request. To discover changes to groups, perform a request using the *delta* function. See [Using Delta Query](../../../concepts/delta_query_overview.md) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="f25a9-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f25a9-105">Permissions</span></span>
<span data-ttu-id="f25a9-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f25a9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f25a9-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f25a9-108">Permission type</span></span>      | <span data-ttu-id="f25a9-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f25a9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f25a9-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f25a9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f25a9-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f25a9-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f25a9-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f25a9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f25a9-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f25a9-113">Not supported.</span></span>    |
|<span data-ttu-id="f25a9-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f25a9-114">Application</span></span> | <span data-ttu-id="f25a9-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f25a9-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f25a9-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f25a9-116">HTTP request</span></span>
<span data-ttu-id="f25a9-117">Um Änderungen nachzuverfolgen, führe Sie zunächst eine Anforderung einschließlich der delta-Funktion für die Gruppenressource aus.</span><span class="sxs-lookup"><span data-stu-id="f25a9-117">To begin tracking changes, you make a request including the delta function on the groups resource.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /groups/delta
```

### <a name="query-parameters"></a><span data-ttu-id="f25a9-118">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f25a9-118">Query parameters</span></span>
<span data-ttu-id="f25a9-p103">Beim Nachverfolgen von Änderungen in Gruppen wird eine Runde von einem oder mehreren **delta**-Funktionsaufrufen ausgeführt. Wenn Sie Abfrageparameter (außer `$deltatoken` und `$skiptoken`) verwenden, müssen Sie sie in der ursprünglichen **delta**-Anforderung angeben. Microsoft Graph codiert automatisch alle angegebenen Parameter in den Tokenteil der in der Antwort enthaltenen `nextLink`- oder `deltaLink`-URL.</span><span class="sxs-lookup"><span data-stu-id="f25a9-p103">Tracking changes in groups incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response. You only need to specify any desired query parameters once upfront. In subsequent requests, copy and apply the  or  URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

<span data-ttu-id="f25a9-122">Sie müssen alle gewünschten Abfrageparameter nur einmal im Vorfeld angeben.</span><span class="sxs-lookup"><span data-stu-id="f25a9-122">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="f25a9-123">In nachfolgenden Anforderungen können Sie die  `nextLink`- oder `deltaLink`-URL aus der vorherigen Antwort kopieren und anwenden, da diese URL bereits die codierten gewünschten Parameter enthält.</span><span class="sxs-lookup"><span data-stu-id="f25a9-123">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="f25a9-124">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f25a9-124">Query parameter</span></span>      | <span data-ttu-id="f25a9-125">Typ</span><span class="sxs-lookup"><span data-stu-id="f25a9-125">Type</span></span>   |<span data-ttu-id="f25a9-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f25a9-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f25a9-127">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="f25a9-127">$deltatoken</span></span> | <span data-ttu-id="f25a9-128">string</span><span class="sxs-lookup"><span data-stu-id="f25a9-128">string</span></span> | <span data-ttu-id="f25a9-p104">Ein [Statustoken](../../../concepts/delta_query_overview.md), das in der `deltaLink`-URL des vorhergehenden **delta**-Funktionsaufrufs für dieselbe Gruppensammlung zurückgegeben wird und den Abschluss dieser Runde der Änderungsnachverfolgung anzeigt. Speichern Sie die gesamte `deltaLink`-URL einschließlich dieses Tokens, und wenden Sie sie in der ersten Anforderung der nächsten Änderungsnachverfolgungsrunde für diese Sammlung an.</span><span class="sxs-lookup"><span data-stu-id="f25a9-p104">A [state token](../../../concepts/delta_query_overview.md) returned in the `deltaLink` URL of the previous **delta** function call for the same group collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="f25a9-131">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="f25a9-131">$skiptoken</span></span> | <span data-ttu-id="f25a9-132">string</span><span class="sxs-lookup"><span data-stu-id="f25a9-132">string</span></span> | <span data-ttu-id="f25a9-133">Ein [Statustoken](../../../concepts/delta_query_overview.md), das in der `nextLink`-URL des vorhergehenden **delta**-Funktionsaufrufs zurückgegeben wird und anzeigt, dass in derselben Gruppensammlung weitere Änderungen zum Nachverfolgen vorliegen.</span><span class="sxs-lookup"><span data-stu-id="f25a9-133">A [state token](../../../concepts/delta_query_overview.md) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same group collection.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="f25a9-134">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f25a9-134">Optional query parameters</span></span>
<span data-ttu-id="f25a9-135">Diese Methode unterstützt OData-Abfrageparameter zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f25a9-135">This method supports OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="f25a9-p105">Sie können wie bei jeder GET-Anforderung den Abfrageparameter `$select` verwenden, um zwecks Leistungsoptimierung nur die benötigten Eigenschaften anzugeben. Die Eigenschaft _id_ wird immer zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f25a9-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 
- <span data-ttu-id="f25a9-138">Die Delta-Abfrage unterstützt `$select`, `$top` und `$expand` für Gruppen.</span><span class="sxs-lookup"><span data-stu-id="f25a9-138">Delta query support `$select`, `$top`, and `$expand` for groups.</span></span> 
- <span data-ttu-id="f25a9-p106">Es besteht eingeschränkte Unterstützung für `$orderby`: Der einzige unterstützte `$orderby`-Ausdruck ist `$orderby=receivedDateTime+desc`. Wenn Sie keinen `$orderby`-Ausdruck einschließen, ist die Rückgabereihenfolge nicht gewährleistet.</span><span class="sxs-lookup"><span data-stu-id="f25a9-p106">There is limited support for `$orderby`: The only supported `$orderby` expression is `$orderby=receivedDateTime+desc`. If you do not include an `$orderby` expression, the return order is not guaranteed.</span></span> 
- <span data-ttu-id="f25a9-141">`$search` wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f25a9-141">There is no support for `$search`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f25a9-142">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f25a9-142">Request headers</span></span>
| <span data-ttu-id="f25a9-143">Name</span><span class="sxs-lookup"><span data-stu-id="f25a9-143">Name</span></span>       | <span data-ttu-id="f25a9-144">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f25a9-144">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f25a9-145">Authorization</span><span class="sxs-lookup"><span data-stu-id="f25a9-145">Authorization</span></span>  | <span data-ttu-id="f25a9-146">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="f25a9-146">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="f25a9-147">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f25a9-147">Content-Type</span></span>  | <span data-ttu-id="f25a9-148">application/json</span><span class="sxs-lookup"><span data-stu-id="f25a9-148">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="f25a9-149">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f25a9-149">Request body</span></span>
<span data-ttu-id="f25a9-150">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f25a9-150">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f25a9-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="f25a9-151">Response</span></span>
<span data-ttu-id="f25a9-p107">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [group](../resources/group.md)-Sammlungsobjekt im Antworttext zurückgegeben. Die Antwort enthält zudem ein Statustoken, entweder eine nextLink- oder eine deltaLink-URL.</span><span class="sxs-lookup"><span data-stu-id="f25a9-p107">If successful, this method returns `200 OK` response code and [group](../resources/group.md) collection object in the response body. The response also includes a state token which is either a nextLink URL or a deltaLink URL.</span></span>

- <span data-ttu-id="f25a9-p108">Wenn eine nextLink-URL zurückgegeben wird, gibt es zusätzliche Seiten mit Daten, die in der Sitzung abgerufen werden müssen. Die Anwendung nimmt weiterhin Anforderungen über die nextLink-URL vor, bis eine deltaLink-URL in der Antwort zurückgegeben wird.</span><span class="sxs-lookup"><span data-stu-id="f25a9-p108">If a nextLink URL is returned, there are additional pages of data to be retrieved in the session. The application continues making requests using the nextLink URL until a deltaLink URL is included in the response.</span></span>

- <span data-ttu-id="f25a9-p109">Wenn eine deltaLink-URL zurückgegeben wird, gibt es keine weiteren Daten über den derzeitigen Status der zurückzugebenen Ressource. Für zukünftige Anforderungen verwendet die Anwendung die deltaLink-URL, um Informationen zu Änderungen an der Ressource zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="f25a9-p109">If a deltaLink URL is returned, there is no more data about the existing state of the resource to be returned. For future requests, the application uses the deltaLink URL to learn about changes to the resource.</span></span>

<span data-ttu-id="f25a9-158">Siehe:</span><span class="sxs-lookup"><span data-stu-id="f25a9-158">See:</span></span></br>
- <span data-ttu-id="f25a9-159">Weitere Informationen finden Sie unter [Verwenden einer Delta-Abfrage](../../../concepts/delta_query_overview.md).</span><span class="sxs-lookup"><span data-stu-id="f25a9-159">[Using Delta Query](../../../concepts/delta_query_overview.md) for more details</span></span></br>
- <span data-ttu-id="f25a9-160">Beispielanforderungen finden Sie unter [Inkrementelle Änderungen für Gruppen abrufen](../../../concepts/delta_query_groups.md).</span><span class="sxs-lookup"><span data-stu-id="f25a9-160">[Get incremental changes for groups](../../../concepts/delta_query_groups.md) for an example requests.</span></span></br>
    
## <a name="example"></a><span data-ttu-id="f25a9-161">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f25a9-161">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f25a9-162">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f25a9-162">Request</span></span>
<span data-ttu-id="f25a9-163">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f25a9-163">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/delta
```

#### <a name="response"></a><span data-ttu-id="f25a9-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="f25a9-164">Response</span></span>
<span data-ttu-id="f25a9-165">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f25a9-165">The following is an example of the response.</span></span>
><span data-ttu-id="f25a9-166">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="f25a9-166">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f25a9-167">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="f25a9-167">All the properties will be returned from an actual call.</span></span>

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
      "mail": "mail-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->