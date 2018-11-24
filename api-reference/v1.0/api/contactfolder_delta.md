# <a name="contactfolder-delta"></a><span data-ttu-id="cd86a-101">contactFolder: delta</span><span class="sxs-lookup"><span data-stu-id="cd86a-101">contactFolder: delta</span></span>

<span data-ttu-id="cd86a-102">Dient zum Abrufen eines Satzes von Kontaktordnern, die dem Postfach des Benutzers hinzugefügt bzw. daraus gelöscht oder entfernt wurden.</span><span class="sxs-lookup"><span data-stu-id="cd86a-102">Get a set of contact folders that have been added, deleted, or removed from the user's mailbox.</span></span>

<span data-ttu-id="cd86a-p101">Ein **delta**-Funktionsaufruf für Kontaktordner in einem Postfach ähnelt einer GET-Anforderung, mit der Ausnahme, dass durch entsprechende Anwendung von [Statustoken](../../../concepts/delta_query_overview.md) in einem oder mehreren dieser Aufrufe inkrementelle Änderungen in den Kontaktordnern abgefragt werden können. Dies ermöglicht es Ihnen, einen lokalen Speicher der Kontaktordner eines Benutzers zu pflegen und zu synchronisieren, ohne dass Sie jedes Mal alle Kontaktordner des betreffenden Postfachs vom Server abrufen müssen.</span><span class="sxs-lookup"><span data-stu-id="cd86a-p101">A **delta** function call for contact folders in a mailbox is similar to a GET request, except that by appropriately applying [state tokens](../../../concepts/delta_query_overview.md) in one or more of these calls, you can query for incremental changes in the contact folders. This allows you to maintain and synchronize a local store of a user's contact folders without having to fetch all the contact folders of that mailbox from the server every time.</span></span>

