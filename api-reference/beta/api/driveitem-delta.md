---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Synchronisieren der Inhalte eines Laufwerks
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 14cc73d9e90c71815e6c72047fe78bf2b325abdd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525318"
---
# <a name="track-changes-for-a-drive"></a><span data-ttu-id="b5cc0-102">Laufwerksänderungen nachverfolgen</span><span class="sxs-lookup"><span data-stu-id="b5cc0-102">Track changes for a Drive</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5cc0-103">Mit dieser Methode kann Ihre App Änderungen nachverfolgen, die im Laufe der Zeit an Laufwerken sowie deren untergeordneten Elementen vorgenommen werden.</span><span class="sxs-lookup"><span data-stu-id="b5cc0-103">This method allows your app to track changes to a drive and its children over time.</span></span>

<span data-ttu-id="b5cc0-p101">Die App ruft zunächst `delta` ohne Parameter auf. Der Dienst startet dann eine Enumeration der Laufwerkshierarchie und gibt Seiten mit Elementen sowie entweder einen `@odata.nextLink` oder einen `@odata.deltaLink` zurück, wie unten beschrieben. Die App sollte die Aufrufe solange mit dem `@odata.nextLink` fortführen, bis kein `@odata.nextLink` mehr zurückgegeben wird oder bis eine Antwort mit einem leeren Satz an Änderungen zurückgegeben wird.</span><span class="sxs-lookup"><span data-stu-id="b5cc0-p101">Your app begins by calling `delta` without any parameters. The service starts enumerating the drive's hierarchy, returning pages of items and either an `@odata.nextLink` or an `@odata.deltaLink`, as described below. Your app should continue calling with the `@odata.nextLink` until you no longer see an `@odata.nextLink` returned, or you see a response with an empty set of changes.</span></span>

<span data-ttu-id="b5cc0-p102">Sobald alle Änderungen empfangen wurden, können Sie sie auf den lokalen Zustand anwenden. Wenn Sie zu einem späteren Zeitpunkt nochmals auf Änderungen prüfen möchten, rufen Sie erneut `delta` auf, mit dem `@odata.deltaLink` aus der vorherigen Antwort.</span><span class="sxs-lookup"><span data-stu-id="b5cc0-p102">After you have finished receiving all the changes, you may apply them to your local state. To check for changes in the future, call `delta` again with the `@odata.deltaLink` from the previous response.</span></span>

<span data-ttu-id="b5cc0-p103">Gelöschte Elemente werden mit dem [`deleted`-Facet](../resources/deleted.md) zurückgegeben. Elemente, für die diese Eigenschaft festgelegt ist, sollten aus dem lokalen Zustand entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="b5cc0-p103">Deleted items are returned with the [`deleted` facet](../resources/deleted.md). Items with this property set should be removed from your local state.</span></span> 

<span data-ttu-id="b5cc0-111">**Hinweis:** Löschen Sie Ordner nur lokal, wenn sie nach der Synchronisierung aller Änderungen leer sind.</span><span class="sxs-lookup"><span data-stu-id="b5cc0-111">**Note:** you should only delete a folder locally if it is empty after syncing all the changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="b5cc0-112">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b5cc0-112">Permissions</span></span>

