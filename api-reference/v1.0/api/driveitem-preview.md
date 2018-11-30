---
title: 'DriveItem: Vorschau'
description: Diese Aktion können Sie kurzlebige eingebettet werden URLs für ein Element abrufen, um eine temporäre Vorschau zu rendern.
ms.openlocfilehash: 741e449c972ad372aae30d9921cdb3b7fa1fc40d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018913"
---
# <a name="driveitem-preview"></a><span data-ttu-id="c2388-103">DriveItem: Vorschau</span><span class="sxs-lookup"><span data-stu-id="c2388-103">driveItem: preview</span></span>

<span data-ttu-id="c2388-104">Diese Aktion können Sie kurzlebige eingebettet werden URLs für ein Element abrufen, um eine temporäre Vorschau zu rendern.</span><span class="sxs-lookup"><span data-stu-id="c2388-104">This action allows you to obtain short-lived embeddable URLs for an item in order to render a temporary preview.</span></span>

<span data-ttu-id="c2388-105">Wenn Sie Links mit langer Lebensdauer eingebettet werden abrufen möchten, verwenden Sie stattdessen die [CreateLink][] API.</span><span class="sxs-lookup"><span data-stu-id="c2388-105">If you want to obtain long-lived embeddable links, use the [createLink][] API instead.</span></span>

> <span data-ttu-id="c2388-106">**Hinweis:** Die **Preview** -Aktion ist derzeit nur auf SharePoint und OneDrive für Unternehmen verfügbar.</span><span class="sxs-lookup"><span data-stu-id="c2388-106">**Note:** The **preview** action is currently only available on SharePoint and OneDrive for Business.</span></span>

[createLink]: driveitem-createlink.md

## <a name="permissions"></a><span data-ttu-id="c2388-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c2388-108">Permissions</span></span>

