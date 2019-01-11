---
title: 'message: delta'
description: Dient zum Abrufen eines Satzes von Nachrichten, die einem bestimmten Ordner hinzugefügt bzw. daraus gelöscht oder darin aktualisiert wurden.
localization_priority: Normal
ms.openlocfilehash: 149acc68081d8497567f07fe6d58f4b42a0c031d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852059"
---
# <a name="message-delta"></a><span data-ttu-id="fe462-103">message: delta</span><span class="sxs-lookup"><span data-stu-id="fe462-103">message: delta</span></span>

> <span data-ttu-id="fe462-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="fe462-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fe462-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fe462-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fe462-106">Dient zum Abrufen eines Satzes von Nachrichten, die einem bestimmten Ordner hinzugefügt bzw. daraus gelöscht oder darin aktualisiert wurden.</span><span class="sxs-lookup"><span data-stu-id="fe462-106">Get a set of messages that have been added, deleted, or updated in a specified folder.</span></span>

<span data-ttu-id="fe462-p102">Ein **delta**-Funktionsaufruf für Nachrichten in einem Ordner ähnelt einer GET-Anforderung, mit der Ausnahme, dass durch entsprechende Anwendung von [Statustoken](/graph/delta-query-overview) in einem oder mehreren dieser Aufrufe [inkrementelle Änderungen an den Nachrichten im betreffenden Ordner abgefragt](/graph/delta-query-messages) werden können. Dies ermöglicht es Ihnen, einen lokalen Speicher der Nachrichten eines Benutzers zu pflegen und zu synchronisieren, ohne dass Sie jedes Mal den gesamten Satz Nachrichten vom Server abrufen müssen.</span><span class="sxs-lookup"><span data-stu-id="fe462-p102">A **delta** function call for messages in a folder is similar to a GET request, except that by appropriately applying [state tokens](/graph/delta-query-overview) in one or more of these calls, you can [query for incremental changes in the messages in that folder](/graph/delta-query-messages). This allows you to maintain and synchronize a local store of a user's messages without having to fetch the entire set of messages from the server every time.</span></span>  

