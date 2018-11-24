# <a name="driveitem-preview"></a><span data-ttu-id="f2d0d-101">DriveItem: Vorschau</span><span class="sxs-lookup"><span data-stu-id="f2d0d-101">driveItem: preview</span></span>

<span data-ttu-id="f2d0d-102">Diese Aktion können Sie kurzlebige eingebettet werden URLs für ein Element abrufen, um eine temporäre Vorschau zu rendern.</span><span class="sxs-lookup"><span data-stu-id="f2d0d-102">This action allows you to obtain short-lived embeddable URLs for an item in order to render a temporary preview.</span></span>

<span data-ttu-id="f2d0d-103">Wenn Sie Links mit langer Lebensdauer eingebettet werden abrufen möchten, verwenden Sie stattdessen die [CreateLink][] API.</span><span class="sxs-lookup"><span data-stu-id="f2d0d-103">If you want to obtain long-lived embeddable links, use the [createLink][] API instead.</span></span>

> <span data-ttu-id="f2d0d-104">**Hinweis:** Die **Preview** -Aktion ist derzeit nur auf SharePoint und OneDrive für Unternehmen verfügbar.</span><span class="sxs-lookup"><span data-stu-id="f2d0d-104">**Note:** The **preview** action is currently only available on SharePoint and OneDrive for Business.</span></span>

[createLink]: driveItem_createLink.md

## <a name="permissions"></a><span data-ttu-id="f2d0d-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f2d0d-106">Permissions</span></span>

