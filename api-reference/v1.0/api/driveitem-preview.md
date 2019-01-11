---
title: 'DriveItem: Vorschau'
description: Diese Aktion können Sie kurzlebige eingebettet werden URLs für ein Element abrufen, um eine temporäre Vorschau zu rendern.
localization_priority: Normal
ms.openlocfilehash: c04a73d514dfb5a92030c4c2016579d469063f9d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27850771"
---
# <a name="driveitem-preview"></a><span data-ttu-id="3c320-103">DriveItem: Vorschau</span><span class="sxs-lookup"><span data-stu-id="3c320-103">driveItem: preview</span></span>

<span data-ttu-id="3c320-104">Diese Aktion können Sie kurzlebige eingebettet werden URLs für ein Element abrufen, um eine temporäre Vorschau zu rendern.</span><span class="sxs-lookup"><span data-stu-id="3c320-104">This action allows you to obtain short-lived embeddable URLs for an item in order to render a temporary preview.</span></span>

<span data-ttu-id="3c320-105">Wenn Sie Links mit langer Lebensdauer eingebettet werden abrufen möchten, verwenden Sie stattdessen die [CreateLink][] API.</span><span class="sxs-lookup"><span data-stu-id="3c320-105">If you want to obtain long-lived embeddable links, use the [createLink][] API instead.</span></span>

> <span data-ttu-id="3c320-106">**Hinweis:** Die **Preview** -Aktion ist derzeit nur auf SharePoint und OneDrive für Unternehmen verfügbar.</span><span class="sxs-lookup"><span data-stu-id="3c320-106">**Note:** The **preview** action is currently only available on SharePoint and OneDrive for Business.</span></span>

[createLink]: driveitem-createlink.md

## <a name="permissions"></a><span data-ttu-id="3c320-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3c320-108">Permissions</span></span>