<span data-ttu-id="b5cc0-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5cc0-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5cc0-115">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b5cc0-115">Permission type</span></span>      | <span data-ttu-id="b5cc0-116">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b5cc0-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b5cc0-117">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b5cc0-117">Delegated (work or school account)</span></span> | <span data-ttu-id="b5cc0-118">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5cc0-118">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="b5cc0-119">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b5cc0-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5cc0-120">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5cc0-120">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="b5cc0-121">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b5cc0-121">Application</span></span> | <span data-ttu-id="b5cc0-122">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5cc0-122">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b5cc0-123">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b5cc0-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/root/delta
GET /groups/{groupId}/drive/root/delta
GET /me/drive/root/delta
GET /sites/{siteId}/drive/root/delta
GET /users/{userId}/drive/root/delta
```

## <a name="function-parameters"></a><span data-ttu-id="b5cc0-124">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="b5cc0-124">Function parameters</span></span>

| <span data-ttu-id="b5cc0-125">Parameter</span><span class="sxs-lookup"><span data-stu-id="b5cc0-125">Parameter</span></span>   | <span data-ttu-id="b5cc0-126">Typ</span><span class="sxs-lookup"><span data-stu-id="b5cc0-126">Type</span></span>  | <span data-ttu-id="b5cc0-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b5cc0-127">Description</span></span>                                                                                                                          |
|:-------|:-------|:-------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="b5cc0-128">token</span><span class="sxs-lookup"><span data-stu-id="b5cc0-128">token</span></span>  | <span data-ttu-id="b5cc0-129">string</span><span class="sxs-lookup"><span data-stu-id="b5cc0-129">string</span></span> | <span data-ttu-id="b5cc0-130">Optional.</span><span class="sxs-lookup"><span data-stu-id="b5cc0-130">Optional.</span></span> <span data-ttu-id="b5cc0-131">Falls nicht angegeben, wird der aktuelle Status der Hierarchie aufgelistet.</span><span class="sxs-lookup"><span data-stu-id="b5cc0-131">If unspecified, enumerates the hierarchy's current state.</span></span> <span data-ttu-id="b5cc0-132">Für `latest` wird eine leere Antwort mit dem neuesten Delta-Token zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b5cc0-132">If `latest`, returns empty response with latest delta token.</span></span> <span data-ttu-id="b5cc0-133">Im Fall eines vorherigen Delta-Token wird der neue Status seit diesem Token zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b5cc0-133">If a previous delta token, returns new state since that token.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="b5cc0-134">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="b5cc0-134">Optional query parameters</span></span>

<span data-ttu-id="b5cc0-135">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) von  `$select`, `$expand` und `$top` zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b5cc0-135">This method supports the `$select`, `$expand`, and `$top` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="b5cc0-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="b5cc0-136">Response</span></span>

<span data-ttu-id="b5cc0-137">Bei Erfolg gibt diese Methode den Antwortcode `200 OK` und eine Sammlung von Ressourcen des Typs [DriveItem](../resources/driveitem.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b5cc0-137">If successful, this method returns a `200 OK` response code and a collection of [DriveItem](../resources/driveitem.md) resources in the response body.</span></span>

<span data-ttu-id="b5cc0-138">Zusätzlich zu der Sammlung von DriveItems enthält die Antwort außerdem eine der folgenden Eigenschaften:</span><span class="sxs-lookup"><span data-stu-id="b5cc0-138">In addition to the collection of DriveItems, the response will also include one of the following properties:</span></span>

| <span data-ttu-id="b5cc0-139">Name</span><span class="sxs-lookup"><span data-stu-id="b5cc0-139">Name</span></span>                 | <span data-ttu-id="b5cc0-140">Wert</span><span class="sxs-lookup"><span data-stu-id="b5cc0-140">Value</span></span>  | <span data-ttu-id="b5cc0-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b5cc0-141">Description</span></span>                                                                                                                                      |
|:---------------------|:-------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="b5cc0-142">**@odata.nextLink**</span><span class="sxs-lookup"><span data-stu-id="b5cc0-142">**@odata.nextLink**</span></span>  | <span data-ttu-id="b5cc0-143">url</span><span class="sxs-lookup"><span data-stu-id="b5cc0-143">url</span></span>    | <span data-ttu-id="b5cc0-144">Eine URL zum Abrufen der nächsten verfügbaren Seite von Änderungen, sofern weitere Änderungen im aktuellen Satz vorhanden sind</span><span class="sxs-lookup"><span data-stu-id="b5cc0-144">A URL to retrieve the next available page of changes, if there are additional changes in the current set.</span></span>                                        |
| <span data-ttu-id="b5cc0-145">**@odata.deltaLink**</span><span class="sxs-lookup"><span data-stu-id="b5cc0-145">**@odata.deltaLink**</span></span> | <span data-ttu-id="b5cc0-146">url</span><span class="sxs-lookup"><span data-stu-id="b5cc0-146">url</span></span>    | <span data-ttu-id="b5cc0-p106">Eine URL, die anstelle eines **@odata.nextLink** zurückgegeben wird, sobald alle aktuellen Änderungen zurückgegeben wurden. Sie wird verwendet, um zu einem späteren Zeitpunkt den nächsten Satz von Änderungen zu lesen.</span><span class="sxs-lookup"><span data-stu-id="b5cc0-p106">A URL returned instead of **@odata.nextLink** after all current changes have been returned. Used to read the next set of changes in the future.</span></span>  |

## <a name="example-initial-request"></a><span data-ttu-id="b5cc0-149">Beispiel (ursprüngliche Anforderung)</span><span class="sxs-lookup"><span data-stu-id="b5cc0-149">Example (Initial Request)</span></span>

<span data-ttu-id="b5cc0-150">Hier sehen Sie ein Beispiel für einen Aufruf dieser API zur Ermittlung Ihres lokalen Zustands.</span><span class="sxs-lookup"><span data-stu-id="b5cc0-150">Here is an example of how to call this API to establish your local state.</span></span>

### <a name="request"></a><span data-ttu-id="b5cc0-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b5cc0-151">Request</span></span>

<span data-ttu-id="b5cc0-152">Unten ein Beispiel für eine ursprüngliche Anforderung:</span><span class="sxs-lookup"><span data-stu-id="b5cc0-152">Here is an example of the initial request.</span></span>

<!-- { "blockType": "request", "name": "get_item_delta_first" } -->

```http
GET https://graph.microsoft.com/v1.0/me/drive/root/delta
```

### <a name="response"></a><span data-ttu-id="b5cc0-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="b5cc0-153">Response</span></span>

<span data-ttu-id="b5cc0-154">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b5cc0-154">Here is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItem)", "truncated": true, "scope": "file.read" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "0123456789abc",
            "name": "folder2",
            "folder": { }
        },
        {
            "id": "123010204abac",
            "name": "file.txt",
            "file": { }
        },
        {
            "id": "2353010204ddgg",
            "name": "file5.txt",
            "deleted": { }
        }
    ],
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/drive/delta(token=1230919asd190410jlka)"
}
```

