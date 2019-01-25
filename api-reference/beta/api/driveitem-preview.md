---
title: 'DriveItem: Vorschau'
description: Diese Aktion können Sie kurzlebige eingebettet werden URLs für ein Element abrufen, um eine temporäre Vorschau zu rendern.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5a49a05e1e01616bc9bbbb713fd05805d9af3070
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508538"
---
# <a name="driveitem-preview"></a><span data-ttu-id="64c68-103">DriveItem: Vorschau</span><span class="sxs-lookup"><span data-stu-id="64c68-103">driveItem: preview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64c68-104">Diese Aktion können Sie kurzlebige eingebettet werden URLs für ein Element abrufen, um eine temporäre Vorschau zu rendern.</span><span class="sxs-lookup"><span data-stu-id="64c68-104">This action allows you to obtain short-lived embeddable URLs for an item in order to render a temporary preview.</span></span>

<span data-ttu-id="64c68-105">Wenn Sie Links mit langer Lebensdauer eingebettet werden abrufen möchten, verwenden Sie stattdessen die [CreateLink][] API.</span><span class="sxs-lookup"><span data-stu-id="64c68-105">If you want to obtain long-lived embeddable links, use the [createLink][] API instead.</span></span>

> <span data-ttu-id="64c68-106">**Hinweis:** Die **Preview** -Aktion ist derzeit nur auf SharePoint und OneDrive für Unternehmen verfügbar.</span><span class="sxs-lookup"><span data-stu-id="64c68-106">**Note:** The **preview** action is currently only available on SharePoint and OneDrive for Business.</span></span>

[createLink]: driveitem-createlink.md

## <a name="permissions"></a><span data-ttu-id="64c68-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="64c68-108">Permissions</span></span>

