---
title: 'contactFolder: delta'
description: Dient zum Abrufen eines Satzes von Kontaktordnern, die dem Postfach des Benutzers hinzugefügt bzw. daraus gelöscht oder entfernt wurden.
localization_priority: Normal
ms.openlocfilehash: 87474f4a70d4730bfb9d510c43c017d86883116a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815267"
---
# <a name="contactfolder-delta"></a><span data-ttu-id="0b84c-103">contactFolder: delta</span><span class="sxs-lookup"><span data-stu-id="0b84c-103">contactFolder: delta</span></span>

<span data-ttu-id="0b84c-104">Dient zum Abrufen eines Satzes von Kontaktordnern, die dem Postfach des Benutzers hinzugefügt bzw. daraus gelöscht oder entfernt wurden.</span><span class="sxs-lookup"><span data-stu-id="0b84c-104">Get a set of contact folders that have been added, deleted, or removed from the user's mailbox.</span></span>

<span data-ttu-id="0b84c-p101">Ein **delta**-Funktionsaufruf für Kontaktordner in einem Postfach ähnelt einer GET-Anforderung, mit der Ausnahme, dass durch entsprechende Anwendung von [Statustoken](/graph/delta-query-overview) in einem oder mehreren dieser Aufrufe inkrementelle Änderungen in den Kontaktordnern abgefragt werden können. Dies ermöglicht es Ihnen, einen lokalen Speicher der Kontaktordner eines Benutzers zu pflegen und zu synchronisieren, ohne dass Sie jedes Mal alle Kontaktordner des betreffenden Postfachs vom Server abrufen müssen.</span><span class="sxs-lookup"><span data-stu-id="0b84c-p101">A **delta** function call for contact folders in a mailbox is similar to a GET request, except that by appropriately applying [state tokens](/graph/delta-query-overview) in one or more of these calls, you can query for incremental changes in the contact folders. This allows you to maintain and synchronize a local store of a user's contact folders without having to fetch all the contact folders of that mailbox from the server every time.</span></span>