<span data-ttu-id="b5cc0-p107">Diese Antwort enthält die erste Seite von Änderungen. Die Eigenschaft **@odata.nextLink** gibt an, dass im aktuellen Satz von Elementen weitere Elemente verfügbar sind. Die App sollte nun solange den URL-Wert von **@odata.nextLink** anfordern, bis alle Seiten von Elementen abgerufen wurden.</span><span class="sxs-lookup"><span data-stu-id="b5cc0-p107">This response includes the first page of changes, and the **@odata.nextLink** property indicates that there are more items available in the current set of items. Your app should continue to request the URL value of **@odata.nextLink** until all pages of items have been retrieved.</span></span>

## <a name="example-last-page-in-a-set"></a><span data-ttu-id="b5cc0-157">Beispiel (letzte Seite in einem Satz)</span><span class="sxs-lookup"><span data-stu-id="b5cc0-157">Example (Last page in a set)</span></span>

<span data-ttu-id="b5cc0-158">Unten sehen Sie ein Beispiel für einen Aufruf dieser API zur Aktualisierung Ihres lokalen Zustands.</span><span class="sxs-lookup"><span data-stu-id="b5cc0-158">Here is an example of how to call this API to update your local state.</span></span>

### <a name="request"></a><span data-ttu-id="b5cc0-159">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b5cc0-159">Request</span></span>

