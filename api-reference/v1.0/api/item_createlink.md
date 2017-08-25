# <a name="create-a-sharing-link-for-a-driveitem"></a><span data-ttu-id="4f089-101">Freigabelink für ein DriveItem erstellen</span><span class="sxs-lookup"><span data-stu-id="4f089-101">Create a sharing link for a DriveItem</span></span>

<span data-ttu-id="4f089-102">Sie können die Aktion **createLink** verwenden, um ein [DriveItem](../resources/driveitem.md) über einen Freigabelink freizugeben.</span><span class="sxs-lookup"><span data-stu-id="4f089-102">You can use **createLink** action to share a [DriveItem](../resources/driveitem.md) via a sharing link.</span></span>

<span data-ttu-id="4f089-p101">Die Aktion **createLink** erstellt einen neuen Freigabelink, falls der angegebene Linktyp für die aufrufende Anwendung noch nicht existiert. Existiert für die App bereits ein Freigabelink des angegebenen Typs, wird dieser bereits vorhandene Freigabelink zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4f089-p101">The **createLink** action will create a new sharing link if the specified link type doesn't already exist for the calling application. If a sharing link of the specified type already exists for the app, the existing sharing link will be returned.</span></span>

<span data-ttu-id="4f089-105">Ressourcen des Typs „DriveItem“ erben Berechtigungen von ihren Vorgängern.</span><span class="sxs-lookup"><span data-stu-id="4f089-105">DriveItem resources inherit permissions from their ancestors.</span></span>

