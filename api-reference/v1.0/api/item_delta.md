# <a name="track-changes-for-a-drive"></a><span data-ttu-id="04400-101">Laufwerksänderungen nachverfolgen</span><span class="sxs-lookup"><span data-stu-id="04400-101">Track changes for a Drive</span></span>

<span data-ttu-id="04400-102">Mit dieser Methode kann Ihre App Änderungen nachverfolgen, die im Laufe der Zeit an Laufwerken sowie deren untergeordneten Elementen vorgenommen werden.</span><span class="sxs-lookup"><span data-stu-id="04400-102">This method allows your app to track changes to a drive and its children over time.</span></span>

<span data-ttu-id="04400-p101">Die App ruft zunächst `delta` ohne Parameter auf. Der Dienst startet dann eine Enumeration der Laufwerkshierarchie und gibt Seiten mit Elementen sowie entweder einen `@odata.nextLink` oder einen `@odata.deltaLink` zurück, wie unten beschrieben. Die App sollte die Aufrufe solange mit dem `@odata.nextLink` fortführen, bis kein `@odata.nextLink` mehr zurückgegeben wird oder bis eine Antwort mit einem leeren Satz an Änderungen zurückgegeben wird.</span><span class="sxs-lookup"><span data-stu-id="04400-p101">Your app begins by calling `delta` without any parameters. The service starts enumerating the drive's hierarchy, returning pages of items and either an `@odata.nextLink` or an `@odata.deltaLink`, as described below. Your app should continue calling with the `@odata.nextLink` until you no longer see an `@odata.nextLink` returned, or you see a response with an empty set of changes.</span></span>

<span data-ttu-id="04400-p102">Sobald alle Änderungen empfangen wurden, können Sie sie auf den lokalen Zustand anwenden. Wenn Sie zu einem späteren Zeitpunkt nochmals auf Änderungen prüfen möchten, rufen Sie erneut `delta` auf, mit dem `@odata.deltaLink` aus der vorherigen Antwort.</span><span class="sxs-lookup"><span data-stu-id="04400-p102">After you have finished receiving all the changes, you may apply them to your local state. To check for changes in the future, call `delta` again with the `@odata.deltaLink` from the previous response.</span></span>

<span data-ttu-id="04400-p103">Gelöschte Elemente werden mit dem [`deleted`Facet](../resources/deleted.md) zurückgegeben. Elemente, für die diese Eigenschaft gesetzt ist, sollten Sie aus Ihrem lokalen Zustand entfernen.</span><span class="sxs-lookup"><span data-stu-id="04400-p103">Deleted items are returned with the [`deleted` facet](../resources/deleted.md). Items with this property set should be removed from your local state.</span></span> 