<span data-ttu-id="b5cc0-160">Hier sehen Sie ein Beispiel für eine Anforderung nach der ursprünglichen Anforderung:</span><span class="sxs-lookup"><span data-stu-id="b5cc0-160">Here is an example request after the initial request.</span></span>

<!-- { "blockType": "request", "name": "get_item_delta_last" }-->

```http
GET https://graph.microsoft.com/v1.0/me/drive/root/delta(token='1230919asd190410jlka')
```

### <a name="response"></a><span data-ttu-id="b5cc0-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="b5cc0-161">Response</span></span>

<span data-ttu-id="b5cc0-162">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b5cc0-162">Here is an example of the response.</span></span>

<!-- { "blockType": "response", "truncated": true, "@odata.type": "Collection(microsoft.graph.driveItem)", "scope": "file.read" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "0123456789abc",
            "name": "folder2",
            "folder": { },
            "deleted": { }
        },
        {
            "id": "123010204abac",
            "name": "file.txt",
            "file": { }
        }
    ],
    "@odata.deltaLink": "https://graph.microsoft.com/v1.0/me/drive/root/delta?(token='1230919asd190410jlka')"
}
```

<span data-ttu-id="b5cc0-163">Diese Antwort gibt an, dass im Zeitraum zwischen der ursprünglichen Anforderung und dieser Anforderung zur Aktualisierung des lokalen Zustands das Element `folder2` gelöscht wurde und das Element `file.txt` entweder hinzugefügt oder geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="b5cc0-163">This response indicates that the item named `folder2` was deleted and the item `file.txt` was either added or modified between the initial request and this request to update the local state.</span></span>

<span data-ttu-id="b5cc0-164">Die letzte Seite mit Elementen enthält die Eigenschaft **@odata.deltaLink**. Sie spezifiziert die URL, über die zu einem späteren Zeitpunkt Änderungen abgerufen werden können, die bis dahin an dem jetzt aktuellen Elementsatz vorgenommen wurden.</span><span class="sxs-lookup"><span data-stu-id="b5cc0-164">The final page of items will include the **@odata.deltaLink** property, which provides the URL that can be used later to retrieve changes since the current set of items.</span></span>

<span data-ttu-id="b5cc0-p108">Es kann passieren, dass der Dienst für ein Token keine Änderungsliste zurückgeben kann. (Das ist beispielsweise der Fall, wenn ein Client nach einer längeren Verbindungsunterbrechung versucht, ein altes Token wiederzuverwenden, oder wenn sich der Zustand eines Servers geändert hat und daher ein neues Token erforderlich ist.) In solchen Fällen gibt der Dienst einen Fehler des Typs `HTTP 410 Gone` zurück. Die Fehlerantwort enthält einen der unten aufgeführten Fehlercodes und einen Header `Location` mit einem neuen „nextLink“, der eine vollständig neue „delta“-Enumeration startet. Vergleichen Sie nach Abschluss der vollständigen Enumeration die zurückgegebenen Elemente mit Ihrem lokalen Zustand, und befolgen Sie diese Anweisungen:</span><span class="sxs-lookup"><span data-stu-id="b5cc0-p108">There may be cases when the service can't provide a list of changes for a given token (for example, if a client tries to reuse an old token after being disconnected for a long time, or if server state has changed and a new token is required). In these cases the service will return an `HTTP 410 Gone` error with an error response containing one of the error codes below, and a `Location` header containing a new nextLink that starts a fresh delta enumeration from scratch. After finishing the full enumeration, compare the returned items with your local state and follow these instructions.</span></span>

| <span data-ttu-id="b5cc0-168">Fehlertyp</span><span class="sxs-lookup"><span data-stu-id="b5cc0-168">Error Type</span></span>                       | <span data-ttu-id="b5cc0-169">Anweisungen</span><span class="sxs-lookup"><span data-stu-id="b5cc0-169">Instructions</span></span>                                                                                                                                                                                                                    |
|:---------------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `resyncChangesApplyDifferences`  | <span data-ttu-id="b5cc0-p109">Ersetzen Sie alle lokalen Elemente durch die Serverversion (einschließlich gelöschter Elemente), wenn Sie sicher sind, dass der Dienst bei der letzten Synchronisierung mit den lokalen Änderungen aktualisiert wurde. Laden Sie alle lokalen Änderungen hoch, die dem Server noch nicht bekannt sind.</span><span class="sxs-lookup"><span data-stu-id="b5cc0-p109">Replace any local items with the server's version (including deletes) if you're sure that the service was up to date with your local changes when you last sync'd. Upload any local changes that the server doesn't know about.</span></span> |
| `resyncChangesUploadDifferences` | <span data-ttu-id="b5cc0-172">Laden Sie alle lokalen Elemente hoch, die der Dienst nicht zurückgegeben hat, und laden Sie alle Dateien hoch, die sich von der Version auf dem Server unterscheiden (wobei Sie beide Kopien beibehalten, wenn Sie nicht sicher sind, welche die aktuelle ist).</span><span class="sxs-lookup"><span data-stu-id="b5cc0-172">Upload any local items that the service did not return, and upload any files that differ from the server's version (keeping both copies if you're not sure which one is more up-to-date).</span></span>                                       |

## <a name="retrieving-the-current-deltalink"></a><span data-ttu-id="b5cc0-173">Abrufen des aktuellen deltaLink</span><span class="sxs-lookup"><span data-stu-id="b5cc0-173">Retrieving the current deltaLink</span></span>

<span data-ttu-id="b5cc0-174">In einigen Fällen kann es sinnvoll sein, den aktuellen Wert von DeltaLink anzufordern, ohne zunächst die bereits auf dem Laufwerk vorhandenen Elemente aufzulisten.</span><span class="sxs-lookup"><span data-stu-id="b5cc0-174">In some scenarios, it may be useful to request the current deltaLink value without first enumerating all of the items in the drive already.</span></span>

<span data-ttu-id="b5cc0-175">Dies kann hilfreich sein, wenn die App nur über Änderungen informiert werden möchte und vorhandene Elemente keine Rolle spielen.</span><span class="sxs-lookup"><span data-stu-id="b5cc0-175">This can be useful if your app only wants to know about changes, and doesn't need to know about existing items.</span></span>
<span data-ttu-id="b5cc0-176">Rufen Sie zum Abrufen des aktuellen deltaLink `delta` mit dem Abfragezeichenfolgenparameter `?token=latest` auf.</span><span class="sxs-lookup"><span data-stu-id="b5cc0-176">To retrieve the latest deltaLink, call `delta` with a query string parameter `?token=latest`.</span></span>

<span data-ttu-id="b5cc0-177">**Hinweis: Wenn Sie versuchen, eine vollständige lokale Darstellung der Elemente in einem Ordner oder Laufwerk zu verwalten, müssen Sie `delta` für die erste Enumeration verwenden. Andere Methoden, z. B. Auslagerung über die `children`-Sammlung eines Ordners, geben nicht unbedingt jedes einzelne Element zurück, wenn während der Enumeration ein Schreibvorgang ausgeführt wird. Die Verwendung von `delta` ist die einzige Möglichkeit sicherzustellen, dass Sie alle erforderlichen Daten gelesen haben.**</span><span class="sxs-lookup"><span data-stu-id="b5cc0-177">**Note: If you are trying to maintain a full local representation of the items in a folder or a drive, you must use `delta` for the initial enumeration. Other approaches, such as paging through the `children` collection of a folder, are not guaranteed to return every single item if any writes take place during the enumeration. Using `delta` is the only way to guarantee that you've read all of the data you need to.**</span></span>

### <a name="request"></a><span data-ttu-id="b5cc0-178">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b5cc0-178">Request</span></span>

<!-- { "blockType": "request", "name": "get-delta-latest", "scope": "files.read", "target": "action" } -->

```http
GET /me/drive/root/delta?token=latest
```

### <a name="response"></a><span data-ttu-id="b5cc0-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="b5cc0-179">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItem)" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [ ],
    "@odata.deltaLink": "https://graph.microsoft.com/v1.0/me/drive/root/delta?token=1230919asd190410jlka"
}
```