## <a name="permissions"></a><span data-ttu-id="4f089-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4f089-106">Permissions</span></span>
<span data-ttu-id="4f089-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4f089-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4f089-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4f089-109">Permission type</span></span>      | <span data-ttu-id="4f089-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4f089-110">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="4f089-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4f089-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4f089-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f089-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    | 
|<span data-ttu-id="4f089-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4f089-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f089-114">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f089-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    | 
|<span data-ttu-id="4f089-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4f089-115">Application</span></span> | <span data-ttu-id="4f089-116">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f089-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="4f089-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4f089-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{item-id}/createLink
POST /me/drive/root:/{item-path}:/createLink
POST /groups/{group-id}/drive/items/{item-id}/createLink
POST /drives/{drive-id}/items/{item-id}/createLink
```

## <a name="request-body"></a><span data-ttu-id="4f089-118">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4f089-118">Request body</span></span>
<span data-ttu-id="4f089-p103">Der Anforderungstext definiert den Typ des Freigabelinks, nach dem die Anwendung sucht. Die Anforderung sollte ein JSON-Objekt mit dieser Eigenschaft sein.</span><span class="sxs-lookup"><span data-stu-id="4f089-p103">The body of the request defines the type of sharing link your application is looking for. The request should be a JSON object with this property.</span></span>

| <span data-ttu-id="4f089-121">Name</span><span class="sxs-lookup"><span data-stu-id="4f089-121">Name</span></span>      | <span data-ttu-id="4f089-122">Typ</span><span class="sxs-lookup"><span data-stu-id="4f089-122">Type</span></span>   | <span data-ttu-id="4f089-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4f089-123">Description</span></span>                                                                  |
|:----------|:-------|:-----------------------------------------------------------------------------|
| <span data-ttu-id="4f089-124">**type**</span><span class="sxs-lookup"><span data-stu-id="4f089-124">**type**</span></span>  | <span data-ttu-id="4f089-125">string</span><span class="sxs-lookup"><span data-stu-id="4f089-125">string</span></span> | <span data-ttu-id="4f089-p104">Der Typ Freigabelink, der erstellt werden soll. Möglich sind `view`, `edit` oder `embed`.</span><span class="sxs-lookup"><span data-stu-id="4f089-p104">The type of sharing link to create. Either `view`, `edit`, or `embed`.</span></span>       |
| <span data-ttu-id="4f089-128">**scope**</span><span class="sxs-lookup"><span data-stu-id="4f089-128">**scope**</span></span> | <span data-ttu-id="4f089-129">string</span><span class="sxs-lookup"><span data-stu-id="4f089-129">string</span></span> | <span data-ttu-id="4f089-p105">Der Bereich des zu erstellenden Links. Möglich sind `anonymous` oder `organization`. Optional.</span><span class="sxs-lookup"><span data-stu-id="4f089-p105">The scope of link to create. Either `anonymous` or `organization`. Optional.</span></span> |

## <a name="link-types"></a><span data-ttu-id="4f089-133">Linktypen</span><span class="sxs-lookup"><span data-stu-id="4f089-133">Link types</span></span>
<span data-ttu-id="4f089-134">Für den Parameter **type** sind die folgenden Werte zulässig:</span><span class="sxs-lookup"><span data-stu-id="4f089-134">The following values are allowed for the **type** parameter.</span></span>

| <span data-ttu-id="4f089-135">Typwert</span><span class="sxs-lookup"><span data-stu-id="4f089-135">Type value</span></span> | <span data-ttu-id="4f089-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4f089-136">Description</span></span>                                                                                  |
|:-----------|:---------------------------------------------------------------------------------------------|
| `view`     | <span data-ttu-id="4f089-137">Erstellt einen schreibgeschützten Link zum Element.</span><span class="sxs-lookup"><span data-stu-id="4f089-137">Creates a read-only link to the item.</span></span>                                                        |
| `edit`     | <span data-ttu-id="4f089-138">Erstellt einen Lese-/Schreiblink zum Element.</span><span class="sxs-lookup"><span data-stu-id="4f089-138">Creates a read-write link to the item.</span></span>                                                       |
| `embed`    | <span data-ttu-id="4f089-p106">Erstellt einen einbettbaren Link zum Element. Diese Option ist nur für OneDrive Personal verfügbar.</span><span class="sxs-lookup"><span data-stu-id="4f089-p106">Creates an embeddable link to the item. This option is only available for OneDrive Personal.</span></span> |

## <a name="scope-types"></a><span data-ttu-id="4f089-141">Bereichstypen</span><span class="sxs-lookup"><span data-stu-id="4f089-141">Scope types</span></span>
<span data-ttu-id="4f089-p107">Für den Parameter **scope** sind die nachfolgend aufgeführten Werte zulässig. Der Parameter ist optional. Wird der Parameter **scope** nicht festgelegt, wird von den verfügbaren Links derjenige mit den meisten Berechtigungen erstellt.</span><span class="sxs-lookup"><span data-stu-id="4f089-p107">The following values are allowed for the **scope** parameter. This is an optional parameter. If the **scope** parameter is not specified, the most permissive link available will be created.</span></span>

| <span data-ttu-id="4f089-145">Typwert</span><span class="sxs-lookup"><span data-stu-id="4f089-145">Type value</span></span>     | <span data-ttu-id="4f089-146">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4f089-146">Description</span></span>                                                                                                                   |
|:---------------|:------------------------------------------------------------------------------------------------------------------------------|
| `anonymous`    | <span data-ttu-id="4f089-p108">Erstellt einen Link zum Element, auf den jedermann zugreifen kann. Anonyme Links können vom Mandantenadministrator deaktiviert werden.</span><span class="sxs-lookup"><span data-stu-id="4f089-p108">Creates a link to the item accessible to anyone. Anonymous links may be disabled by the tenant administrator.</span></span>                 |
| `organization` | <span data-ttu-id="4f089-p109">Erstellt einen Link zum Element, auf den innerhalb einer Organisation zugegriffen werden kann. Der Linkbereich „organization“ ist nicht für OneDrive Personal verfügbar.</span><span class="sxs-lookup"><span data-stu-id="4f089-p109">Creates a link to the item accessible within an organization. Organization link scope is not available for OneDrive Personal.</span></span> |

## <a name="response"></a><span data-ttu-id="4f089-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="4f089-151">Response</span></span>

<span data-ttu-id="4f089-152">Bei Erfolg gibt diese Methode eine einzige Ressource des Typs [Permission](../resources/permission.md) im Antworttext zurück. Dabei handelt es sich um die Berechtigung für den angeforderten Freigabelink.</span><span class="sxs-lookup"><span data-stu-id="4f089-152">If successful, this method returns a single [Permission](../resources/permission.md) resource in the response body that represents the requested sharing link permission.</span></span>

<span data-ttu-id="4f089-153">Der Dienst prüft zuerst die aktuellen Berechtigungen, um festzustellen, ob für die aufrufende Anwendung bereits eine Berechtigung mit demselben Wert für den Parameter **type** existiert.</span><span class="sxs-lookup"><span data-stu-id="4f089-153">The service will first look at the current permissions and check if one already exists that has the same **type** for the calling application.</span></span>

<span data-ttu-id="4f089-154">Wird ein neuer Freigabelink für das Element erstellt, lautet die Antwort `201 Created`. Wird ein bereits vorhandener Link zurückgegeben, lautet die Antwort `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="4f089-154">The response will be `201 Created` if a new sharing link is created for the item or `200 OK` if an existing link is returned.</span></span>

## <a name="example"></a><span data-ttu-id="4f089-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4f089-155">Example</span></span>
<span data-ttu-id="4f089-156">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="4f089-156">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="4f089-157">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4f089-157">Request</span></span>
<span data-ttu-id="4f089-158">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4f089-158">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "item_createlink"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root:/{item-path}:/createLink
Content-type: application/json