<span data-ttu-id="04400-110">**Hinweis:** Löschen Sie Ordner nur lokal, wenn sie nach der Synchronisierung aller Änderungen leer sind.</span><span class="sxs-lookup"><span data-stu-id="04400-110">**Note:** you should only delete a folder locally if it is empty after syncing all the changes.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="04400-111">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="04400-111">Prerequisites</span></span>
<span data-ttu-id="04400-112">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen:</span><span class="sxs-lookup"><span data-stu-id="04400-112">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="04400-113">Files.Read</span><span class="sxs-lookup"><span data-stu-id="04400-113">Files.Read</span></span>
* <span data-ttu-id="04400-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04400-114">Files.ReadWrite</span></span>
* <span data-ttu-id="04400-115">Files.Read.All</span><span class="sxs-lookup"><span data-stu-id="04400-115">Files.Read.All</span></span>
* <span data-ttu-id="04400-116">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04400-116">Files.ReadWrite.All</span></span>
* <span data-ttu-id="04400-117">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="04400-117">Sites.Read.All</span></span>
* <span data-ttu-id="04400-118">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04400-118">Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="04400-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="04400-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root/delta
GET /drives/{drive-id}/root/delta
GET /groups/{group-id}/drive/root/delta
```

## <a name="optional-query-parameters"></a><span data-ttu-id="04400-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="04400-120">Optional query parameters</span></span>
<span data-ttu-id="04400-121">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) `$select`, `$expand` und `$top` zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="04400-121">This method supports `$select`, `$expand`, and `$top` [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to customize the response.</span></span>

## <a name="request-body"></a><span data-ttu-id="04400-122">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="04400-122">Request body</span></span>
<span data-ttu-id="04400-123">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="04400-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="04400-124">Antwort</span><span class="sxs-lookup"><span data-stu-id="04400-124">Response</span></span>

<span data-ttu-id="04400-125">Bei Erfolg gibt diese Methode den Antwortcode `200 OK` und eine Sammlung von Ressourcen des Typs [DriveItem](../resources/driveitem.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="04400-125">If successful, this method returns a `200 OK` response code and a collection of [DriveItem](../resources/driveitem.md) resources in the response body.</span></span>

<span data-ttu-id="04400-126">Zusätzlich zu der Sammlung von DriveItems enthält die Antwort außerdem eine der folgenden Eigenschaften:</span><span class="sxs-lookup"><span data-stu-id="04400-126">In addition to the collection of DriveItems, the response will also include one of the following properties:</span></span>

| <span data-ttu-id="04400-127">Name</span><span class="sxs-lookup"><span data-stu-id="04400-127">Name</span></span>                 | <span data-ttu-id="04400-128">Wert</span><span class="sxs-lookup"><span data-stu-id="04400-128">Value</span></span>  | <span data-ttu-id="04400-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="04400-129">Description</span></span>                                                                                                                                      |
|:---------------------|:-------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="04400-130">**@odata.nextLink**</span><span class="sxs-lookup"><span data-stu-id="04400-130">**@odata.nextLink**</span></span>  | <span data-ttu-id="04400-131">url</span><span class="sxs-lookup"><span data-stu-id="04400-131">url</span></span>    | <span data-ttu-id="04400-132">Eine URL zum Abrufen der nächsten verfügbaren Seite von Änderungen, sofern weitere Änderungen im aktuellen Satz vorhanden sind</span><span class="sxs-lookup"><span data-stu-id="04400-132">A URL to retrieve the next available page of changes, if there are additional changes in the current set.</span></span>                                        |
| <span data-ttu-id="04400-133">**@odata.deltaLink**</span><span class="sxs-lookup"><span data-stu-id="04400-133">**@odata.deltaLink**</span></span> | <span data-ttu-id="04400-134">url</span><span class="sxs-lookup"><span data-stu-id="04400-134">url</span></span>    | <span data-ttu-id="04400-p104">Eine URL, die anstelle eines **@odata.nextLink** zurückgegeben wird, sobald alle aktuellen Änderungen zurückgegeben wurden. Sie wird verwendet, um zu einem späteren Zeitpunkt den nächsten Satz von Änderungen zu lesen.</span><span class="sxs-lookup"><span data-stu-id="04400-p104">A URL returned instead of **@odata.nextLink** after all current changes have been returned. Used to read the next set of changes in the future.</span></span>  |


## <a name="example-initial-request"></a><span data-ttu-id="04400-137">Beispiel (ursprüngliche Anforderung)</span><span class="sxs-lookup"><span data-stu-id="04400-137">Example (Initial Request)</span></span>
<span data-ttu-id="04400-138">Hier sehen Sie ein Beispiel für einen Aufruf dieser API zur Ermittlung Ihres lokalen Zustands.</span><span class="sxs-lookup"><span data-stu-id="04400-138">Here is an example of how to call this API to establish your local state.</span></span>

##### <a name="request"></a><span data-ttu-id="04400-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="04400-139">Request</span></span>
<span data-ttu-id="04400-140">Unten ein Beispiel für eine ursprüngliche Anforderung:</span><span class="sxs-lookup"><span data-stu-id="04400-140">Here is an example of the initial request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_item_delta"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/delta
```

##### <a name="response"></a><span data-ttu-id="04400-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="04400-141">Response</span></span>
<span data-ttu-id="04400-142">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="04400-142">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem",
  "isCollection": true
} -->
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

<span data-ttu-id="04400-p105">Diese Antwort enthält die erste Seite von Änderungen. Die Eigenschaft **@odata.nextLink** gibt an, dass im aktuellen Satz von Elementen weitere Elemente verfügbar sind. Die App sollte nun solange den URL-Wert von **@odata.nextLink** anfordern, bis alle Seiten von Elementen abgerufen wurden.</span><span class="sxs-lookup"><span data-stu-id="04400-p105">This response includes the first page of changes, and the **@odata.nextLink** property indicates that there are more items available in the current set of items. Your app should continue to request the URL value of **@odata.nextLink** until all pages of items have been retrieved.</span></span>

