# <a name="contact-delta"></a><span data-ttu-id="e83df-101">contact: delta</span><span class="sxs-lookup"><span data-stu-id="e83df-101">contact: delta</span></span>

<span data-ttu-id="e83df-102">Dient zum Abrufen eines Satzes von Kontakten, die einem bestimmten Ordner hinzugefügt bzw. daraus gelöscht oder darin aktualisiert wurden.</span><span class="sxs-lookup"><span data-stu-id="e83df-102">Get a set of contacts that have been added, deleted, or updated in a specified folder.</span></span>

<span data-ttu-id="e83df-p101">Ein **delta**-Funktionsaufruf für Kontakte in einem Ordner ähnelt einer GET-Anforderung, mit der Ausnahme, dass durch entsprechende Anwendung von [Statustoken](../../../concepts/delta_query_overview.md) in einem oder mehreren dieser Aufrufe inkrementelle Änderungen an den Kontakten im betreffenden Ordner abgefragt werden können. Dies ermöglicht es Ihnen, einen lokalen Speicher der Kontakte eines Benutzers zu pflegen und zu synchronisieren, ohne dass Sie jedes Mal den gesamten Satz Kontakte vom Server abrufen müssen.</span><span class="sxs-lookup"><span data-stu-id="e83df-p101">A **delta** function call for contacts in a folder is similar to a GET request, except that by appropriately applying [state tokens](../../../concepts/delta_query_overview.md) in one or more of these calls, you can query for incremental changes in the contacts in that folder. This allows you to maintain and synchronize a local store of a user's contacts without having to fetch the entire set of contacts from the server every time.</span></span>  