<span data-ttu-id="c2388-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2388-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c2388-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c2388-111">Permission type</span></span>                        | <span data-ttu-id="c2388-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c2388-112">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="c2388-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c2388-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="c2388-114">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2388-114">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="c2388-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c2388-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2388-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2388-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="c2388-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c2388-117">Application</span></span>                            | <span data-ttu-id="c2388-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c2388-118">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="c2388-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c2388-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/preview
POST /groups/{groupId}/drive/items/{itemId}/preview
POST /me/drive/items/{itemId}/preview
POST /sites/{siteId}/drive/items/{itemId}/preview
POST /users/{userId}/drive/items/{itemId}/preview
POST /shares/{shareId}/driveItem/preview
```

## <a name="request-body"></a><span data-ttu-id="c2388-120">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c2388-120">Request body</span></span>

<span data-ttu-id="c2388-121">Der Text der Anforderung definiert Eigenschaften der embeddable URL Ihrer Anwendung anfordert.</span><span class="sxs-lookup"><span data-stu-id="c2388-121">The body of the request defines properties of the embeddable URL your application is requesting.</span></span>
<span data-ttu-id="c2388-122">Bei der Anforderung sollte es sich um ein JSON-Objekt mit folgenden Eigenschaften handeln:</span><span class="sxs-lookup"><span data-stu-id="c2388-122">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="c2388-123">Name</span><span class="sxs-lookup"><span data-stu-id="c2388-123">Name</span></span>      |  <span data-ttu-id="c2388-124">Typ</span><span class="sxs-lookup"><span data-stu-id="c2388-124">Type</span></span>         | <span data-ttu-id="c2388-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c2388-125">Description</span></span>
|:------------|:--------------|:-----------------------------------------------
| <span data-ttu-id="c2388-126">page</span><span class="sxs-lookup"><span data-stu-id="c2388-126">page</span></span>        | <span data-ttu-id="c2388-127">Zeichenfolge/eine einzelne Nummer</span><span class="sxs-lookup"><span data-stu-id="c2388-127">string/number</span></span> | <span data-ttu-id="c2388-128">Optional.</span><span class="sxs-lookup"><span data-stu-id="c2388-128">Optional.</span></span> <span data-ttu-id="c2388-129">Seitenzahl des Dokuments an, falls zutreffend zu starten.</span><span class="sxs-lookup"><span data-stu-id="c2388-129">Page number of document to start at, if applicable.</span></span> <span data-ttu-id="c2388-130">Als Zeichenfolge für die zukünftige Verwendung Fällen um Dateitypen wie ZIP angegeben.</span><span class="sxs-lookup"><span data-stu-id="c2388-130">Specified as string for future use cases around file types such as ZIP.</span></span>
| <span data-ttu-id="c2388-131">Zoom</span><span class="sxs-lookup"><span data-stu-id="c2388-131">zoom</span></span>        | <span data-ttu-id="c2388-132">number</span><span class="sxs-lookup"><span data-stu-id="c2388-132">number</span></span>        | <span data-ttu-id="c2388-133">Optional.</span><span class="sxs-lookup"><span data-stu-id="c2388-133">Optional.</span></span> <span data-ttu-id="c2388-134">Zoom-Wert auf, falls zutreffend.</span><span class="sxs-lookup"><span data-stu-id="c2388-134">Zoom level to start at, if applicable.</span></span>

## <a name="response"></a><span data-ttu-id="c2388-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="c2388-135">Response</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

<span data-ttu-id="c2388-136">Die Antwort wird ein JSON-Objekt mit den folgenden Eigenschaften werden:</span><span class="sxs-lookup"><span data-stu-id="c2388-136">The response will be a JSON object containing the following properties:</span></span>

| <span data-ttu-id="c2388-137">Name</span><span class="sxs-lookup"><span data-stu-id="c2388-137">Name</span></span>           | <span data-ttu-id="c2388-138">Typ</span><span class="sxs-lookup"><span data-stu-id="c2388-138">Type</span></span>   | <span data-ttu-id="c2388-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c2388-139">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="c2388-140">getUrl</span><span class="sxs-lookup"><span data-stu-id="c2388-140">getUrl</span></span>         | <span data-ttu-id="c2388-141">string</span><span class="sxs-lookup"><span data-stu-id="c2388-141">string</span></span> | <span data-ttu-id="c2388-142">URL für das Einbetten von mit HTTP-GET (Iframes usw.) geeignet</span><span class="sxs-lookup"><span data-stu-id="c2388-142">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="c2388-143">postUrl</span><span class="sxs-lookup"><span data-stu-id="c2388-143">postUrl</span></span>        | <span data-ttu-id="c2388-144">string</span><span class="sxs-lookup"><span data-stu-id="c2388-144">string</span></span> | <span data-ttu-id="c2388-145">URL für das Einbetten von mithilfe von HTTP POST geeignet (bilden, JS, usw..)</span><span class="sxs-lookup"><span data-stu-id="c2388-145">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="c2388-146">postParameters</span><span class="sxs-lookup"><span data-stu-id="c2388-146">postParameters</span></span> | <span data-ttu-id="c2388-147">string</span><span class="sxs-lookup"><span data-stu-id="c2388-147">string</span></span> | <span data-ttu-id="c2388-148">POST-Parameter einschließen, wenn PostUrl verwenden</span><span class="sxs-lookup"><span data-stu-id="c2388-148">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="c2388-149">GetUrl, PostUrl oder beide möglicherweise abhängig vom aktuellen Status des Embed-Unterstützung für den angegebenen Optionen zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c2388-149">Either getUrl, postUrl, or both might be returned depending on the current state of embed support for the specified options.</span></span>

<span data-ttu-id="c2388-150">PostParameters ist eine Zeichenfolge, die als formatiert `application/x-www-form-urlencoded`, und wenn Ausführen von POST an den PostUrl Content-Type entsprechend festgelegt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="c2388-150">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="c2388-151">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="c2388-151">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="pagezoom"></a><span data-ttu-id="c2388-152">Seite/zoom</span><span class="sxs-lookup"><span data-stu-id="c2388-152">Page/zoom</span></span>

<span data-ttu-id="c2388-153">Die Optionen 'zoom' und 'Seite' möglicherweise nicht für alle Preview apps verfügbar, jedoch werden angewendet werden soll, wenn die app Preview unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c2388-153">The 'page' and 'zoom' options may not be available for all preview apps, but will be applied if the preview app supports it.</span></span>