## <a name="permissions"></a><span data-ttu-id="0b84c-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0b84c-107">Permissions</span></span>
<span data-ttu-id="0b84c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b84c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="0b84c-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0b84c-110">Permission type</span></span>      | <span data-ttu-id="0b84c-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0b84c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b84c-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0b84c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0b84c-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0b84c-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="0b84c-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0b84c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b84c-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0b84c-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="0b84c-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0b84c-116">Application</span></span> | <span data-ttu-id="0b84c-117">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0b84c-117">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0b84c-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0b84c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/delta
GET /users/{id}/contactFolders/delta
```

## <a name="query-parameters"></a><span data-ttu-id="0b84c-119">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="0b84c-119">Query parameters</span></span>

<span data-ttu-id="0b84c-p103">Beim Nachverfolgen von Änderungen in Kontaktordnern wird eine Runde von einem oder mehreren **delta**-Funktionsaufrufen ausgeführt. Wenn Sie Abfrageparameter (außer `$deltatoken` und `$skiptoken`) verwenden, müssen Sie sie in der ursprünglichen **delta**-Anforderung angeben. Microsoft Graph codiert automatisch alle angegebenen Parameter in den Tokenteil (`skiptoken` oder `$deltatoken`) der in der Antwort enthaltenen `nextLink`- oder `deltaLink`-URL. Sie müssen alle gewünschten Abfrageparameter nur einmal im Vorfeld angeben. In nachfolgenden Anforderungen können Sie die `nextLink`- oder `deltaLink`-URL einfach aus der vorherigen Antwort kopieren und anwenden, da diese URL bereits die codierten gewünschten Parameter enthält.</span><span class="sxs-lookup"><span data-stu-id="0b84c-p103">Tracking changes in contact folders incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion (`skiptoken` or `$deltatoken`) of the `nextLink` or `deltaLink` URL provided in the response. You only need to specify any desired query parameters once upfront. In subsequent requests, simply copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="0b84c-125">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="0b84c-125">Query parameter</span></span>      | <span data-ttu-id="0b84c-126">Typ</span><span class="sxs-lookup"><span data-stu-id="0b84c-126">Type</span></span>   |<span data-ttu-id="0b84c-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0b84c-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0b84c-128">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="0b84c-128">$deltatoken</span></span> | <span data-ttu-id="0b84c-129">string</span><span class="sxs-lookup"><span data-stu-id="0b84c-129">string</span></span> | <span data-ttu-id="0b84c-p104">Ein [Statustoken](/graph/delta-query-overview), das in der `deltaLink`-URL des vorhergehenden **delta**-Funktionsaufrufs für dieselbe Sammlung von Kontaktordnern zurückgegeben wird und den Abschluss dieser Runde der Änderungsnachverfolgung anzeigt. Speichern Sie die gesamte `deltaLink`-URL einschließlich dieses Tokens, und wenden Sie sie in der ersten Anforderung der nächsten Änderungsnachverfolgungsrunde für diese Sammlung an.</span><span class="sxs-lookup"><span data-stu-id="0b84c-p104">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same contact folder collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="0b84c-132">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="0b84c-132">$skiptoken</span></span> | <span data-ttu-id="0b84c-133">string</span><span class="sxs-lookup"><span data-stu-id="0b84c-133">string</span></span> | <span data-ttu-id="0b84c-134">Ein [Statustoken](/graph/delta-query-overview), das in der `nextLink`-URL des vorhergehenden **delta**-Funktionsaufrufs zurückgegeben wird und anzeigt, dass in derselben Sammlung von Kontaktordnern weitere Änderungen zum Nachverfolgen vorliegen.</span><span class="sxs-lookup"><span data-stu-id="0b84c-134">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same contact folder collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="0b84c-135">OData-Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="0b84c-135">OData query parameters</span></span>

<span data-ttu-id="0b84c-p105">Sie können wie bei jeder GET-Anforderung den Abfrageparameter `$select` verwenden, um zwecks Leistungsoptimierung nur die benötigten Eigenschaften anzugeben. Die Eigenschaft _id_ wird immer zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0b84c-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="0b84c-138">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0b84c-138">Request headers</span></span>
| <span data-ttu-id="0b84c-139">Name</span><span class="sxs-lookup"><span data-stu-id="0b84c-139">Name</span></span>       | <span data-ttu-id="0b84c-140">Typ</span><span class="sxs-lookup"><span data-stu-id="0b84c-140">Type</span></span> | <span data-ttu-id="0b84c-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0b84c-141">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="0b84c-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b84c-142">Authorization</span></span>  | <span data-ttu-id="0b84c-143">string</span><span class="sxs-lookup"><span data-stu-id="0b84c-143">string</span></span>  | <span data-ttu-id="0b84c-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0b84c-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0b84c-146">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0b84c-146">Content-Type</span></span>  | <span data-ttu-id="0b84c-147">string</span><span class="sxs-lookup"><span data-stu-id="0b84c-147">string</span></span>  | <span data-ttu-id="0b84c-p107">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="0b84c-p107">application/json. Required.</span></span> |
| <span data-ttu-id="0b84c-150">Prefer</span><span class="sxs-lookup"><span data-stu-id="0b84c-150">Prefer</span></span> | <span data-ttu-id="0b84c-151">string</span><span class="sxs-lookup"><span data-stu-id="0b84c-151">string</span></span>  | <span data-ttu-id="0b84c-p108">odata.maxpagesize={x}. Optional.</span><span class="sxs-lookup"><span data-stu-id="0b84c-p108">odata.maxpagesize={x}. Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="0b84c-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="0b84c-154">Response</span></span>

<span data-ttu-id="0b84c-155">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [contactFolder](../resources/contactfolder.md)-Sammlungsobjekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0b84c-155">If successful, this method returns a `200 OK` response code and [contactFolder](../resources/contactfolder.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b84c-156">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0b84c-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0b84c-157">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0b84c-157">Request</span></span>
<span data-ttu-id="0b84c-158">Das folgende Beispiel zeigt, wie Sie einen einzelnen **delta**-Funktionsaufruf ausführen und die maximale Anzahl von Kontaktordnern im Antworttext auf 2 beschränken.</span><span class="sxs-lookup"><span data-stu-id="0b84c-158">The following example shows how to make a single **delta** function call, and limit the maximum number of contact folders in the response body to 2.</span></span>

<span data-ttu-id="0b84c-159">Zum Nachverfolgen von Änderungen in den Kontaktordnern eines Postfachs führen Sie einen oder mehrere **delta**-Funktionsaufrufe mit entsprechenden Statustoken aus, um den Satz der inkrementellen Änderungen seit der letzten Delta-Abfrage abzurufen.</span><span class="sxs-lookup"><span data-stu-id="0b84c-159">To track changes in the contact folders of a mailbox, you would make one or more **delta** function calls, with appropriate state tokens, to get the set of incremental changes since the last delta query.</span></span> 

<span data-ttu-id="0b84c-p109">Ein ähnliches Beispiel zeigt, wie die Statustoken zum Nachverfolgen von Änderungen in den Nachrichten eines E-Mail-Ordners verwendet werden: [Inkrementelle Änderungen an Nachrichten in einem Ordner abrufen](/graph/delta-query-messages) Die wichtigsten Unterschiede zwischen dem Nachverfolgen von Kontaktordnern und dem Nachverfolgen von Nachrichten in einem Ordner liegen in den Anforderungs-URLs der Delta-Abfrage vor; außerdem geben die Abfrageantworten **contactFolder**- anstelle von **message**-Sammlungen zurück.</span><span class="sxs-lookup"><span data-stu-id="0b84c-p109">You can find a similar example that shows how to use the state tokens to track changes in the messages of a mail folder: [Get incremental changes to messages in a folder](/graph/delta-query-messages). The main differences between tracking contact folders and tracking messages in a folder are in the delta query request URLs, and the query responses returning **contactFolder** rather than **message** collections.</span></span>

<!-- {
  "blockType": "request",
  "name": "contactfolder_delta"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contactFolders/delta
Prefer: odata.maxpagesize=2
```

