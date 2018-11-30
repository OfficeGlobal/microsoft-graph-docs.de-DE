---
title: 'contact: delta'
description: Dient zum Abrufen eines Satzes von Kontakten, die einem bestimmten Ordner hinzugefügt bzw. daraus gelöscht oder darin aktualisiert wurden.
ms.openlocfilehash: 1e97a59de7abec0c69a5e02559081f7b344ebad0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062711"
---
# <a name="contact-delta"></a><span data-ttu-id="a8425-103">contact: delta</span><span class="sxs-lookup"><span data-stu-id="a8425-103">contact: delta</span></span>

> <span data-ttu-id="a8425-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a8425-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a8425-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a8425-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a8425-106">Dient zum Abrufen eines Satzes von Kontakten, die einem bestimmten Ordner hinzugefügt bzw. daraus gelöscht oder darin aktualisiert wurden.</span><span class="sxs-lookup"><span data-stu-id="a8425-106">Get a set of contacts that have been added, deleted, or updated in a specified folder.</span></span>

<span data-ttu-id="a8425-p102">Ein **delta**-Funktionsaufruf für Kontakte in einem Ordner ähnelt einer GET-Anforderung, mit der Ausnahme, dass durch entsprechende Anwendung von [Statustoken](/graph/delta-query-overview) in einem oder mehreren dieser Aufrufe inkrementelle Änderungen an den Kontakten im betreffenden Ordner abgefragt werden können. Dies ermöglicht es Ihnen, einen lokalen Speicher der Kontakte eines Benutzers zu pflegen und zu synchronisieren, ohne dass Sie jedes Mal den gesamten Satz Kontakte vom Server abrufen müssen.</span><span class="sxs-lookup"><span data-stu-id="a8425-p102">A **delta** function call for contacts in a folder is similar to a GET request, except that by appropriately applying [state tokens](/graph/delta-query-overview) in one or more of these calls, you can query for incremental changes in the contacts in that folder. This allows you to maintain and synchronize a local store of a user's contacts without having to fetch the entire set of contacts from the server every time.</span></span>  