## <a name="permissions"></a><span data-ttu-id="e83df-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e83df-105">Permissions</span></span>
<span data-ttu-id="e83df-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e83df-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e83df-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e83df-108">Permission type</span></span>      | <span data-ttu-id="e83df-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e83df-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e83df-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e83df-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e83df-111">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e83df-111">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="e83df-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e83df-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e83df-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e83df-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="e83df-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e83df-114">Application</span></span> | <span data-ttu-id="e83df-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e83df-115">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e83df-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e83df-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}/contacts/delta
GET /users/<id>/contactFolders/{id}/contacts/delta
```

### <a name="query-parameters"></a><span data-ttu-id="e83df-117">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e83df-117">Query parameters</span></span>

<span data-ttu-id="e83df-p103">Beim Nachverfolgen von Änderungen an Kontakten wird eine Runde von einem oder mehreren **delta**-Funktionsaufrufen ausgeführt. Wenn Sie Abfrageparameter (außer `$deltatoken` und `$skiptoken`) verwenden, müssen Sie sie in der ursprünglichen **delta**-Anforderung angeben. Microsoft Graph codiert automatisch alle angegebenen Parameter in den Tokenteil der in der Antwort enthaltenen `nextLink`- oder `deltaLink`-URL. Sie müssen alle gewünschten Abfrageparameter nur einmal im Vorfeld angeben. In nachfolgenden Anforderungen können Sie die `nextLink`- oder `deltaLink`-URL einfach aus der vorherigen Antwort kopieren und anwenden, da diese URL bereits die codierten gewünschten Parameter enthält.</span><span class="sxs-lookup"><span data-stu-id="e83df-p103">Tracking changes in contacts incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response. You only need to specify any desired query parameters once upfront. In subsequent requests, simply copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="e83df-123">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e83df-123">Query parameter</span></span>      | <span data-ttu-id="e83df-124">Typ</span><span class="sxs-lookup"><span data-stu-id="e83df-124">Type</span></span>   |<span data-ttu-id="e83df-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e83df-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e83df-126">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="e83df-126">$deltatoken</span></span> | <span data-ttu-id="e83df-127">string</span><span class="sxs-lookup"><span data-stu-id="e83df-127">string</span></span> | <span data-ttu-id="e83df-p104">Ein [Statustoken](../../../concepts/delta_query_overview.md), das in der `deltaLink`-URL des vorhergehenden **delta**-Funktionsaufrufs für dieselbe Kontaktsammlung zurückgegeben wird und den Abschluss dieser Runde der Änderungsnachverfolgung anzeigt. Speichern Sie die gesamte `deltaLink`-URL einschließlich dieses Tokens, und wenden Sie sie in der ersten Anforderung der nächsten Änderungsnachverfolgungsrunde für diese Sammlung an.</span><span class="sxs-lookup"><span data-stu-id="e83df-p104">A [state token](../../../concepts/delta_query_overview.md) returned in the `deltaLink` URL of the previous **delta** function call for the same contact collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="e83df-130">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="e83df-130">$skiptoken</span></span> | <span data-ttu-id="e83df-131">string</span><span class="sxs-lookup"><span data-stu-id="e83df-131">string</span></span> | <span data-ttu-id="e83df-132">Ein [Statustoken](../../../concepts/delta_query_overview.md), das in der `nextLink`-URL des vorhergehenden **delta**-Funktionsaufrufs zurückgegeben wird und anzeigt, dass in derselben Kontaktsammlung weitere Änderungen zum Nachverfolgen vorliegen.</span><span class="sxs-lookup"><span data-stu-id="e83df-132">A [state token](../../../concepts/delta_query_overview.md) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same contact collection.</span></span> |

#### <a name="odata-query-parameters"></a><span data-ttu-id="e83df-133">OData-Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e83df-133">OData query parameters</span></span>

- <span data-ttu-id="e83df-p105">Sie können wie bei jeder GET-Anforderung den Abfrageparameter `$select` verwenden, um zwecks Leistungsoptimierung nur die benötigten Eigenschaften anzugeben. Die Eigenschaft _id_ wird immer zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e83df-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 


## <a name="request-headers"></a><span data-ttu-id="e83df-136">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e83df-136">Request headers</span></span>
| <span data-ttu-id="e83df-137">Name</span><span class="sxs-lookup"><span data-stu-id="e83df-137">Name</span></span>       | <span data-ttu-id="e83df-138">Typ</span><span class="sxs-lookup"><span data-stu-id="e83df-138">Type</span></span> | <span data-ttu-id="e83df-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e83df-139">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="e83df-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="e83df-140">Authorization</span></span>  | <span data-ttu-id="e83df-141">string</span><span class="sxs-lookup"><span data-stu-id="e83df-141">string</span></span>  | <span data-ttu-id="e83df-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e83df-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e83df-144">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e83df-144">Content-Type</span></span>  | <span data-ttu-id="e83df-145">string</span><span class="sxs-lookup"><span data-stu-id="e83df-145">string</span></span>  | <span data-ttu-id="e83df-p107">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="e83df-p107">application/json. Required.</span></span> |
| <span data-ttu-id="e83df-148">Prefer</span><span class="sxs-lookup"><span data-stu-id="e83df-148">Prefer</span></span> | <span data-ttu-id="e83df-149">string</span><span class="sxs-lookup"><span data-stu-id="e83df-149">string</span></span>  | <span data-ttu-id="e83df-p108">odata.maxpagesize={x}. Optional.</span><span class="sxs-lookup"><span data-stu-id="e83df-p108">odata.maxpagesize={x}. Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="e83df-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="e83df-152">Response</span></span>

<span data-ttu-id="e83df-153">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [contact](../resources/contact.md)-Sammlungsobjekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e83df-153">If successful, this method returns a `200 OK` response code and [contact](../resources/contact.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e83df-154">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e83df-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e83df-155">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e83df-155">Request</span></span>
<span data-ttu-id="e83df-156">Das folgende Beispiel zeigt, wie Sie einen einzelnen **delta**-Funktionsaufruf ausführen, den `$select`-Parameter verwenden, um nur die Eigenschaft **displayName** jedes Kontakts abzurufen, und die maximale Anzahl von Kontakten im Antworttext auf 2 beschränken.</span><span class="sxs-lookup"><span data-stu-id="e83df-156">The following example shows how to make a single **delta** function call, use the `$select` parameter to get only each contact's **displayName** property, and limit the maximum number of contacts in the response body to 2.</span></span>

<span data-ttu-id="e83df-157">Zum Nachverfolgen von Änderungen an den Kontakten in einem Ordner führen Sie einen oder mehrere **delta**-Funktionsaufrufe mit entsprechenden Statustoken aus, um den Satz der inkrementellen Änderungen seit der letzten Delta-Abfrage abzurufen.</span><span class="sxs-lookup"><span data-stu-id="e83df-157">To track changes in the contacts in a folder, you would make one or more **delta** function calls, with appropriate state tokens, to get the set of incremental changes since the last delta query.</span></span> 

<span data-ttu-id="e83df-p109">Ein ähnliches Beispiel zeigt, wie die Statustoken zum Nachverfolgen von Änderungen in den Nachrichten eines E-Mail-Ordners verwendet werden: [Inkrementelle Änderungen an Nachrichten in einem Ordner abrufen](../../../concepts/delta_query_messages.md) Die wichtigsten Unterschiede zwischen dem Nachverfolgen von Kontakten und dem Nachverfolgen von Nachrichten in einem Ordner liegen in den Anforderungs-URLs der Delta-Abfrage vor; außerdem geben die Abfrageantworten **contact**- anstelle von **message**-Sammlungen zurück.</span><span class="sxs-lookup"><span data-stu-id="e83df-p109">You can find a similar example that shows how to use the state tokens to track changes in the messages of a mail folder: [Get incremental changes to messages in a folder](../../../concepts/delta_query_messages.md). The main differences between tracking contacts and tracking messages in a folder are in the delta query request URLs, and the query responses returning **contact** rather than **message** collections.</span></span>
 
<!-- {
  "blockType": "request",
  "name": "contact_delta"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contactFolders/{id}/contacts/delta?$select=displayName

Prefer: odata.maxpagesize=2
```