## <a name="permissions"></a><span data-ttu-id="cd86a-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="cd86a-105">Permissions</span></span>
<span data-ttu-id="cd86a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="cd86a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="cd86a-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cd86a-108">Permission type</span></span>      | <span data-ttu-id="cd86a-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cd86a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cd86a-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cd86a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cd86a-111">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cd86a-111">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="cd86a-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cd86a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd86a-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cd86a-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="cd86a-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cd86a-114">Application</span></span> | <span data-ttu-id="cd86a-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cd86a-115">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="cd86a-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cd86a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/delta
GET /users/{id}/contactFolders/delta
```

## <a name="query-parameters"></a><span data-ttu-id="cd86a-117">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="cd86a-117">Query parameters</span></span>

<span data-ttu-id="cd86a-p103">Beim Nachverfolgen von Änderungen in Kontaktordnern wird eine Runde von einem oder mehreren **delta**-Funktionsaufrufen ausgeführt. Wenn Sie Abfrageparameter (außer `$deltatoken` und `$skiptoken`) verwenden, müssen Sie sie in der ursprünglichen **delta**-Anforderung angeben. Microsoft Graph codiert automatisch alle angegebenen Parameter in den Tokenteil (`skiptoken` oder `$deltatoken`) der in der Antwort enthaltenen `nextLink`- oder `deltaLink`-URL. Sie müssen alle gewünschten Abfrageparameter nur einmal im Vorfeld angeben. In nachfolgenden Anforderungen können Sie die `nextLink`- oder `deltaLink`-URL einfach aus der vorherigen Antwort kopieren und anwenden, da diese URL bereits die codierten gewünschten Parameter enthält.</span><span class="sxs-lookup"><span data-stu-id="cd86a-p103">Tracking changes in contact folders incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion (`skiptoken` or `$deltatoken`) of the `nextLink` or `deltaLink` URL provided in the response. You only need to specify any desired query parameters once upfront. In subsequent requests, simply copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="cd86a-123">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="cd86a-123">Query parameter</span></span>      | <span data-ttu-id="cd86a-124">Typ</span><span class="sxs-lookup"><span data-stu-id="cd86a-124">Type</span></span>   |<span data-ttu-id="cd86a-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cd86a-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cd86a-126">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="cd86a-126">$deltatoken</span></span> | <span data-ttu-id="cd86a-127">string</span><span class="sxs-lookup"><span data-stu-id="cd86a-127">string</span></span> | <span data-ttu-id="cd86a-p104">Ein [Statustoken](../../../concepts/delta_query_overview.md), das in der `deltaLink`-URL des vorhergehenden **delta**-Funktionsaufrufs für dieselbe Sammlung von Kontaktordnern zurückgegeben wird und den Abschluss dieser Runde der Änderungsnachverfolgung anzeigt. Speichern Sie die gesamte `deltaLink`-URL einschließlich dieses Tokens, und wenden Sie sie in der ersten Anforderung der nächsten Änderungsnachverfolgungsrunde für diese Sammlung an.</span><span class="sxs-lookup"><span data-stu-id="cd86a-p104">A [state token](../../../concepts/delta_query_overview.md) returned in the `deltaLink` URL of the previous **delta** function call for the same contact folder collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="cd86a-130">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="cd86a-130">$skiptoken</span></span> | <span data-ttu-id="cd86a-131">string</span><span class="sxs-lookup"><span data-stu-id="cd86a-131">string</span></span> | <span data-ttu-id="cd86a-132">Ein [Statustoken](../../../concepts/delta_query_overview.md), das in der `nextLink`-URL des vorhergehenden **delta**-Funktionsaufrufs zurückgegeben wird und anzeigt, dass in derselben Sammlung von Kontaktordnern weitere Änderungen zum Nachverfolgen vorliegen.</span><span class="sxs-lookup"><span data-stu-id="cd86a-132">A [state token](../../../concepts/delta_query_overview.md) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same contact folder collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="cd86a-133">OData-Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="cd86a-133">OData query parameters</span></span>

<span data-ttu-id="cd86a-p105">Sie können wie bei jeder GET-Anforderung den Abfrageparameter `$select` verwenden, um zwecks Leistungsoptimierung nur die benötigten Eigenschaften anzugeben. Die Eigenschaft _id_ wird immer zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cd86a-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="cd86a-136">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cd86a-136">Request headers</span></span>
| <span data-ttu-id="cd86a-137">Name</span><span class="sxs-lookup"><span data-stu-id="cd86a-137">Name</span></span>       | <span data-ttu-id="cd86a-138">Typ</span><span class="sxs-lookup"><span data-stu-id="cd86a-138">Type</span></span> | <span data-ttu-id="cd86a-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cd86a-139">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="cd86a-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd86a-140">Authorization</span></span>  | <span data-ttu-id="cd86a-141">string</span><span class="sxs-lookup"><span data-stu-id="cd86a-141">string</span></span>  | <span data-ttu-id="cd86a-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cd86a-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cd86a-144">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cd86a-144">Content-Type</span></span>  | <span data-ttu-id="cd86a-145">string</span><span class="sxs-lookup"><span data-stu-id="cd86a-145">string</span></span>  | <span data-ttu-id="cd86a-p107">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="cd86a-p107">application/json. Required.</span></span> |
| <span data-ttu-id="cd86a-148">Prefer</span><span class="sxs-lookup"><span data-stu-id="cd86a-148">Prefer</span></span> | <span data-ttu-id="cd86a-149">string</span><span class="sxs-lookup"><span data-stu-id="cd86a-149">string</span></span>  | <span data-ttu-id="cd86a-p108">odata.maxpagesize={x}. Optional.</span><span class="sxs-lookup"><span data-stu-id="cd86a-p108">odata.maxpagesize={x}. Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="cd86a-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="cd86a-152">Response</span></span>

<span data-ttu-id="cd86a-153">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [contactFolder](../resources/contactfolder.md)-Sammlungsobjekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cd86a-153">If successful, this method returns a `200 OK` response code and [contactFolder](../resources/contactfolder.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd86a-154">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cd86a-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cd86a-155">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cd86a-155">Request</span></span>
<span data-ttu-id="cd86a-156">Das folgende Beispiel zeigt, wie Sie einen einzelnen **delta**-Funktionsaufruf ausführen und die maximale Anzahl von Kontaktordnern im Antworttext auf 2 beschränken.</span><span class="sxs-lookup"><span data-stu-id="cd86a-156">The following example shows how to make a single **delta** function call, and limit the maximum number of contact folders in the response body to 2.</span></span>

<span data-ttu-id="cd86a-157">Zum Nachverfolgen von Änderungen in den Kontaktordnern eines Postfachs führen Sie einen oder mehrere **delta**-Funktionsaufrufe mit entsprechenden Statustoken aus, um den Satz der inkrementellen Änderungen seit der letzten Delta-Abfrage abzurufen.</span><span class="sxs-lookup"><span data-stu-id="cd86a-157">To track changes in the contact folders of a mailbox, you would make one or more **delta** function calls, with appropriate state tokens, to get the set of incremental changes since the last delta query.</span></span> 

<span data-ttu-id="cd86a-p109">Ein ähnliches Beispiel zeigt, wie die Statustoken zum Nachverfolgen von Änderungen in den Nachrichten eines E-Mail-Ordners verwendet werden: [Inkrementelle Änderungen an Nachrichten in einem Ordner abrufen](../../../concepts/delta_query_messages.md) Die wichtigsten Unterschiede zwischen dem Nachverfolgen von Kontaktordnern und dem Nachverfolgen von Nachrichten in einem Ordner liegen in den Anforderungs-URLs der Delta-Abfrage vor; außerdem geben die Abfrageantworten **contactFolder**- anstelle von **message**-Sammlungen zurück.</span><span class="sxs-lookup"><span data-stu-id="cd86a-p109">You can find a similar example that shows how to use the state tokens to track changes in the messages of a mail folder: [Get incremental changes to messages in a folder](../../../concepts/delta_query_messages.md). The main differences between tracking contact folders and tracking messages in a folder are in the delta query request URLs, and the query responses returning **contactFolder** rather than **message** collections.</span></span>

<!-- {
  "blockType": "request",
  "name": "contactfolder_delta"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contactFolders/delta
Prefer: odata.maxpagesize=2
```