<span data-ttu-id="64c68-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64c68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="64c68-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="64c68-111">Permission type</span></span>                        | <span data-ttu-id="64c68-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="64c68-112">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="64c68-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="64c68-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="64c68-114">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64c68-114">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="64c68-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="64c68-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64c68-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64c68-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="64c68-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="64c68-117">Application</span></span>                            | <span data-ttu-id="64c68-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="64c68-118">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="64c68-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="64c68-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/preview
POST /groups/{groupId}/drive/items/{itemId}/preview
POST /me/drive/items/{itemId}/preview
POST /sites/{siteId}/drive/items/{itemId}/preview
POST /users/{userId}/drive/items/{itemId}/preview
POST /shares/{shareId}/driveItem/preview
```

## <a name="request-body"></a><span data-ttu-id="64c68-120">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="64c68-120">Request body</span></span>

<span data-ttu-id="64c68-121">Der Text der Anforderung definiert Eigenschaften der embeddable URL Ihrer Anwendung anfordert.</span><span class="sxs-lookup"><span data-stu-id="64c68-121">The body of the request defines properties of the embeddable URL your application is requesting.</span></span>
<span data-ttu-id="64c68-122">Bei der Anforderung sollte es sich um ein JSON-Objekt mit folgenden Eigenschaften handeln:</span><span class="sxs-lookup"><span data-stu-id="64c68-122">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="64c68-123">Name</span><span class="sxs-lookup"><span data-stu-id="64c68-123">Name</span></span>      |  <span data-ttu-id="64c68-124">Typ</span><span class="sxs-lookup"><span data-stu-id="64c68-124">Type</span></span>         | <span data-ttu-id="64c68-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="64c68-125">Description</span></span>
|:------------|:--------------|:-----------------------------------------------
| <span data-ttu-id="64c68-126">Viewer</span><span class="sxs-lookup"><span data-stu-id="64c68-126">viewer</span></span>      | <span data-ttu-id="64c68-127">string</span><span class="sxs-lookup"><span data-stu-id="64c68-127">string</span></span>        | <span data-ttu-id="64c68-128">Optional.</span><span class="sxs-lookup"><span data-stu-id="64c68-128">Optional.</span></span> <span data-ttu-id="64c68-129">Preview-app verwendet.</span><span class="sxs-lookup"><span data-stu-id="64c68-129">Preview app to use.</span></span> <span data-ttu-id="64c68-130">`onedrive` oder `office`.</span><span class="sxs-lookup"><span data-stu-id="64c68-130">`onedrive` or `office`.</span></span> <span data-ttu-id="64c68-131">Wenn der Wert null ist, wird ein passender Viewer automatisch ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="64c68-131">If null, a suitable viewer will be chosen automatically.</span></span>
| <span data-ttu-id="64c68-132">Chromeless</span><span class="sxs-lookup"><span data-stu-id="64c68-132">chromeless</span></span>  | <span data-ttu-id="64c68-133">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="64c68-133">boolean</span></span>       | <span data-ttu-id="64c68-134">Optional.</span><span class="sxs-lookup"><span data-stu-id="64c68-134">Optional.</span></span> <span data-ttu-id="64c68-135">Wenn `true` (Standard), die eingebettete Ansicht wird nicht schließen Sie alle Steuerelemente.</span><span class="sxs-lookup"><span data-stu-id="64c68-135">If `true` (default), the embedded view will not include any controls.</span></span>
| <span data-ttu-id="64c68-136">AllowEdit</span><span class="sxs-lookup"><span data-stu-id="64c68-136">allowEdit</span></span>   | <span data-ttu-id="64c68-137">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="64c68-137">boolean</span></span>       | <span data-ttu-id="64c68-138">Optional.</span><span class="sxs-lookup"><span data-stu-id="64c68-138">Optional.</span></span> <span data-ttu-id="64c68-139">Wenn `true`, die Datei aus der eingebetteten Benutzeroberfläche bearbeitet werden kann.</span><span class="sxs-lookup"><span data-stu-id="64c68-139">If `true`, the file can be edited from the embedded UI.</span></span>
| <span data-ttu-id="64c68-140">page</span><span class="sxs-lookup"><span data-stu-id="64c68-140">page</span></span>        | <span data-ttu-id="64c68-141">Zeichenfolge/eine einzelne Nummer</span><span class="sxs-lookup"><span data-stu-id="64c68-141">string/number</span></span> | <span data-ttu-id="64c68-142">Optional.</span><span class="sxs-lookup"><span data-stu-id="64c68-142">Optional.</span></span> <span data-ttu-id="64c68-143">Seitenzahl des Dokuments an, falls zutreffend zu starten.</span><span class="sxs-lookup"><span data-stu-id="64c68-143">Page number of document to start at, if applicable.</span></span> <span data-ttu-id="64c68-144">Als Zeichenfolge für die zukünftige Verwendung Fällen um Dateitypen wie ZIP angegeben.</span><span class="sxs-lookup"><span data-stu-id="64c68-144">Specified as string for future use cases around file types such as ZIP.</span></span>
| <span data-ttu-id="64c68-145">Zoom</span><span class="sxs-lookup"><span data-stu-id="64c68-145">zoom</span></span>        | <span data-ttu-id="64c68-146">number</span><span class="sxs-lookup"><span data-stu-id="64c68-146">number</span></span>        | <span data-ttu-id="64c68-147">Optional.</span><span class="sxs-lookup"><span data-stu-id="64c68-147">Optional.</span></span> <span data-ttu-id="64c68-148">Zoom-Wert auf, falls zutreffend.</span><span class="sxs-lookup"><span data-stu-id="64c68-148">Zoom level to start at, if applicable.</span></span>

## <a name="response"></a><span data-ttu-id="64c68-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="64c68-149">Response</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

<span data-ttu-id="64c68-150">Die Antwort wird ein JSON-Objekt mit den folgenden Eigenschaften werden:</span><span class="sxs-lookup"><span data-stu-id="64c68-150">The response will be a JSON object containing the following properties:</span></span>

| <span data-ttu-id="64c68-151">Name</span><span class="sxs-lookup"><span data-stu-id="64c68-151">Name</span></span>           | <span data-ttu-id="64c68-152">Typ</span><span class="sxs-lookup"><span data-stu-id="64c68-152">Type</span></span>   | <span data-ttu-id="64c68-153">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="64c68-153">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="64c68-154">getUrl</span><span class="sxs-lookup"><span data-stu-id="64c68-154">getUrl</span></span>         | <span data-ttu-id="64c68-155">string</span><span class="sxs-lookup"><span data-stu-id="64c68-155">string</span></span> | <span data-ttu-id="64c68-156">URL für das Einbetten von mit HTTP-GET (Iframes usw.) geeignet</span><span class="sxs-lookup"><span data-stu-id="64c68-156">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="64c68-157">postUrl</span><span class="sxs-lookup"><span data-stu-id="64c68-157">postUrl</span></span>        | <span data-ttu-id="64c68-158">string</span><span class="sxs-lookup"><span data-stu-id="64c68-158">string</span></span> | <span data-ttu-id="64c68-159">URL für das Einbetten von mithilfe von HTTP POST geeignet (bilden, JS, usw..)</span><span class="sxs-lookup"><span data-stu-id="64c68-159">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="64c68-160">postParameters</span><span class="sxs-lookup"><span data-stu-id="64c68-160">postParameters</span></span> | <span data-ttu-id="64c68-161">string</span><span class="sxs-lookup"><span data-stu-id="64c68-161">string</span></span> | <span data-ttu-id="64c68-162">POST-Parameter einschließen, wenn PostUrl verwenden</span><span class="sxs-lookup"><span data-stu-id="64c68-162">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="64c68-163">GetUrl, PostUrl oder beide möglicherweise abhängig vom aktuellen Status des Embed-Unterstützung für den angegebenen Optionen zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="64c68-163">Either getUrl, postUrl, or both might be returned depending on the current state of embed support for the specified options.</span></span>

<span data-ttu-id="64c68-164">PostParameters ist eine Zeichenfolge, die als formatiert `application/x-www-form-urlencoded`, und wenn Ausführen von POST an den PostUrl Content-Type entsprechend festgelegt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="64c68-164">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="64c68-165">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="64c68-165">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="viewers"></a><span data-ttu-id="64c68-166">Leser von Berichten</span><span class="sxs-lookup"><span data-stu-id="64c68-166">Viewers</span></span>

<span data-ttu-id="64c68-167">Die folgenden Werte sind für den **Viewer** -Parameter zulässig.</span><span class="sxs-lookup"><span data-stu-id="64c68-167">The following values are allowed for the **viewer** parameter.</span></span>

| <span data-ttu-id="64c68-168">Typwert</span><span class="sxs-lookup"><span data-stu-id="64c68-168">Type value</span></span> | <span data-ttu-id="64c68-169">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="64c68-169">Description</span></span>
|:-----------|:----------------------------------------------------------------
| <span data-ttu-id="64c68-170">Null
</span><span class="sxs-lookup"><span data-stu-id="64c68-170">(null)</span></span>     | <span data-ttu-id="64c68-171">Wählt eine entsprechende app für das Rendern der Datei.</span><span class="sxs-lookup"><span data-stu-id="64c68-171">Chooses an appropriate app for rendering the file.</span></span> <span data-ttu-id="64c68-172">Hiermit wird in den meisten Fällen verwendet die `onedrive` Vorschau, aber nach dem Dateityp variieren.</span><span class="sxs-lookup"><span data-stu-id="64c68-172">In most cases this will use the `onedrive` previewer, but may vary by file type.</span></span>
| `onedrive` | <span data-ttu-id="64c68-173">Verwenden Sie die previewer OneDrive-app, um die Datei zu rendern.</span><span class="sxs-lookup"><span data-stu-id="64c68-173">Use the OneDrive previewer app to render the file.</span></span>
| `office`   | <span data-ttu-id="64c68-174">Verwenden Sie die WAC (online für Office), um die Datei zu rendern.</span><span class="sxs-lookup"><span data-stu-id="64c68-174">Use the WAC (Office online) to render the file.</span></span> <span data-ttu-id="64c68-175">Nur gültig für Office-Dokumenten.</span><span class="sxs-lookup"><span data-stu-id="64c68-175">Only valid for Office documents.</span></span>

### <a name="chrome-vs-chromeless"></a><span data-ttu-id="64c68-176">Chrome Vs chromeless</span><span class="sxs-lookup"><span data-stu-id="64c68-176">Chrome vs chromeless</span></span>

<span data-ttu-id="64c68-177">Wenn `chromeless` true ist, wird die Vorschau einer bare Rendering der Datei werden.</span><span class="sxs-lookup"><span data-stu-id="64c68-177">If `chromeless` is true, the preview will be a bare rendering of the file.</span></span>
<span data-ttu-id="64c68-178">Anderenfalls möglicherweise zusätzliche Symbolleisten/Schaltflächen für die Interaktion mit der Dokument-Ansicht angezeigt.</span><span class="sxs-lookup"><span data-stu-id="64c68-178">Otherwise, there may be additional toolbars/buttons displayed for interacting with the document/view.</span></span>

### <a name="viewedit"></a><span data-ttu-id="64c68-179">Anzeigen/Bearbeiten</span><span class="sxs-lookup"><span data-stu-id="64c68-179">View/edit</span></span>

<span data-ttu-id="64c68-180">Wenn `allowEdit` true ist, das Dokument durch Benutzerinteraktion mit eingebettete Vorschau geändert werden kann.</span><span class="sxs-lookup"><span data-stu-id="64c68-180">If `allowEdit` is true, the document can be modified by user interaction with the embedded preview.</span></span>
<span data-ttu-id="64c68-181">Diese Funktion möglicherweise nicht für alle apps Preview oder Dateitypen zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="64c68-181">This capability may not be available for all preview apps or file types.</span></span>

### <a name="pagezoom"></a><span data-ttu-id="64c68-182">Seite/zoom</span><span class="sxs-lookup"><span data-stu-id="64c68-182">Page/zoom</span></span>

<span data-ttu-id="64c68-183">Die `page` und `zoom` Optionen möglicherweise nicht für alle Preview apps verfügbar, jedoch wird angewendet werden soll, wenn die app Preview unterstützt.</span><span class="sxs-lookup"><span data-stu-id="64c68-183">The `page` and `zoom` options might not be available for all preview apps, but will be applied if the preview app supports it.</span></span>
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-preview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
