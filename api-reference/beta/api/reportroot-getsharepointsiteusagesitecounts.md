---
title: 'reportRoot: getSharePointSiteUsageSiteCounts'
description: Rufen Sie die Gesamtzahl der Dateien auf allen Websites und die Anzahl der aktiven Dateien ab. Eine Datei (Benutzer oder System) wird als aktiv betrachtet, wenn sie innerhalb des angegebenen Zeitraums gespeichert, synchronisiert, geändert oder freigegeben wurde.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: c3dfaf628f33102016b57cab12c720a28f3d4ebd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27973174"
---
# <a name="reportroot-getsharepointsiteusagesitecounts"></a><span data-ttu-id="ac113-104">reportRoot: getSharePointSiteUsageSiteCounts</span><span class="sxs-lookup"><span data-stu-id="ac113-104">reportRoot: getSharePointSiteUsageSiteCounts</span></span>

> <span data-ttu-id="ac113-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ac113-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ac113-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ac113-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ac113-107">Rufen Sie die Gesamtzahl der Dateien auf allen Websites und die Anzahl der aktiven Dateien ab.</span><span class="sxs-lookup"><span data-stu-id="ac113-107">Get the total number of files across all sites and the number of active files.</span></span> <span data-ttu-id="ac113-108">Eine Datei (Benutzer oder System) wird als aktiv betrachtet, wenn sie innerhalb des angegebenen Zeitraums gespeichert, synchronisiert, geändert oder freigegeben wurde.</span><span class="sxs-lookup"><span data-stu-id="ac113-108">A file (user or system) is considered active if it has been saved, synced, modified, or shared within the specified time period.</span></span>

> <span data-ttu-id="ac113-109">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – SharePoint-Websiteverwendung](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span><span class="sxs-lookup"><span data-stu-id="ac113-109">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="ac113-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ac113-110">Permissions</span></span>

<span data-ttu-id="ac113-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac113-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ac113-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ac113-113">Permission type</span></span>                        | <span data-ttu-id="ac113-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ac113-114">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ac113-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ac113-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="ac113-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ac113-116">Reports.Read.All</span></span>                         |
| <span data-ttu-id="ac113-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ac113-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac113-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ac113-118">Not supported.</span></span>                           |
| <span data-ttu-id="ac113-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ac113-119">Application</span></span>                            | <span data-ttu-id="ac113-120">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ac113-120">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="ac113-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ac113-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageSiteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="ac113-122">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="ac113-122">Function parameters</span></span>

<span data-ttu-id="ac113-123">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="ac113-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="ac113-124">Parameter</span><span class="sxs-lookup"><span data-stu-id="ac113-124">Parameter</span></span> | <span data-ttu-id="ac113-125">Typ</span><span class="sxs-lookup"><span data-stu-id="ac113-125">Type</span></span>   | <span data-ttu-id="ac113-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ac113-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="ac113-127">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="ac113-127">period</span></span>    | <span data-ttu-id="ac113-128">string</span><span class="sxs-lookup"><span data-stu-id="ac113-128">string</span></span> | <span data-ttu-id="ac113-129">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="ac113-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="ac113-130">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="ac113-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="ac113-131">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="ac113-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="ac113-132">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="ac113-132">Required.</span></span> |

<span data-ttu-id="ac113-133">Diese Methode unterstützt die `$format` [OData-Abfragezeichenfolgen-Parameter](/graph/query-parameters) zum Anpassen der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ac113-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="ac113-134">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="ac113-134">The default output type is text/csv.</span></span> <span data-ttu-id="ac113-135">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="ac113-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ac113-136">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ac113-136">Request headers</span></span>

| <span data-ttu-id="ac113-137">Name</span><span class="sxs-lookup"><span data-stu-id="ac113-137">Name</span></span>          | <span data-ttu-id="ac113-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ac113-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="ac113-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="ac113-139">Authorization</span></span> | <span data-ttu-id="ac113-p107">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ac113-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="ac113-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="ac113-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="ac113-143">CSV</span><span class="sxs-lookup"><span data-stu-id="ac113-143">CSV</span></span>

<span data-ttu-id="ac113-144">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="ac113-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ac113-145">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ac113-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ac113-146">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="ac113-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="ac113-147">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="ac113-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="ac113-148">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="ac113-148">Report Refresh Date</span></span>
- <span data-ttu-id="ac113-149">Websitetyp</span><span class="sxs-lookup"><span data-stu-id="ac113-149">Site Type</span></span>
- <span data-ttu-id="ac113-150">Gesamt</span><span class="sxs-lookup"><span data-stu-id="ac113-150">Total</span></span>
- <span data-ttu-id="ac113-151">Aktiv</span><span class="sxs-lookup"><span data-stu-id="ac113-151">Active</span></span>
- <span data-ttu-id="ac113-152">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="ac113-152">Report Date</span></span>
- <span data-ttu-id="ac113-153">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="ac113-153">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="ac113-154">JSON</span><span class="sxs-lookup"><span data-stu-id="ac113-154">JSON</span></span>

<span data-ttu-id="ac113-155">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines **[SharePointSiteUsageSiteCounts](../resources/sharepointsiteusagesitecounts.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="ac113-155">If successful, this method returns a `200 OK` response code and a **[sharePointSiteUsageSiteCounts](../resources/sharepointsiteusagesitecounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac113-156">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ac113-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="ac113-157">CSV</span><span class="sxs-lookup"><span data-stu-id="ac113-157">CSV</span></span>

<span data-ttu-id="ac113-158">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="ac113-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="ac113-159">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ac113-159">Request</span></span>

<span data-ttu-id="ac113-160">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ac113-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagesitecounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageSiteCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="ac113-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="ac113-161">Response</span></span>

<span data-ttu-id="ac113-162">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ac113-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="ac113-163">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="ac113-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Total,Active,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="ac113-164">JSON</span><span class="sxs-lookup"><span data-stu-id="ac113-164">JSON</span></span>

<span data-ttu-id="ac113-165">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ac113-165">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="ac113-166">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ac113-166">Request</span></span>

<span data-ttu-id="ac113-167">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ac113-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagesitecounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageSiteCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="ac113-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="ac113-168">Response</span></span>

<span data-ttu-id="ac113-169">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ac113-169">The following is an example of the response.</span></span>

> <span data-ttu-id="ac113-p109">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="ac113-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharePointSiteUsageSiteCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 251

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.sharePointSiteUsageSiteCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteType": "All", 
      "total": 47, 
      "active": 15, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