{
  "type": "view",
  "scope": "anonymous"
}
```

##### <a name="response"></a><span data-ttu-id="4f089-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="4f089-159">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission" } -->
```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["write"],
  "link": {
    "type": "view",
    "scope": "anonymous",
    "webUrl": "https://1drv.ms/A6913278E564460AA616C71B28AD6EB6",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```

## <a name="creating-company-sharable-links"></a><span data-ttu-id="4f089-160">Erstellen von nur innerhalb eines Unternehmens freigegebenen Links</span><span class="sxs-lookup"><span data-stu-id="4f089-160">Creating company sharable links</span></span>

<span data-ttu-id="4f089-p110">OneDrive for Business und SharePoint unterstützen Links, die nur innerhalb eines Unternehmens freigegeben sind. Diese ähneln anonymen Links, funktionieren aber nur für Mitglieder des Mandanten, der Besitzer ist. Verwenden Sie den Parameter **scope** mit dem Wert `organization`, um einen Link zu erstellen, der nur innerhalb eines Unternehmens freigegeben ist.</span><span class="sxs-lookup"><span data-stu-id="4f089-p110">OneDrive for Business and SharePoint support company sharable links. These are similar to anonymous links, except they only work for members of the owning tenant. To create a company sharable link, use the **scope** parameter with a value of `organization`.</span></span>

## <a name="http-request"></a><span data-ttu-id="4f089-164">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4f089-164">HTTP request</span></span>

<!-- { "blockType": "request", "name": "create-link-scoped", "scopes": "files.readwrite service.sharepoint" } -->
```
POST https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "edit",
  "scope": "organization"
}
```

## <a name="http-response"></a><span data-ttu-id="4f089-165">HTTP-Antwort</span><span class="sxs-lookup"><span data-stu-id="4f089-165">HTTP response</span></span>

<span data-ttu-id="4f089-166">Wird ein neuer Freigabelink für das Element erstellt, lautet die Antwort `201 Created`. Wird ein bereits vorhandener Link zurückgegeben, lautet die Antwort `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="4f089-166">The response will be `201 Created` if a new sharing link is created for the item or `200 OK` if an existing link is returned.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission" } -->
```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["write"],
  "link": {
    "type": "view",
    "scope": "organization",
    "webUrl": "https://contoso-my.sharepoint.com/personal/ellen_contoso_com/...",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```

## <a name="embeddable-links"></a><span data-ttu-id="4f089-167">Einbettbare Links</span><span class="sxs-lookup"><span data-stu-id="4f089-167">Embeddable links</span></span>

<span data-ttu-id="4f089-p111">Bei Verwendung des Linktyps `embed` kann der zurückgegebene Wert für „webUrl“ in ein HTML-Element des Typs `<iframe>` eingebettet werden. Wird ein Einbettungslink erstellt, enthält die Eigenschaft `webHtml` den HTML-Code für einen `<iframe>`, der den Inhalt hostet.</span><span class="sxs-lookup"><span data-stu-id="4f089-p111">When using the `embed` link type, the webUrl returned can be embedded in an `<iframe>` HTML element. When an embed link is created the `webHtml` property contains the HTML code for an `<iframe>` to host the content.</span></span>

<span data-ttu-id="4f089-170">**Hinweis:** Einbettungslinks werden nur für Ressourcen des Typs [Drive](../resources/drive.md) unterstützt, bei denen für **driveType** `personal` festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="4f089-170">**Note:** Embed links are only supported in [Drives](../resources/drive.md) where the **driveType** is `personal`.</span></span>

## <a name="remarks"></a><span data-ttu-id="4f089-171">Hinweise</span><span class="sxs-lookup"><span data-stu-id="4f089-171">Remarks</span></span>

* <span data-ttu-id="4f089-172">Mit dieser Aktion erstellte Links laufen nicht ab, es sei denn, für die Organisation wird eine Standardablaufrichtlinie erzwungen.</span><span class="sxs-lookup"><span data-stu-id="4f089-172">Links created using this action do not expire unless a default expiration policy is enforced for the organization.</span></span>
* <span data-ttu-id="4f089-173">Links sind in den Freigabeberechtigungen für das Element sichtbar und können von einem Besitzer des Elements entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="4f089-173">Links are visible in the sharing permissions for the item and can be removed by an owner of the item.</span></span>
* <span data-ttu-id="4f089-174">Links zeigen immer auf die aktuelle Version eines Elements, es sei denn, das Element ist ausgecheckt (nur SharePoint).</span><span class="sxs-lookup"><span data-stu-id="4f089-174">Links always point to the current version of a item unless the item is checked out (SharePoint only).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "item: createLink",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Create sharing link"
} -->