## <a name="example-last-page-in-a-set"></a><span data-ttu-id="04400-145">Beispiel (letzte Seite in einem Satz)</span><span class="sxs-lookup"><span data-stu-id="04400-145">Example (Last page in a set)</span></span>
<span data-ttu-id="04400-146">Unten sehen Sie ein Beispiel für einen Aufruf dieser API zur Aktualisierung Ihres lokalen Zustands.</span><span class="sxs-lookup"><span data-stu-id="04400-146">Here is an example of how to call this API to update your local state.</span></span>

##### <a name="request"></a><span data-ttu-id="04400-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="04400-147">Request</span></span>
<span data-ttu-id="04400-148">Hier sehen Sie ein Beispiel für eine Anforderung nach der ursprünglichen Anforderung:</span><span class="sxs-lookup"><span data-stu-id="04400-148">Here is an example request after the initial request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_item_delta"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/delta(token='1230919asd190410jlka')
```

##### <a name="response"></a><span data-ttu-id="04400-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="04400-149">Response</span></span>
<span data-ttu-id="04400-150">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="04400-150">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem",
  "isCollection": true
} -->
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

<span data-ttu-id="04400-151">Diese Antwort gibt an, dass im Zeitraum zwischen der ursprünglichen Anforderung und dieser Anforderung zur Aktualisierung des lokalen Zustands das Element `folder2` gelöscht wurde und das Element `file.txt` entweder hinzugefügt oder geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="04400-151">This response indicates that the item named `folder2` was deleted and the item `file.txt` was either added or modified between the initial request and this request to update the local state.</span></span>

<span data-ttu-id="04400-152">Die letzte Seite mit Elementen enthält die Eigenschaft **@odata.deltaLink**. Sie spezifiziert die URL, über die zu einem späteren Zeitpunkt Änderungen abgerufen werden können, die bis dahin an dem jetzt aktuellen Elementsatz vorgenommen wurden.</span><span class="sxs-lookup"><span data-stu-id="04400-152">The final page of items will include the **@odata.deltaLink** property, which provides the URL that can be used later to retrieve changes since the current set of items.</span></span>

## <a name="remarks"></a><span data-ttu-id="04400-153">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="04400-153">Remarks</span></span>

* <span data-ttu-id="04400-p106">Der „delta“-Feed zeigt den aktuellen Zustand jedes Elements, nicht jede Änderung. Wenn ein Element beispielsweise zweimal umbenannt wurde, wird es nur einmal angezeigt, mit seinem neuesten Namen.</span><span class="sxs-lookup"><span data-stu-id="04400-p106">The delta feed shows the latest state for each item, not each change. If an item were renamed twice, it would only show up once, with its latest name.</span></span>
* <span data-ttu-id="04400-p107">Ein Element kann mehrmals in einem delta-Feed aufgeführt werden, aus jeweils unterschiedlichen Gründen. Verwenden Sie das letzte Vorkommen in der Auflistung.</span><span class="sxs-lookup"><span data-stu-id="04400-p107">The same item may appear more than once in a delta feed, for various reasons. You should use the last occurrence you see.</span></span>
* <span data-ttu-id="04400-p108">Die Eigenschaft `parentReference` von Elementen enthält keinen Wert für **path**. Der Grund: Wenn ein Ordner umbenannt wird, gibt **delta** keine Nachfolger dieses Ordners zurück. **Bei Verwendung von „delta“ sollten Sie Elemente immer anhand ihrer ID nachverfolgen.**</span><span class="sxs-lookup"><span data-stu-id="04400-p108">The `parentReference` property on items will not include a value for **path**. This occurs because renaming a folder does not result in any descendants of the folder being returned from **delta**. **When using delta you should always track items by id**.</span></span>

<span data-ttu-id="04400-p109">Es kann passieren, dass der Dienst für ein Token keine Änderungsliste zurückgeben kann. (Das ist beispielsweise der Fall, wenn ein Client nach einer längeren Verbindungsunterbrechung versucht, ein altes Token wiederzuverwenden, oder wenn sich der Zustand eines Servers geändert hat und daher ein neues Token erforderlich ist.) In solchen Fällen gibt der Dienst einen Fehler des Typs `HTTP 410 Gone` zurück. Die Fehlerantwort enthält einen der unten aufgeführten Fehlercodes und einen Header `Location` mit einem neuen „nextLink“, der eine vollständig neue „delta“-Enumeration startet. Vergleichen Sie nach Abschluss der vollständigen Enumeration die zurückgegebenen Elemente mit Ihrem lokalen Zustand, und befolgen Sie diese Anweisungen:</span><span class="sxs-lookup"><span data-stu-id="04400-p109">There may be cases when the service can't provide a list of changes for a given token (for example, if a client tries to reuse an old token after being disconnected for a long time, or if server state has changed and a new token is required). In these cases the service will return an `HTTP 410 Gone` error with an error response containing one of the error codes below, and a `Location` header containing a new nextLink that starts a fresh delta enumeration from scratch. After finishing the full enumeration, compare the returned items with your local state and follow these instructions.</span></span>

| <span data-ttu-id="04400-164">Fehlertyp</span><span class="sxs-lookup"><span data-stu-id="04400-164">Error Type</span></span>                       | <span data-ttu-id="04400-165">Anweisungen</span><span class="sxs-lookup"><span data-stu-id="04400-165">Instructions</span></span>                                                                                                                                                                                                                    |
|:---------------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `resyncChangesApplyDifferences`  | <span data-ttu-id="04400-p110">Ersetzen Sie alle lokalen Elemente durch die Serverversion (einschließlich gelöschter Elemente), wenn Sie sicher sind, dass der Dienst bei der letzten Synchronisierung mit den lokalen Änderungen aktualisiert wurde. Laden Sie alle lokalen Änderungen hoch, die dem Server noch nicht bekannt sind.</span><span class="sxs-lookup"><span data-stu-id="04400-p110">Replace any local items with the server's version (including deletes) if you're sure that the service was up to date with your local changes when you last sync'd. Upload any local changes that the server doesn't know about.</span></span> |
| `resyncChangesUploadDifferences` | <span data-ttu-id="04400-168">Laden Sie alle lokalen Elemente hoch, die der Dienst nicht zurückgegeben hat, und laden Sie alle Dateien hoch, die sich von der Version auf dem Server unterscheiden (wobei Sie beide Kopien beibehalten, wenn Sie nicht sicher sind, welche die aktuelle ist).</span><span class="sxs-lookup"><span data-stu-id="04400-168">Upload any local items that the service did not return, and upload any files that differ from the server's version (keeping both copies if you're not sure which one is more up-to-date).</span></span>                                       |


<span data-ttu-id="04400-p111">In OneDrive for Business und SharePoint wird `delta` nur für den Ordner `root` unterstützt, für andere Ordner jedoch nicht. Zudem gibt es keine der folgenden „DriveItem“-Eigenschaften zurück:</span><span class="sxs-lookup"><span data-stu-id="04400-p111">In OneDrive for Business and SharePoint, `delta` is only supported on the `root` folder, not on other folders. It also will not return the following DriveItem properties:</span></span>

* <span data-ttu-id="04400-171">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="04400-171">**createdBy**</span></span>
* <span data-ttu-id="04400-172">**cTag**</span><span class="sxs-lookup"><span data-stu-id="04400-172">**cTag**</span></span>
* <span data-ttu-id="04400-173">**eTag**</span><span class="sxs-lookup"><span data-stu-id="04400-173">**etag**</span></span>
* <span data-ttu-id="04400-174">**fileSystemInfo**</span><span class="sxs-lookup"><span data-stu-id="04400-174">**fileSystemInfo**</span></span>
* <span data-ttu-id="04400-175">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="04400-175">**lastModifiedBy**</span></span>
* <span data-ttu-id="04400-176">**parentReference**</span><span class="sxs-lookup"><span data-stu-id="04400-176">**parentReference**</span></span>
* <span data-ttu-id="04400-177">**size**</span><span class="sxs-lookup"><span data-stu-id="04400-177">**size**</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "Get item delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