## <a name="permissions"></a><span data-ttu-id="fe462-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="fe462-109">Permissions</span></span>
<span data-ttu-id="fe462-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe462-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe462-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fe462-112">Permission type</span></span>      | <span data-ttu-id="fe462-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fe462-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe462-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fe462-114">Delegated (work or school account)</span></span> | <span data-ttu-id="fe462-115">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fe462-115">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="fe462-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fe462-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe462-117">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fe462-117">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="fe462-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fe462-118">Application</span></span> | <span data-ttu-id="fe462-119">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fe462-119">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe462-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fe462-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages/delta
GET /users/<id>/mailFolders/{id}/messages/delta
```

## <a name="query-parameters"></a><span data-ttu-id="fe462-121">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="fe462-121">Query parameters</span></span>

<span data-ttu-id="fe462-p104">Beim Nachverfolgen von Änderungen in Nachrichten wird eine Runde von einem oder mehreren **delta**-Funktionsaufrufen ausgeführt. Wenn Sie Abfrageparameter (außer `$deltatoken` und `$skiptoken`) verwenden, müssen Sie sie in der ursprünglichen **delta**-Anforderung angeben. Microsoft Graph codiert automatisch alle angegebenen Parameter in den Tokenteil der in der Antwort enthaltenen `nextLink`- oder `deltaLink`-URL. Sie müssen alle gewünschten Abfrageparameter nur einmal im Vorfeld angeben. In nachfolgenden Anforderungen können Sie die `nextLink`- oder `deltaLink`-URL einfach aus der vorherigen Antwort kopieren und anwenden, da diese URL bereits die codierten gewünschten Parameter enthält.</span><span class="sxs-lookup"><span data-stu-id="fe462-p104">Tracking changes in messages incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response. You only need to specify any desired query parameters once upfront. In subsequent requests, simply copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="fe462-127">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="fe462-127">Query parameter</span></span>      | <span data-ttu-id="fe462-128">Typ</span><span class="sxs-lookup"><span data-stu-id="fe462-128">Type</span></span>   |<span data-ttu-id="fe462-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fe462-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fe462-130">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="fe462-130">$deltatoken</span></span> | <span data-ttu-id="fe462-131">string</span><span class="sxs-lookup"><span data-stu-id="fe462-131">string</span></span> | <span data-ttu-id="fe462-p105">Ein [Statustoken](/graph/delta-query-overview), das in der `deltaLink`-URL des vorhergehenden **delta**-Funktionsaufrufs für dieselbe Nachrichtensammlung zurückgegeben wird und den Abschluss dieser Runde der Änderungsnachverfolgung anzeigt. Speichern Sie die gesamte `deltaLink`-URL einschließlich dieses Tokens, und wenden Sie sie in der ersten Anforderung der nächsten Änderungsnachverfolgungsrunde für diese Sammlung an.</span><span class="sxs-lookup"><span data-stu-id="fe462-p105">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same message collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="fe462-134">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="fe462-134">$skiptoken</span></span> | <span data-ttu-id="fe462-135">string</span><span class="sxs-lookup"><span data-stu-id="fe462-135">string</span></span> | <span data-ttu-id="fe462-136">Ein [Statustoken](/graph/delta-query-overview), das in der `nextLink`-URL des vorhergehenden **delta**-Funktionsaufrufs zurückgegeben wird und anzeigt, dass in derselben Nachrichtensammlung weitere Änderungen zum Nachverfolgen vorliegen.</span><span class="sxs-lookup"><span data-stu-id="fe462-136">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same message collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="fe462-137">OData-Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="fe462-137">OData query parameters</span></span>

- <span data-ttu-id="fe462-p106">Sie können wie bei jeder GET-Anforderung den Abfrageparameter `$select` verwenden, um zwecks Leistungsoptimierung nur die benötigten Eigenschaften anzugeben. Die Eigenschaft _id_ wird immer zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fe462-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 
- <span data-ttu-id="fe462-140">Die Delta-Abfrage unterstützt `$select`, `$top` und `$expand` für Nachrichten.</span><span class="sxs-lookup"><span data-stu-id="fe462-140">Delta query support `$select`, `$top`, and `$expand` for messages.</span></span> 
- <span data-ttu-id="fe462-141">Es besteht eingeschränkte Unterstützung für `$filter` und `$orderby`:</span><span class="sxs-lookup"><span data-stu-id="fe462-141">There is limited support for `$filter` and `$orderby`:</span></span>
  * <span data-ttu-id="fe462-142">Es werden nur die `$filter`-Ausdrücke `$filter=receivedDateTime+ge+{value}` oder `$filter=receivedDateTime+gt+{value}` unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fe462-142">The only supported `$filter` expresssions are `$filter=receivedDateTime+ge+{value}` or `$filter=receivedDateTime+gt+{value}`.</span></span>
  * <span data-ttu-id="fe462-p107">Es wird nur der `$orderby`-Ausdruck `$orderby=receivedDateTime+desc` unterstützt. Wenn Sie keinen `$orderby`-Ausdruck einschließen, ist die Rückgabereihenfolge nicht gewährleistet.</span><span class="sxs-lookup"><span data-stu-id="fe462-p107">The only supported `$orderby` expression is `$orderby=receivedDateTime+desc`. If you do not include an `$orderby` expression, the return order is not guaranteed.</span></span> 
- <span data-ttu-id="fe462-145">`$search` wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fe462-145">There is no support for `$search`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fe462-146">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fe462-146">Request headers</span></span>
| <span data-ttu-id="fe462-147">Name</span><span class="sxs-lookup"><span data-stu-id="fe462-147">Name</span></span>       | <span data-ttu-id="fe462-148">Typ</span><span class="sxs-lookup"><span data-stu-id="fe462-148">Type</span></span> | <span data-ttu-id="fe462-149">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fe462-149">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="fe462-150">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe462-150">Authorization</span></span>  | <span data-ttu-id="fe462-151">string</span><span class="sxs-lookup"><span data-stu-id="fe462-151">string</span></span>  | <span data-ttu-id="fe462-p108">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fe462-p108">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fe462-154">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fe462-154">Content-Type</span></span>  | <span data-ttu-id="fe462-155">string</span><span class="sxs-lookup"><span data-stu-id="fe462-155">string</span></span>  | <span data-ttu-id="fe462-p109">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="fe462-p109">application/json. Required.</span></span> |
| <span data-ttu-id="fe462-158">Prefer</span><span class="sxs-lookup"><span data-stu-id="fe462-158">Prefer</span></span> | <span data-ttu-id="fe462-159">string</span><span class="sxs-lookup"><span data-stu-id="fe462-159">string</span></span>  | <span data-ttu-id="fe462-p110">odata.maxpagesize={x}. Optional.</span><span class="sxs-lookup"><span data-stu-id="fe462-p110">odata.maxpagesize={x}. Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="fe462-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="fe462-162">Response</span></span>

<span data-ttu-id="fe462-163">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [message](../resources/message.md)-Sammlungsobjekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fe462-163">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe462-164">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fe462-164">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fe462-165">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fe462-165">Request</span></span>
<span data-ttu-id="fe462-166">Das folgende Beispiel zeigt, wie Sie einen einzelnen **delta**-Funktionsaufruf ausführen und die maximale Anzahl von Nachrichten im Textkörper der Antwort auf 2 beschränken.</span><span class="sxs-lookup"><span data-stu-id="fe462-166">The following example shows how to make a single **delta** function call, and limit the maximum number of messages in the response body to 2.</span></span>

<span data-ttu-id="fe462-p111">Zum Nachverfolgen von Änderungen in den Nachrichten eines Ordners führen Sie einen oder mehrere **delta**-Funktionsaufrufe aus, um den Satz der inkrementellen Änderungen seit der letzten Delta-Abfrage abzurufen. Ein Beispiel für eine Runde von Delta-Abfrageaufrufen finden Sie unter [Inkrementelle Änderungen an Nachrichten in einem Ordner abrufen](/graph/delta-query-messages).</span><span class="sxs-lookup"><span data-stu-id="fe462-p111">To track changes in the messages in a folder, you would make one or more **delta** function calls to get the set of incremental changes since the last delta query. For an example that shows a round of delta query calls, see [Get incremental changes to messages in a folder](/graph/delta-query-messages).</span></span>
 
<!-- {
  "blockType": "request",
  "name": "message_delta"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders/{id}/messages/delta

Prefer: odata.maxpagesize=2
```