<span data-ttu-id="f2d0d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f2d0d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="f2d0d-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f2d0d-109">Permission type</span></span>                        | <span data-ttu-id="f2d0d-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f2d0d-110">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="f2d0d-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f2d0d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f2d0d-112">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2d0d-112">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="f2d0d-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f2d0d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2d0d-114">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2d0d-114">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="f2d0d-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f2d0d-115">Application</span></span>                            | <span data-ttu-id="f2d0d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f2d0d-116">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="f2d0d-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f2d0d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/preview
POST /groups/{groupId}/drive/items/{itemId}/preview
POST /me/drive/items/{itemId}/preview
POST /sites/{siteId}/drive/items/{itemId}/preview
POST /users/{userId}/drive/items/{itemId}/preview
POST /shares/{shareId}/driveItem/preview
```

## <a name="request-body"></a><span data-ttu-id="f2d0d-118">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f2d0d-118">Request body</span></span>

<span data-ttu-id="f2d0d-119">Der Text der Anforderung definiert Eigenschaften der embeddable URL Ihrer Anwendung anfordert.</span><span class="sxs-lookup"><span data-stu-id="f2d0d-119">The body of the request defines properties of the embeddable URL your application is requesting.</span></span>
<span data-ttu-id="f2d0d-120">Bei der Anforderung sollte es sich um ein JSON-Objekt mit folgenden Eigenschaften handeln:</span><span class="sxs-lookup"><span data-stu-id="f2d0d-120">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="f2d0d-121">Name</span><span class="sxs-lookup"><span data-stu-id="f2d0d-121">Name</span></span>      |  <span data-ttu-id="f2d0d-122">Typ</span><span class="sxs-lookup"><span data-stu-id="f2d0d-122">Type</span></span>         | <span data-ttu-id="f2d0d-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f2d0d-123">Description</span></span>
|:------------|:--------------|:-----------------------------------------------
| <span data-ttu-id="f2d0d-124">page</span><span class="sxs-lookup"><span data-stu-id="f2d0d-124">page</span></span>        | <span data-ttu-id="f2d0d-125">Zeichenfolge/eine einzelne Nummer</span><span class="sxs-lookup"><span data-stu-id="f2d0d-125">string/number</span></span> | <span data-ttu-id="f2d0d-126">Optional.</span><span class="sxs-lookup"><span data-stu-id="f2d0d-126">Optional.</span></span> <span data-ttu-id="f2d0d-127">Seitenzahl des Dokuments an, falls zutreffend zu starten.</span><span class="sxs-lookup"><span data-stu-id="f2d0d-127">Page number of document to start at, if applicable.</span></span> <span data-ttu-id="f2d0d-128">Als Zeichenfolge für die zukünftige Verwendung Fällen um Dateitypen wie ZIP angegeben.</span><span class="sxs-lookup"><span data-stu-id="f2d0d-128">Specified as string for future use cases around file types such as ZIP.</span></span>
| <span data-ttu-id="f2d0d-129">Zoom</span><span class="sxs-lookup"><span data-stu-id="f2d0d-129">zoom</span></span>        | <span data-ttu-id="f2d0d-130">number</span><span class="sxs-lookup"><span data-stu-id="f2d0d-130">number</span></span>        | <span data-ttu-id="f2d0d-131">Optional.</span><span class="sxs-lookup"><span data-stu-id="f2d0d-131">Optional.</span></span> <span data-ttu-id="f2d0d-132">Zoom-Wert auf, falls zutreffend.</span><span class="sxs-lookup"><span data-stu-id="f2d0d-132">Zoom level to start at, if applicable.</span></span>

## <a name="response"></a><span data-ttu-id="f2d0d-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="f2d0d-133">Response</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

<span data-ttu-id="f2d0d-134">Die Antwort wird ein JSON-Objekt mit den folgenden Eigenschaften werden:</span><span class="sxs-lookup"><span data-stu-id="f2d0d-134">The response will be a JSON object containing the following properties:</span></span>

| <span data-ttu-id="f2d0d-135">Name</span><span class="sxs-lookup"><span data-stu-id="f2d0d-135">Name</span></span>           | <span data-ttu-id="f2d0d-136">Typ</span><span class="sxs-lookup"><span data-stu-id="f2d0d-136">Type</span></span>   | <span data-ttu-id="f2d0d-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f2d0d-137">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="f2d0d-138">getUrl</span><span class="sxs-lookup"><span data-stu-id="f2d0d-138">getUrl</span></span>         | <span data-ttu-id="f2d0d-139">string</span><span class="sxs-lookup"><span data-stu-id="f2d0d-139">string</span></span> | <span data-ttu-id="f2d0d-140">URL für das Einbetten von mit HTTP-GET (Iframes usw.) geeignet</span><span class="sxs-lookup"><span data-stu-id="f2d0d-140">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="f2d0d-141">postUrl</span><span class="sxs-lookup"><span data-stu-id="f2d0d-141">postUrl</span></span>        | <span data-ttu-id="f2d0d-142">string</span><span class="sxs-lookup"><span data-stu-id="f2d0d-142">string</span></span> | <span data-ttu-id="f2d0d-143">URL für das Einbetten von mithilfe von HTTP POST geeignet (bilden, JS, usw..)</span><span class="sxs-lookup"><span data-stu-id="f2d0d-143">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="f2d0d-144">postParameters</span><span class="sxs-lookup"><span data-stu-id="f2d0d-144">postParameters</span></span> | <span data-ttu-id="f2d0d-145">string</span><span class="sxs-lookup"><span data-stu-id="f2d0d-145">string</span></span> | <span data-ttu-id="f2d0d-146">POST-Parameter einschließen, wenn PostUrl verwenden</span><span class="sxs-lookup"><span data-stu-id="f2d0d-146">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="f2d0d-147">GetUrl, PostUrl oder beide möglicherweise abhängig vom aktuellen Status des Embed-Unterstützung für den angegebenen Optionen zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f2d0d-147">Either getUrl, postUrl, or both might be returned depending on the current state of embed support for the specified options.</span></span>

<span data-ttu-id="f2d0d-148">PostParameters ist eine Zeichenfolge, die als formatiert `application/x-www-form-urlencoded`, und wenn Ausführen von POST an den PostUrl Content-Type entsprechend festgelegt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="f2d0d-148">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="f2d0d-149">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="f2d0d-149">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="pagezoom"></a><span data-ttu-id="f2d0d-150">Seite/zoom</span><span class="sxs-lookup"><span data-stu-id="f2d0d-150">Page/zoom</span></span>

<span data-ttu-id="f2d0d-151">Die Optionen 'zoom' und 'Seite' möglicherweise nicht für alle Preview apps verfügbar, jedoch werden angewendet werden soll, wenn die app Preview unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f2d0d-151">The 'page' and 'zoom' options may not be available for all preview apps, but will be applied if the preview app supports it.</span></span>