<span data-ttu-id="3c320-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c320-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3c320-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3c320-111">Permission type</span></span>                        | <span data-ttu-id="3c320-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3c320-112">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="3c320-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3c320-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="3c320-114">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c320-114">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="3c320-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3c320-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c320-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c320-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="3c320-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3c320-117">Application</span></span>                            | <span data-ttu-id="3c320-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3c320-118">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="3c320-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3c320-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/preview
POST /groups/{groupId}/drive/items/{itemId}/preview
POST /me/drive/items/{itemId}/preview
POST /sites/{siteId}/drive/items/{itemId}/preview
POST /users/{userId}/drive/items/{itemId}/preview
POST /shares/{shareId}/driveItem/preview
```

## <a name="request-body"></a><span data-ttu-id="3c320-120">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3c320-120">Request body</span></span>

<span data-ttu-id="3c320-121">Der Text der Anforderung definiert Eigenschaften der embeddable URL Ihrer Anwendung anfordert.</span><span class="sxs-lookup"><span data-stu-id="3c320-121">The body of the request defines properties of the embeddable URL your application is requesting.</span></span>
<span data-ttu-id="3c320-122">Bei der Anforderung sollte es sich um ein JSON-Objekt mit folgenden Eigenschaften handeln:</span><span class="sxs-lookup"><span data-stu-id="3c320-122">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="3c320-123">Name</span><span class="sxs-lookup"><span data-stu-id="3c320-123">Name</span></span>      |  <span data-ttu-id="3c320-124">Typ</span><span class="sxs-lookup"><span data-stu-id="3c320-124">Type</span></span>         | <span data-ttu-id="3c320-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3c320-125">Description</span></span>
|:------------|:--------------|:-----------------------------------------------
| <span data-ttu-id="3c320-126">page</span><span class="sxs-lookup"><span data-stu-id="3c320-126">page</span></span>        | <span data-ttu-id="3c320-127">Zeichenfolge/eine einzelne Nummer</span><span class="sxs-lookup"><span data-stu-id="3c320-127">string/number</span></span> | <span data-ttu-id="3c320-128">Optional.</span><span class="sxs-lookup"><span data-stu-id="3c320-128">Optional.</span></span> <span data-ttu-id="3c320-129">Seitenzahl des Dokuments an, falls zutreffend zu starten.</span><span class="sxs-lookup"><span data-stu-id="3c320-129">Page number of document to start at, if applicable.</span></span> <span data-ttu-id="3c320-130">Als Zeichenfolge für die zukünftige Verwendung Fällen um Dateitypen wie ZIP angegeben.</span><span class="sxs-lookup"><span data-stu-id="3c320-130">Specified as string for future use cases around file types such as ZIP.</span></span>
| <span data-ttu-id="3c320-131">Zoom</span><span class="sxs-lookup"><span data-stu-id="3c320-131">zoom</span></span>        | <span data-ttu-id="3c320-132">number</span><span class="sxs-lookup"><span data-stu-id="3c320-132">number</span></span>        | <span data-ttu-id="3c320-133">Optional.</span><span class="sxs-lookup"><span data-stu-id="3c320-133">Optional.</span></span> <span data-ttu-id="3c320-134">Zoom-Wert auf, falls zutreffend.</span><span class="sxs-lookup"><span data-stu-id="3c320-134">Zoom level to start at, if applicable.</span></span>

## <a name="response"></a><span data-ttu-id="3c320-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="3c320-135">Response</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

<span data-ttu-id="3c320-136">Die Antwort wird ein JSON-Objekt mit den folgenden Eigenschaften werden:</span><span class="sxs-lookup"><span data-stu-id="3c320-136">The response will be a JSON object containing the following properties:</span></span>

| <span data-ttu-id="3c320-137">Name</span><span class="sxs-lookup"><span data-stu-id="3c320-137">Name</span></span>           | <span data-ttu-id="3c320-138">Typ</span><span class="sxs-lookup"><span data-stu-id="3c320-138">Type</span></span>   | <span data-ttu-id="3c320-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3c320-139">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="3c320-140">getUrl</span><span class="sxs-lookup"><span data-stu-id="3c320-140">getUrl</span></span>         | <span data-ttu-id="3c320-141">string</span><span class="sxs-lookup"><span data-stu-id="3c320-141">string</span></span> | <span data-ttu-id="3c320-142">URL für das Einbetten von mit HTTP-GET (Iframes usw.) geeignet</span><span class="sxs-lookup"><span data-stu-id="3c320-142">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="3c320-143">postUrl</span><span class="sxs-lookup"><span data-stu-id="3c320-143">postUrl</span></span>        | <span data-ttu-id="3c320-144">string</span><span class="sxs-lookup"><span data-stu-id="3c320-144">string</span></span> | <span data-ttu-id="3c320-145">URL für das Einbetten von mithilfe von HTTP POST geeignet (bilden, JS, usw..)</span><span class="sxs-lookup"><span data-stu-id="3c320-145">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="3c320-146">postParameters</span><span class="sxs-lookup"><span data-stu-id="3c320-146">postParameters</span></span> | <span data-ttu-id="3c320-147">string</span><span class="sxs-lookup"><span data-stu-id="3c320-147">string</span></span> | <span data-ttu-id="3c320-148">POST-Parameter einschließen, wenn PostUrl verwenden</span><span class="sxs-lookup"><span data-stu-id="3c320-148">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="3c320-149">GetUrl, PostUrl oder beide möglicherweise abhängig vom aktuellen Status des Embed-Unterstützung für den angegebenen Optionen zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3c320-149">Either getUrl, postUrl, or both might be returned depending on the current state of embed support for the specified options.</span></span>

<span data-ttu-id="3c320-150">PostParameters ist eine Zeichenfolge, die als formatiert `application/x-www-form-urlencoded`, und wenn Ausführen von POST an den PostUrl Content-Type entsprechend festgelegt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="3c320-150">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="3c320-151">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="3c320-151">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="pagezoom"></a><span data-ttu-id="3c320-152">Seite/zoom</span><span class="sxs-lookup"><span data-stu-id="3c320-152">Page/zoom</span></span>

<span data-ttu-id="3c320-153">Die Optionen 'zoom' und 'Seite' möglicherweise nicht für alle Preview apps verfügbar, jedoch werden angewendet werden soll, wenn die app Preview unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3c320-153">The 'page' and 'zoom' options may not be available for all preview apps, but will be applied if the preview app supports it.</span></span>