##### <a name="response"></a><span data-ttu-id="fe462-169">Antwort</span><span class="sxs-lookup"><span data-stu-id="fe462-169">Response</span></span>
<span data-ttu-id="fe462-170">Wenn die Anforderung erfolgreich ist, enthält die Antwort ein Statustoken, entweder ein _skipToken_</span><span class="sxs-lookup"><span data-stu-id="fe462-170">If the request is successful, the response would include a state token, which is either a _skipToken_</span></span>  
<span data-ttu-id="fe462-p112">(in einem _@odata.nextLink_-Antwortheader) oder ein _deltaToken_ (in einem _@odata.deltaLink_-Antwortheader). Diese geben an, ob Sie mit der Runde fortfahren sollten oder ob alle Änderungen für diese Runde abgerufen wurden.</span><span class="sxs-lookup"><span data-stu-id="fe462-p112">(in an _@odata.nextLink_ response header) or a _deltaToken_ (in an _@odata.deltaLink_ response header). Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="fe462-173">Die Antwort unten zeigt ein _skipToken_ in einem _@odata.nextLink_-Antwortheader.</span><span class="sxs-lookup"><span data-stu-id="fe462-173">The response below shows a _skipToken_ in an _@odata.nextLink_ response header.</span></span>

<span data-ttu-id="fe462-p113">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fe462-p113">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "@odata.nextLink":"https://graph.microsoft.com/beta/me/mailfolders('{id}')/messages/delta?$skiptoken={_skipToken_}",
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

### <a name="see-also"></a><span data-ttu-id="fe462-176">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="fe462-176">See also</span></span>

- [<span data-ttu-id="fe462-177">Microsoft Graph-Delta-Abfrage</span><span class="sxs-lookup"><span data-stu-id="fe462-177">Microsoft Graph delta query</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="fe462-178">Inkrementelle Änderungen an Nachrichten in einem Ordner abrufen</span><span class="sxs-lookup"><span data-stu-id="fe462-178">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
