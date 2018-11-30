---
title: 'DriveItem: Vorschau'
description: Diese Aktion können Sie kurzlebige eingebettet werden URLs für ein Element abrufen, um eine temporäre Vorschau zu rendern.
ms.openlocfilehash: 51432e53d6986e680dda8508ef0069c7713b3a9d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059598"
---
# <a name="driveitem-preview"></a><span data-ttu-id="25e89-103">DriveItem: Vorschau</span><span class="sxs-lookup"><span data-stu-id="25e89-103">driveItem: preview</span></span>

> <span data-ttu-id="25e89-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="25e89-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="25e89-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="25e89-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="25e89-106">Diese Aktion können Sie kurzlebige eingebettet werden URLs für ein Element abrufen, um eine temporäre Vorschau zu rendern.</span><span class="sxs-lookup"><span data-stu-id="25e89-106">This action allows you to obtain short-lived embeddable URLs for an item in order to render a temporary preview.</span></span>

<span data-ttu-id="25e89-107">Wenn Sie Links mit langer Lebensdauer eingebettet werden abrufen möchten, verwenden Sie stattdessen die [CreateLink][] API.</span><span class="sxs-lookup"><span data-stu-id="25e89-107">If you want to obtain long-lived embeddable links, use the [createLink][] API instead.</span></span>

> <span data-ttu-id="25e89-108">**Hinweis:** Die **Preview** -Aktion ist derzeit nur auf SharePoint und OneDrive für Unternehmen verfügbar.</span><span class="sxs-lookup"><span data-stu-id="25e89-108">**Note:** The **preview** action is currently only available on SharePoint and OneDrive for Business.</span></span>

[createLink]: driveitem-createlink.md

## <a name="permissions"></a><span data-ttu-id="25e89-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="25e89-110">Permissions</span></span>