## <a name="permissions"></a><span data-ttu-id="a8425-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a8425-109">Permissions</span></span>
<span data-ttu-id="a8425-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8425-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8425-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a8425-112">Permission type</span></span>      | <span data-ttu-id="a8425-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a8425-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a8425-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a8425-114">Delegated (work or school account)</span></span> | <span data-ttu-id="a8425-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a8425-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a8425-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a8425-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8425-117">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a8425-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a8425-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a8425-118">Application</span></span> | <span data-ttu-id="a8425-119">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a8425-119">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a8425-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a8425-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}/contacts/delta
GET /users/<id>/contactFolders/{id}/contacts/delta
```

## <a name="query-parameters"></a><span data-ttu-id="a8425-121">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="a8425-121">Query parameters</span></span>

<span data-ttu-id="a8425-p104">Beim Nachverfolgen von Änderungen an Kontakten wird eine Runde von einem oder mehreren **delta**-Funktionsaufrufen ausgeführt. Wenn Sie Abfrageparameter (außer `$deltatoken` und `$skiptoken`) verwenden, müssen Sie sie in der ursprünglichen **delta**-Anforderung angeben. Microsoft Graph codiert automatisch alle angegebenen Parameter in den Tokenteil der in der Antwort enthaltenen `nextLink`- oder `deltaLink`-URL. Sie müssen alle gewünschten Abfrageparameter nur einmal im Vorfeld angeben. In nachfolgenden Anforderungen können Sie die `nextLink`- oder `deltaLink`-URL einfach aus der vorherigen Antwort kopieren und anwenden, da diese URL bereits die codierten gewünschten Parameter enthält.</span><span class="sxs-lookup"><span data-stu-id="a8425-p104">Tracking changes in contacts incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response. You only need to specify any desired query parameters once upfront. In subsequent requests, simply copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="a8425-127">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="a8425-127">Query parameter</span></span>      | <span data-ttu-id="a8425-128">Typ</span><span class="sxs-lookup"><span data-stu-id="a8425-128">Type</span></span>   |<span data-ttu-id="a8425-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a8425-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a8425-130">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="a8425-130">$deltatoken</span></span> | <span data-ttu-id="a8425-131">string</span><span class="sxs-lookup"><span data-stu-id="a8425-131">string</span></span> | <span data-ttu-id="a8425-p105">Ein [Statustoken](/graph/delta-query-overview), das in der `deltaLink`-URL des vorhergehenden **delta**-Funktionsaufrufs für dieselbe Kontaktsammlung zurückgegeben wird und den Abschluss dieser Runde der Änderungsnachverfolgung anzeigt. Speichern Sie die gesamte `deltaLink`-URL einschließlich dieses Tokens, und wenden Sie sie in der ersten Anforderung der nächsten Änderungsnachverfolgungsrunde für diese Sammlung an.</span><span class="sxs-lookup"><span data-stu-id="a8425-p105">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same contact collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="a8425-134">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="a8425-134">$skiptoken</span></span> | <span data-ttu-id="a8425-135">string</span><span class="sxs-lookup"><span data-stu-id="a8425-135">string</span></span> | <span data-ttu-id="a8425-136">Ein [Statustoken](/graph/delta-query-overview), das in der `nextLink`-URL des vorhergehenden **delta**-Funktionsaufrufs zurückgegeben wird und anzeigt, dass in derselben Kontaktsammlung weitere Änderungen zum Nachverfolgen vorliegen.</span><span class="sxs-lookup"><span data-stu-id="a8425-136">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same contact collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="a8425-137">OData-Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="a8425-137">OData query parameters</span></span>

- <span data-ttu-id="a8425-p106">Sie können wie bei jeder GET-Anforderung den Abfrageparameter `$select` verwenden, um zwecks Leistungsoptimierung nur die benötigten Eigenschaften anzugeben. Die Eigenschaft _id_ wird immer zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a8425-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 


## <a name="request-headers"></a><span data-ttu-id="a8425-140">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a8425-140">Request headers</span></span>
| <span data-ttu-id="a8425-141">Name</span><span class="sxs-lookup"><span data-stu-id="a8425-141">Name</span></span>       | <span data-ttu-id="a8425-142">Typ</span><span class="sxs-lookup"><span data-stu-id="a8425-142">Type</span></span> | <span data-ttu-id="a8425-143">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a8425-143">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="a8425-144">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8425-144">Authorization</span></span>  | <span data-ttu-id="a8425-145">string</span><span class="sxs-lookup"><span data-stu-id="a8425-145">string</span></span>  | <span data-ttu-id="a8425-p107">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a8425-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a8425-148">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a8425-148">Content-Type</span></span>  | <span data-ttu-id="a8425-149">string</span><span class="sxs-lookup"><span data-stu-id="a8425-149">string</span></span>  | <span data-ttu-id="a8425-p108">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="a8425-p108">application/json. Required.</span></span> |
| <span data-ttu-id="a8425-152">Prefer</span><span class="sxs-lookup"><span data-stu-id="a8425-152">Prefer</span></span> | <span data-ttu-id="a8425-153">string</span><span class="sxs-lookup"><span data-stu-id="a8425-153">string</span></span>  | <span data-ttu-id="a8425-p109">odata.maxpagesize={x}. Optional.</span><span class="sxs-lookup"><span data-stu-id="a8425-p109">odata.maxpagesize={x}. Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="a8425-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="a8425-156">Response</span></span>

<span data-ttu-id="a8425-157">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [contact](../resources/contact.md)-Sammlungsobjekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a8425-157">If successful, this method returns a `200 OK` response code and [contact](../resources/contact.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8425-158">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a8425-158">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a8425-159">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a8425-159">Request</span></span>
<span data-ttu-id="a8425-160">Das folgende Beispiel zeigt, wie Sie einen einzelnen **delta**-Funktionsaufruf ausführen, den `$select`-Parameter verwenden, um nur die Eigenschaft **displayName** jedes Kontakts abzurufen, und die maximale Anzahl von Kontakten im Antworttext auf 2 beschränken.</span><span class="sxs-lookup"><span data-stu-id="a8425-160">The following example shows how to make a single **delta** function call, use the `$select` parameter to get only each contact's **displayName** property, and limit the maximum number of contacts in the response body to 2.</span></span>

<span data-ttu-id="a8425-161">Zum Nachverfolgen von Änderungen an den Kontakten in einem Ordner führen Sie einen oder mehrere **delta**-Funktionsaufrufe mit entsprechenden Statustoken aus, um den Satz der inkrementellen Änderungen seit der letzten Delta-Abfrage abzurufen.</span><span class="sxs-lookup"><span data-stu-id="a8425-161">To track changes in the contacts in a folder, you would make one or more **delta** function calls, with appropriate state tokens, to get the set of incremental changes since the last delta query.</span></span> 

<span data-ttu-id="a8425-p110">Ein ähnliches Beispiel zeigt, wie die Statustoken zum Nachverfolgen von Änderungen in den Nachrichten eines E-Mail-Ordners verwendet werden: [Inkrementelle Änderungen an Nachrichten in einem Ordner abrufen](/graph/delta-query-messages) Die wichtigsten Unterschiede zwischen dem Nachverfolgen von Kontakten und dem Nachverfolgen von Nachrichten in einem Ordner liegen in den Anforderungs-URLs der Delta-Abfrage vor; außerdem geben die Abfrageantworten **contact**- anstelle von **message**-Sammlungen zurück.</span><span class="sxs-lookup"><span data-stu-id="a8425-p110">You can find a similar example that shows how to use the state tokens to track changes in the messages of a mail folder: [Get incremental changes to messages in a folder](/graph/delta-query-messages). The main differences between tracking contacts and tracking messages in a folder are in the delta query request URLs, and the query responses returning **contact** rather than **message** collections.</span></span>
 
<!-- {
  "blockType": "request",
  "name": "contact_delta"
}-->
```http
GET https://graph.microsoft.com/beta/me/contactFolders/{id}/contacts/delta?$select=displayName