##### <a name="response"></a><span data-ttu-id="cd86a-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="cd86a-160">Response</span></span>

<span data-ttu-id="cd86a-161">Wenn die Anforderung erfolgreich ist, enthält die Antwort ein Statustoken, entweder ein _skipToken_</span><span class="sxs-lookup"><span data-stu-id="cd86a-161">If the request is successful, the response would include a state token, which is either a _skipToken_</span></span>  
<span data-ttu-id="cd86a-p110">(in einem _@odata.nextLink_-Antwortheader) oder ein _deltaToken_ (in einem _@odata.deltaLink_-Antwortheader). Diese geben an, ob Sie mit der Runde fortfahren sollten oder ob alle Änderungen für diese Runde abgerufen wurden.</span><span class="sxs-lookup"><span data-stu-id="cd86a-p110">(in an _@odata.nextLink_ response header) or a _deltaToken_ (in an _@odata.deltaLink_ response header). Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="cd86a-164">Die Antwort unten zeigt ein _skipToken_ in einem _@odata.nextLink_-Antwortheader.</span><span class="sxs-lookup"><span data-stu-id="cd86a-164">The response below shows a _skipToken_ in an _@odata.nextLink_ response header.</span></span>

<span data-ttu-id="cd86a-p111">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cd86a-p111">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 254

{
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/me/contactfolders/delta?$skiptoken={_skipToken_}",
  "value": [
    {
     "parentFolderId": "parentFolderId-value",
      "displayName": "displayName-value",
      "id": "id-value"
    }
  ]
}
```

### <a name="see-also"></a><span data-ttu-id="cd86a-167">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="cd86a-167">See also</span></span>

- [<span data-ttu-id="cd86a-168">Verwenden einer Delta-Abfrage zum Nachverfolgen von Änderungen in Microsoft Graph-Daten</span><span class="sxs-lookup"><span data-stu-id="cd86a-168">Use delta query to track changes in Microsoft Graph data</span></span>](../../../concepts/delta_query_overview.md)
- [<span data-ttu-id="cd86a-169">Inkrementelle Änderungen an Nachrichten in einem Ordner abrufen</span><span class="sxs-lookup"><span data-stu-id="cd86a-169">Get incremental changes to messages in a folder</span></span>](../../../concepts/delta_query_messages.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contactFolder: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->