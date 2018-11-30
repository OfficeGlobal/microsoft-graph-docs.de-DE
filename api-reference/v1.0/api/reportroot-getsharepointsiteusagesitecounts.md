---
title: 'reportRoot: getSharePointSiteUsageSiteCounts'
description: Rufen Sie die Gesamtzahl der Dateien auf allen Websites und die Anzahl der aktiven Dateien ab. Eine Datei (Benutzer oder System) wird als aktiv betrachtet, wenn sie innerhalb des angegebenen Zeitraums gespeichert, synchronisiert, geändert oder freigegeben wurde.
ms.openlocfilehash: d5d3f3b104fbed49ce669b0d6051fc2a3ef13b0d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018236"
---
# <a name="reportroot-getsharepointsiteusagesitecounts"></a><span data-ttu-id="3b29c-104">reportRoot: getSharePointSiteUsageSiteCounts</span><span class="sxs-lookup"><span data-stu-id="3b29c-104">reportRoot: getSharePointSiteUsageSiteCounts</span></span>

<span data-ttu-id="3b29c-105">Rufen Sie die Gesamtzahl der Dateien auf allen Websites und die Anzahl der aktiven Dateien ab.</span><span class="sxs-lookup"><span data-stu-id="3b29c-105">Get the total number of files across all sites and the number of active files.</span></span> <span data-ttu-id="3b29c-106">Eine Datei (Benutzer oder System) wird als aktiv betrachtet, wenn sie innerhalb des angegebenen Zeitraums gespeichert, synchronisiert, geändert oder freigegeben wurde.</span><span class="sxs-lookup"><span data-stu-id="3b29c-106">A file (user or system) is considered active if it has been saved, synced, modified, or shared within the specified time period.</span></span>

> <span data-ttu-id="3b29c-107">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – SharePoint-Websiteverwendung](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span><span class="sxs-lookup"><span data-stu-id="3b29c-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="3b29c-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3b29c-108">Permissions</span></span>

<span data-ttu-id="3b29c-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b29c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3b29c-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3b29c-111">Permission type</span></span>                        | <span data-ttu-id="3b29c-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3b29c-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="3b29c-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3b29c-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="3b29c-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3b29c-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="3b29c-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3b29c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b29c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3b29c-116">Not supported.</span></span>                           |
| <span data-ttu-id="3b29c-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3b29c-117">Application</span></span>                            | <span data-ttu-id="3b29c-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3b29c-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="3b29c-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3b29c-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageSiteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="3b29c-120">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="3b29c-120">Function parameters</span></span>

<span data-ttu-id="3b29c-121">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="3b29c-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="3b29c-122">Parameter</span><span class="sxs-lookup"><span data-stu-id="3b29c-122">Parameter</span></span> | <span data-ttu-id="3b29c-123">Typ</span><span class="sxs-lookup"><span data-stu-id="3b29c-123">Type</span></span>   | <span data-ttu-id="3b29c-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3b29c-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="3b29c-125">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="3b29c-125">period</span></span>    | <span data-ttu-id="3b29c-126">string</span><span class="sxs-lookup"><span data-stu-id="3b29c-126">string</span></span> | <span data-ttu-id="3b29c-127">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="3b29c-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="3b29c-128">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="3b29c-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="3b29c-129">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="3b29c-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="3b29c-130">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="3b29c-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="3b29c-131">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3b29c-131">Request headers</span></span>

| <span data-ttu-id="3b29c-132">Name</span><span class="sxs-lookup"><span data-stu-id="3b29c-132">Name</span></span>          | <span data-ttu-id="3b29c-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3b29c-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="3b29c-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b29c-134">Authorization</span></span> | <span data-ttu-id="3b29c-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3b29c-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="3b29c-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="3b29c-137">If-None-Match</span></span> | <span data-ttu-id="3b29c-138">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3b29c-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="3b29c-139">Optional.</span><span class="sxs-lookup"><span data-stu-id="3b29c-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="3b29c-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="3b29c-140">Response</span></span>

<span data-ttu-id="3b29c-141">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="3b29c-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="3b29c-142">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3b29c-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="3b29c-143">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="3b29c-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="3b29c-144">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="3b29c-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="3b29c-145">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="3b29c-145">Report Refresh Date</span></span>
- <span data-ttu-id="3b29c-146">Websitetyp</span><span class="sxs-lookup"><span data-stu-id="3b29c-146">Site Type</span></span>
- <span data-ttu-id="3b29c-147">Gesamt</span><span class="sxs-lookup"><span data-stu-id="3b29c-147">Total</span></span>
- <span data-ttu-id="3b29c-148">Aktiv</span><span class="sxs-lookup"><span data-stu-id="3b29c-148">Active</span></span>
- <span data-ttu-id="3b29c-149">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="3b29c-149">Report Date</span></span>
- <span data-ttu-id="3b29c-150">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="3b29c-150">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="3b29c-151">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3b29c-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="3b29c-152">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3b29c-152">Request</span></span>

<span data-ttu-id="3b29c-153">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3b29c-153">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getsharepointsiteusagesitecounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointSiteUsageSiteCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="3b29c-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="3b29c-154">Response</span></span>

<span data-ttu-id="3b29c-155">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3b29c-155">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.report"
} -->

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="3b29c-156">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="3b29c-156">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Total,Active,Report Date,Report Period
```