<span data-ttu-id="25e89-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25e89-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="25e89-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="25e89-113">Permission type</span></span>                        | <span data-ttu-id="25e89-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="25e89-114">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="25e89-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="25e89-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="25e89-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25e89-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="25e89-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="25e89-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25e89-118">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25e89-118">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="25e89-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="25e89-119">Application</span></span>                            | <span data-ttu-id="25e89-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="25e89-120">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="25e89-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="25e89-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/preview
POST /groups/{groupId}/drive/items/{itemId}/preview
POST /me/drive/items/{itemId}/preview
POST /sites/{siteId}/drive/items/{itemId}/preview
POST /users/{userId}/drive/items/{itemId}/preview
POST /shares/{shareId}/driveItem/preview
```

## <a name="request-body"></a><span data-ttu-id="25e89-122">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="25e89-122">Request body</span></span>

<span data-ttu-id="25e89-123">Der Text der Anforderung definiert Eigenschaften der embeddable URL Ihrer Anwendung anfordert.</span><span class="sxs-lookup"><span data-stu-id="25e89-123">The body of the request defines properties of the embeddable URL your application is requesting.</span></span>
<span data-ttu-id="25e89-124">Bei der Anforderung sollte es sich um ein JSON-Objekt mit folgenden Eigenschaften handeln:</span><span class="sxs-lookup"><span data-stu-id="25e89-124">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="25e89-125">Name</span><span class="sxs-lookup"><span data-stu-id="25e89-125">Name</span></span>      |  <span data-ttu-id="25e89-126">Typ</span><span class="sxs-lookup"><span data-stu-id="25e89-126">Type</span></span>         | <span data-ttu-id="25e89-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="25e89-127">Description</span></span>
|:------------|:--------------|:-----------------------------------------------
| <span data-ttu-id="25e89-128">Viewer</span><span class="sxs-lookup"><span data-stu-id="25e89-128">viewer</span></span>      | <span data-ttu-id="25e89-129">string</span><span class="sxs-lookup"><span data-stu-id="25e89-129">string</span></span>        | <span data-ttu-id="25e89-130">Optional.</span><span class="sxs-lookup"><span data-stu-id="25e89-130">Optional.</span></span> <span data-ttu-id="25e89-131">Preview-app verwendet.</span><span class="sxs-lookup"><span data-stu-id="25e89-131">Preview app to use.</span></span> <span data-ttu-id="25e89-132">`onedrive` oder `office`.</span><span class="sxs-lookup"><span data-stu-id="25e89-132">`onedrive` or `office`.</span></span> <span data-ttu-id="25e89-133">Wenn der Wert null ist, wird ein passender Viewer automatisch ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="25e89-133">If null, a suitable viewer will be chosen automatically.</span></span>
| <span data-ttu-id="25e89-134">Chromeless</span><span class="sxs-lookup"><span data-stu-id="25e89-134">chromeless</span></span>  | <span data-ttu-id="25e89-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="25e89-135">boolean</span></span>       | <span data-ttu-id="25e89-136">Optional.</span><span class="sxs-lookup"><span data-stu-id="25e89-136">Optional.</span></span> <span data-ttu-id="25e89-137">Wenn `true` (Standard), die eingebettete Ansicht wird nicht schließen Sie alle Steuerelemente.</span><span class="sxs-lookup"><span data-stu-id="25e89-137">If `true` (default), the embedded view will not include any controls.</span></span>
| <span data-ttu-id="25e89-138">allowEdit</span><span class="sxs-lookup"><span data-stu-id="25e89-138">allowEdit</span></span>   | <span data-ttu-id="25e89-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="25e89-139">boolean</span></span>       | <span data-ttu-id="25e89-140">Optional.</span><span class="sxs-lookup"><span data-stu-id="25e89-140">Optional.</span></span> <span data-ttu-id="25e89-141">Wenn `true`, die Datei aus der eingebetteten Benutzeroberfläche bearbeitet werden kann.</span><span class="sxs-lookup"><span data-stu-id="25e89-141">If `true`, the file can be edited from the embedded UI.</span></span>
| <span data-ttu-id="25e89-142">page</span><span class="sxs-lookup"><span data-stu-id="25e89-142">page</span></span>        | <span data-ttu-id="25e89-143">Zeichenfolge/eine einzelne Nummer</span><span class="sxs-lookup"><span data-stu-id="25e89-143">string/number</span></span> | <span data-ttu-id="25e89-144">Optional.</span><span class="sxs-lookup"><span data-stu-id="25e89-144">Optional.</span></span> <span data-ttu-id="25e89-145">Seitenzahl des Dokuments an, falls zutreffend zu starten.</span><span class="sxs-lookup"><span data-stu-id="25e89-145">Page number of document to start at, if applicable.</span></span> <span data-ttu-id="25e89-146">Als Zeichenfolge für die zukünftige Verwendung Fällen um Dateitypen wie ZIP angegeben.</span><span class="sxs-lookup"><span data-stu-id="25e89-146">Specified as string for future use cases around file types such as ZIP.</span></span>
| <span data-ttu-id="25e89-147">Zoom</span><span class="sxs-lookup"><span data-stu-id="25e89-147">zoom</span></span>        | <span data-ttu-id="25e89-148">number</span><span class="sxs-lookup"><span data-stu-id="25e89-148">number</span></span>        | <span data-ttu-id="25e89-149">Optional.</span><span class="sxs-lookup"><span data-stu-id="25e89-149">Optional.</span></span> <span data-ttu-id="25e89-150">Zoom-Wert auf, falls zutreffend.</span><span class="sxs-lookup"><span data-stu-id="25e89-150">Zoom level to start at, if applicable.</span></span>

## <a name="response"></a><span data-ttu-id="25e89-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="25e89-151">Response</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

<span data-ttu-id="25e89-152">Die Antwort wird ein JSON-Objekt mit den folgenden Eigenschaften werden:</span><span class="sxs-lookup"><span data-stu-id="25e89-152">The response will be a JSON object containing the following properties:</span></span>

| <span data-ttu-id="25e89-153">Name</span><span class="sxs-lookup"><span data-stu-id="25e89-153">Name</span></span>           | <span data-ttu-id="25e89-154">Typ</span><span class="sxs-lookup"><span data-stu-id="25e89-154">Type</span></span>   | <span data-ttu-id="25e89-155">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="25e89-155">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="25e89-156">getUrl</span><span class="sxs-lookup"><span data-stu-id="25e89-156">getUrl</span></span>         | <span data-ttu-id="25e89-157">string</span><span class="sxs-lookup"><span data-stu-id="25e89-157">string</span></span> | <span data-ttu-id="25e89-158">URL für das Einbetten von mit HTTP-GET (Iframes usw.) geeignet</span><span class="sxs-lookup"><span data-stu-id="25e89-158">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="25e89-159">postUrl</span><span class="sxs-lookup"><span data-stu-id="25e89-159">postUrl</span></span>        | <span data-ttu-id="25e89-160">string</span><span class="sxs-lookup"><span data-stu-id="25e89-160">string</span></span> | <span data-ttu-id="25e89-161">URL für das Einbetten von mithilfe von HTTP POST geeignet (bilden, JS, usw..)</span><span class="sxs-lookup"><span data-stu-id="25e89-161">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="25e89-162">postParameters</span><span class="sxs-lookup"><span data-stu-id="25e89-162">postParameters</span></span> | <span data-ttu-id="25e89-163">string</span><span class="sxs-lookup"><span data-stu-id="25e89-163">string</span></span> | <span data-ttu-id="25e89-164">POST-Parameter einschließen, wenn PostUrl verwenden</span><span class="sxs-lookup"><span data-stu-id="25e89-164">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="25e89-165">GetUrl, PostUrl oder beide möglicherweise abhängig vom aktuellen Status des Embed-Unterstützung für den angegebenen Optionen zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="25e89-165">Either getUrl, postUrl, or both might be returned depending on the current state of embed support for the specified options.</span></span>

<span data-ttu-id="25e89-166">PostParameters ist eine Zeichenfolge, die als formatiert `application/x-www-form-urlencoded`, und wenn Ausführen von POST an den PostUrl Content-Type entsprechend festgelegt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="25e89-166">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="25e89-167">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="25e89-167">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="viewers"></a><span data-ttu-id="25e89-168">Leser von Berichten</span><span class="sxs-lookup"><span data-stu-id="25e89-168">Viewers</span></span>

<span data-ttu-id="25e89-169">Die folgenden Werte sind für den **Viewer** -Parameter zulässig.</span><span class="sxs-lookup"><span data-stu-id="25e89-169">The following values are allowed for the **viewer** parameter.</span></span>

| <span data-ttu-id="25e89-170">Typwert</span><span class="sxs-lookup"><span data-stu-id="25e89-170">Type value</span></span> | <span data-ttu-id="25e89-171">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="25e89-171">Description</span></span>
|:-----------|:----------------------------------------------------------------
| <span data-ttu-id="25e89-172">(null)</span><span class="sxs-lookup"><span data-stu-id="25e89-172">(null)</span></span>     | <span data-ttu-id="25e89-173">Wählt eine entsprechende app für das Rendern der Datei.</span><span class="sxs-lookup"><span data-stu-id="25e89-173">Chooses an appropriate app for rendering the file.</span></span> <span data-ttu-id="25e89-174">Hiermit wird in den meisten Fällen verwendet die `onedrive` Vorschau, aber nach dem Dateityp variieren.</span><span class="sxs-lookup"><span data-stu-id="25e89-174">In most cases this will use the `onedrive` previewer, but may vary by file type.</span></span>
| `onedrive` | <span data-ttu-id="25e89-175">Verwenden Sie die previewer OneDrive-app, um die Datei zu rendern.</span><span class="sxs-lookup"><span data-stu-id="25e89-175">Use the OneDrive previewer app to render the file.</span></span>
| `office`   | <span data-ttu-id="25e89-176">Verwenden Sie die WAC (online für Office), um die Datei zu rendern.</span><span class="sxs-lookup"><span data-stu-id="25e89-176">Use the WAC (Office online) to render the file.</span></span> <span data-ttu-id="25e89-177">Nur gültig für Office-Dokumenten.</span><span class="sxs-lookup"><span data-stu-id="25e89-177">Only valid for Office documents.</span></span>

### <a name="chrome-vs-chromeless"></a><span data-ttu-id="25e89-178">Chrome Vs chromeless</span><span class="sxs-lookup"><span data-stu-id="25e89-178">Chrome vs chromeless</span></span>

<span data-ttu-id="25e89-179">Wenn `chromeless` true ist, wird die Vorschau einer bare Rendering der Datei werden.</span><span class="sxs-lookup"><span data-stu-id="25e89-179">If `chromeless` is true, the preview will be a bare rendering of the file.</span></span>
<span data-ttu-id="25e89-180">Anderenfalls möglicherweise zusätzliche Symbolleisten/Schaltflächen für die Interaktion mit der Dokument-Ansicht angezeigt.</span><span class="sxs-lookup"><span data-stu-id="25e89-180">Otherwise, there may be additional toolbars/buttons displayed for interacting with the document/view.</span></span>

### <a name="viewedit"></a><span data-ttu-id="25e89-181">Anzeigen/Bearbeiten</span><span class="sxs-lookup"><span data-stu-id="25e89-181">View/edit</span></span>

<span data-ttu-id="25e89-182">Wenn `allowEdit` true ist, das Dokument durch Benutzerinteraktion mit eingebettete Vorschau geändert werden kann.</span><span class="sxs-lookup"><span data-stu-id="25e89-182">If `allowEdit` is true, the document can be modified by user interaction with the embedded preview.</span></span>
<span data-ttu-id="25e89-183">Diese Funktion möglicherweise nicht für alle apps Preview oder Dateitypen zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="25e89-183">This capability may not be available for all preview apps or file types.</span></span>

### <a name="pagezoom"></a><span data-ttu-id="25e89-184">Seite/zoom</span><span class="sxs-lookup"><span data-stu-id="25e89-184">Page/zoom</span></span>

<span data-ttu-id="25e89-185">Die `page` und `zoom` Optionen möglicherweise nicht für alle Preview apps verfügbar, jedoch wird angewendet werden soll, wenn die app Preview unterstützt.</span><span class="sxs-lookup"><span data-stu-id="25e89-185">The `page` and `zoom` options might not be available for all preview apps, but will be applied if the preview app supports it.</span></span>