## <a name="remarks"></a><span data-ttu-id="b5cc0-180">HinwBemerkungeneise</span><span class="sxs-lookup"><span data-stu-id="b5cc0-180">Remarks</span></span>

* <span data-ttu-id="b5cc0-p111">Der „delta“-Feed zeigt den aktuellen Zustand jedes Elements, nicht jede Änderung. Wenn ein Element beispielsweise zweimal umbenannt wurde, wird es nur einmal angezeigt, mit seinem neuesten Namen.</span><span class="sxs-lookup"><span data-stu-id="b5cc0-p111">The delta feed shows the latest state for each item, not each change. If an item were renamed twice, it would only show up once, with its latest name.</span></span>
* <span data-ttu-id="b5cc0-p112">Ein Element kann mehrmals in einem „delta“-Feed aufgeführt werden, aus jeweils unterschiedlichen Gründen. Verwenden Sie das letzte Vorkommen in der Auflistung.</span><span class="sxs-lookup"><span data-stu-id="b5cc0-p112">The same item may appear more than once in a delta feed, for various reasons. You should use the last occurrence you see.</span></span>
* <span data-ttu-id="b5cc0-p113">Die Eigenschaft `parentReference` von Elementen enthält keinen Wert für **path**. Der Grund: Wenn ein Ordner umbenannt wird, gibt **delta** keine Nachfolger dieses Ordners zurück. **Bei Verwendung von „delta“ sollten Sie Elemente immer anhand ihrer ID nachverfolgen.**</span><span class="sxs-lookup"><span data-stu-id="b5cc0-p113">The `parentReference` property on items will not include a value for **path**. This occurs because renaming a folder does not result in any descendants of the folder being returned from **delta**. **When using delta you should always track items by id**.</span></span>
* <span data-ttu-id="b5cc0-188">In OneDrive for Business und SharePoint wird `delta` nur für den Ordner `root` unterstützt, für andere Ordner auf einem Laufwerk jedoch nicht.</span><span class="sxs-lookup"><span data-stu-id="b5cc0-188">In OneDrive for Business and SharePoint, `delta` is only supported on the `root` folder, not on other folders within a drive.</span></span>