##### <a name="response"></a><span data-ttu-id="e83df-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="e83df-160">Response</span></span>
<span data-ttu-id="e83df-161">Wenn die Anforderung erfolgreich ist, enthält die Antwort ein Statustoken, entweder ein _skipToken_</span><span class="sxs-lookup"><span data-stu-id="e83df-161">If the request is successful, the response would include a state token, which is either a _skipToken_</span></span>  
<span data-ttu-id="e83df-p110">(in einem _@odata.nextLink_-Antwortheader) oder ein _deltaToken_ (in einem _@odata.deltaLink_-Antwortheader). Diese geben an, ob Sie mit der Runde fortfahren sollten oder ob alle Änderungen für diese Runde abgerufen wurden.</span><span class="sxs-lookup"><span data-stu-id="e83df-p110">(in an _@odata.nextLink_ response header) or a _deltaToken_ (in an _@odata.deltaLink_ response header). Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="e83df-164">Die Antwort unten zeigt ein _skipToken_ in einem _@odata.nextLink_-Antwortheader.</span><span class="sxs-lookup"><span data-stu-id="e83df-164">The response below shows a _skipToken_ in an _@odata.nextLink_ response header.</span></span>

<span data-ttu-id="e83df-p111">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e83df-p111">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 337

{
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/me/contactfolders('{id}')/contacts/delta?$skiptoken={_skipToken_}",
  "value": [
    {
      "parentFolderId": "parentFolderId-value",
      "birthday": "2016-10-19T10:37:00Z",
      "fileAs": "fileAs-value",
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "initials": "initials-value"
    }
  ]
}
```

### <a name="see-also"></a><span data-ttu-id="e83df-167">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="e83df-167">See also</span></span>

- [<span data-ttu-id="e83df-168">Verwenden einer Delta-Abfrage zum Nachverfolgen von Änderungen in Microsoft Graph-Daten</span><span class="sxs-lookup"><span data-stu-id="e83df-168">Use delta query to track changes in Microsoft Graph data</span></span>](../../../concepts/delta_query_overview.md)
- [<span data-ttu-id="e83df-169">Inkrementelle Änderungen an Nachrichten in einem Ordner abrufen</span><span class="sxs-lookup"><span data-stu-id="e83df-169">Get incremental changes to messages in a folder</span></span>](../../../concepts/delta_query_messages.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contact: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->