Prefer: odata.maxpagesize=2
```

##### <a name="response"></a><span data-ttu-id="a8425-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="a8425-164">Response</span></span>
<span data-ttu-id="a8425-165">Wenn die Anforderung erfolgreich ist, enthält die Antwort ein Statustoken, entweder ein _skipToken_</span><span class="sxs-lookup"><span data-stu-id="a8425-165">If the request is successful, the response would include a state token, which is either a _skipToken_</span></span>  
<span data-ttu-id="a8425-p111">(in einem _@odata.nextLink_-Antwortheader) oder ein _deltaToken_ (in einem _@odata.deltaLink_-Antwortheader). Diese geben an, ob Sie mit der Runde fortfahren sollten oder ob alle Änderungen für diese Runde abgerufen wurden.</span><span class="sxs-lookup"><span data-stu-id="a8425-p111">(in an _@odata.nextLink_ response header) or a _deltaToken_ (in an _@odata.deltaLink_ response header). Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="a8425-168">Die Antwort unten zeigt ein _skipToken_ in einem _@odata.nextLink_-Antwortheader.</span><span class="sxs-lookup"><span data-stu-id="a8425-168">The response below shows a _skipToken_ in an _@odata.nextLink_ response header.</span></span>

<span data-ttu-id="a8425-p112">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a8425-p112">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "@odata.nextLink":"https://graph.microsoft.com/beta/me/contactfolders('{id}')/contacts/delta?$skiptoken={_skipToken_}",
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

### <a name="see-also"></a><span data-ttu-id="a8425-171">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="a8425-171">See also</span></span>

- [<span data-ttu-id="a8425-172">Microsoft Graph-Delta-Abfrage</span><span class="sxs-lookup"><span data-stu-id="a8425-172">Microsoft Graph delta query</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="a8425-173">Inkrementelle Änderungen an Nachrichten in einem Ordner abrufen</span><span class="sxs-lookup"><span data-stu-id="a8425-173">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contact: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->