##### <a name="response"></a><span data-ttu-id="0b84c-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="0b84c-162">Response</span></span>

<span data-ttu-id="0b84c-163">Wenn die Anforderung erfolgreich ist, enthält die Antwort ein Statustoken, entweder ein _skipToken_</span><span class="sxs-lookup"><span data-stu-id="0b84c-163">If the request is successful, the response would include a state token, which is either a _skipToken_</span></span>  
<span data-ttu-id="0b84c-p110">(in einem _@odata.nextLink_-Antwortheader) oder ein _deltaToken_ (in einem _@odata.deltaLink_-Antwortheader). Diese geben an, ob Sie mit der Runde fortfahren sollten oder ob alle Änderungen für diese Runde abgerufen wurden.</span><span class="sxs-lookup"><span data-stu-id="0b84c-p110">(in an _@odata.nextLink_ response header) or a _deltaToken_ (in an _@odata.deltaLink_ response header). Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="0b84c-166">Die Antwort unten zeigt ein _skipToken_ in einem _@odata.nextLink_-Antwortheader.</span><span class="sxs-lookup"><span data-stu-id="0b84c-166">The response below shows a _skipToken_ in an _@odata.nextLink_ response header.</span></span>

<span data-ttu-id="0b84c-p111">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0b84c-p111">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

### <a name="see-also"></a><span data-ttu-id="0b84c-169">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="0b84c-169">See also</span></span>

- [<span data-ttu-id="0b84c-170">Verwenden einer Delta-Abfrage zum Nachverfolgen von Änderungen in Microsoft Graph-Daten</span><span class="sxs-lookup"><span data-stu-id="0b84c-170">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="0b84c-171">Inkrementelle Änderungen an Nachrichten in einem Ordner abrufen</span><span class="sxs-lookup"><span data-stu-id="0b84c-171">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contactFolder: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