* <span data-ttu-id="b5cc0-189">Delta gibt keine der folgenden „DriveItem“-Eigenschaften zurück:</span><span class="sxs-lookup"><span data-stu-id="b5cc0-189">Delta will not return the following DriveItem properties:</span></span>

* <span data-ttu-id="b5cc0-190">**cTag**</span><span class="sxs-lookup"><span data-stu-id="b5cc0-190">**cTag**</span></span>
* <span data-ttu-id="b5cc0-191">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="b5cc0-191">**lastModifiedBy**</span></span>
* <span data-ttu-id="b5cc0-192">**size**</span><span class="sxs-lookup"><span data-stu-id="b5cc0-192">**size**</span></span>

## <a name="error-responses"></a><span data-ttu-id="b5cc0-193">Fehlerantworten</span><span class="sxs-lookup"><span data-stu-id="b5cc0-193">Error responses</span></span>

<span data-ttu-id="b5cc0-194">Zusätzlich zu den vorstehend beschriebenen Fehlern bei der erneuten Synchronisierung finden Sie unter [Fehlerantworten] [ error-response] weitere Informationen darüber, wie Fehler zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="b5cc0-194">In addition to the resync errors detailed above, see [Error Responses][error-response] for details about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Sync changes from the service to your client state.",
  "keywords": "sync,delta,changes,$delta",
  "section": "documentation",
  "tocPath": "Items/Sync changes",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-delta.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
