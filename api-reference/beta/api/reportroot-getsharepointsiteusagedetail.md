---
title: 'reportRoot: getSharePointSiteUsageDetail'
description: Abrufen von Details zur SharePoint-Websiteverwendung.
ms.openlocfilehash: 58c51bfcc14f3478a53c45f66f64ce7dc547ea6b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062890"
---
# <a name="reportroot-getsharepointsiteusagedetail"></a><span data-ttu-id="fa331-103">reportRoot: getSharePointSiteUsageDetail</span><span class="sxs-lookup"><span data-stu-id="fa331-103">reportRoot: getSharePointSiteUsageDetail</span></span>

> <span data-ttu-id="fa331-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="fa331-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fa331-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fa331-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fa331-106">Abrufen von Details zur SharePoint-Websiteverwendung.</span><span class="sxs-lookup"><span data-stu-id="fa331-106">Get details about SharePoint site usage.</span></span>

> <span data-ttu-id="fa331-107">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – SharePoint-Websiteverwendung](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span><span class="sxs-lookup"><span data-stu-id="fa331-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="fa331-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="fa331-108">Permissions</span></span>

<span data-ttu-id="fa331-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa331-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fa331-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fa331-111">Permission type</span></span>                        | <span data-ttu-id="fa331-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fa331-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="fa331-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fa331-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="fa331-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fa331-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="fa331-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fa331-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa331-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fa331-116">Not supported.</span></span>                           |
| <span data-ttu-id="fa331-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fa331-117">Application</span></span>                            | <span data-ttu-id="fa331-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fa331-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="fa331-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fa331-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageDetail(period='{period_value}')
GET /reports/getSharePointSiteUsageDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="fa331-120">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="fa331-120">Function parameters</span></span>

<span data-ttu-id="fa331-121">Geben Sie in der Anforderungs-URL einen der folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="fa331-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="fa331-122">Parameter</span><span class="sxs-lookup"><span data-stu-id="fa331-122">Parameter</span></span> | <span data-ttu-id="fa331-123">Typ</span><span class="sxs-lookup"><span data-stu-id="fa331-123">Type</span></span>   | <span data-ttu-id="fa331-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fa331-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="fa331-125">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="fa331-125">period</span></span>    | <span data-ttu-id="fa331-126">string</span><span class="sxs-lookup"><span data-stu-id="fa331-126">string</span></span> | <span data-ttu-id="fa331-127">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="fa331-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="fa331-128">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="fa331-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="fa331-129">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="fa331-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="fa331-130">date</span><span class="sxs-lookup"><span data-stu-id="fa331-130">date</span></span>      | <span data-ttu-id="fa331-131">Datum</span><span class="sxs-lookup"><span data-stu-id="fa331-131">Date</span></span>   | <span data-ttu-id="fa331-132">Gibt das Datum an, für das die Benutzer angezeigt werden sollen, die Aktivitäten durchgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="fa331-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="fa331-133">{date_value} muss im Format JJJJ-MM-TT vorliegen.</span><span class="sxs-lookup"><span data-stu-id="fa331-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="fa331-134">Da dieser Bericht nur für die letzten 30 Tage verfügbar ist, sollte {date_value} ein Datum aus diesem Zeitraum sein.</span><span class="sxs-lookup"><span data-stu-id="fa331-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="fa331-135">**Hinweis:** Sie müssen in der URL entweder einen Zeitraum oder ein Datum festlegen.</span><span class="sxs-lookup"><span data-stu-id="fa331-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="fa331-136">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) von  `$format`, `$top` und `$skipToken` zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="fa331-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="fa331-137">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="fa331-137">The default output type is text/csv.</span></span> <span data-ttu-id="fa331-138">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="fa331-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fa331-139">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fa331-139">Request headers</span></span>

| <span data-ttu-id="fa331-140">Name</span><span class="sxs-lookup"><span data-stu-id="fa331-140">Name</span></span>          | <span data-ttu-id="fa331-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fa331-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="fa331-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa331-142">Authorization</span></span> | <span data-ttu-id="fa331-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fa331-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="fa331-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="fa331-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="fa331-146">CSV</span><span class="sxs-lookup"><span data-stu-id="fa331-146">CSV</span></span>

<span data-ttu-id="fa331-147">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="fa331-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="fa331-148">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="fa331-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="fa331-149">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="fa331-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="fa331-150">Die CSV-Datei verfügt über die folgenden Spaltenheader:</span><span class="sxs-lookup"><span data-stu-id="fa331-150">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="fa331-151">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="fa331-151">Report Refresh Date</span></span>
- <span data-ttu-id="fa331-152">Site-Id</span><span class="sxs-lookup"><span data-stu-id="fa331-152">Site Id</span></span>
- <span data-ttu-id="fa331-153">Website-URL</span><span class="sxs-lookup"><span data-stu-id="fa331-153">Site URL</span></span>
- <span data-ttu-id="fa331-154">Anzeigename des Besitzers</span><span class="sxs-lookup"><span data-stu-id="fa331-154">Owner Display Name</span></span>
- <span data-ttu-id="fa331-155">Ist gelöscht</span><span class="sxs-lookup"><span data-stu-id="fa331-155">Is Deleted</span></span>
- <span data-ttu-id="fa331-156">Datum der letzten Aktivität</span><span class="sxs-lookup"><span data-stu-id="fa331-156">Last Activity Date</span></span>
- <span data-ttu-id="fa331-157">Anzahl der Dateien</span><span class="sxs-lookup"><span data-stu-id="fa331-157">File Count</span></span>
- <span data-ttu-id="fa331-158">Anzahl der aktiven Datei</span><span class="sxs-lookup"><span data-stu-id="fa331-158">Active File Count</span></span>
- <span data-ttu-id="fa331-159">Anzahl der angezeigten Seiten</span><span class="sxs-lookup"><span data-stu-id="fa331-159">Page View Count</span></span>
- <span data-ttu-id="fa331-160">Anzahl der besuchten Seiten</span><span class="sxs-lookup"><span data-stu-id="fa331-160">Visited Page Count</span></span>
- <span data-ttu-id="fa331-161">Verwendeter Speicherplatz (Byte)</span><span class="sxs-lookup"><span data-stu-id="fa331-161">Storage Used (Byte)</span></span>
- <span data-ttu-id="fa331-162">Zugewiesener Speicherplatz (Byte)</span><span class="sxs-lookup"><span data-stu-id="fa331-162">Storage Allocated (Byte)</span></span>
- <span data-ttu-id="fa331-163">Stammweb-Vorlage</span><span class="sxs-lookup"><span data-stu-id="fa331-163">Root Web Template</span></span>
- <span data-ttu-id="fa331-164">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="fa331-164">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="fa331-165">JSON</span><span class="sxs-lookup"><span data-stu-id="fa331-165">JSON</span></span>

<span data-ttu-id="fa331-166">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines **[SharePointSiteUsageDetail](../resources/sharepointsiteusagedetail.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="fa331-166">If successful, this method returns a `200 OK` response code and a **[sharePointSiteUsageDetail](../resources/sharepointsiteusagedetail.md)** object in the response body.</span></span>

<span data-ttu-id="fa331-167">Die Seite Standardgröße für diese Anforderung ist 200 Elemente.</span><span class="sxs-lookup"><span data-stu-id="fa331-167">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="fa331-168">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fa331-168">Example</span></span>

### <a name="csv"></a><span data-ttu-id="fa331-169">CSV</span><span class="sxs-lookup"><span data-stu-id="fa331-169">CSV</span></span>

<span data-ttu-id="fa331-170">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="fa331-170">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="fa331-171">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fa331-171">Request</span></span>

<span data-ttu-id="fa331-172">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fa331-172">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagedetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="fa331-173">Antwort</span><span class="sxs-lookup"><span data-stu-id="fa331-173">Response</span></span>

<span data-ttu-id="fa331-174">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="fa331-174">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="fa331-175">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="fa331-175">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Id,Site URL,Owner Display Name,Is Deleted,Last Activity Date,File Count,Active File Count,Page View Count,Visited Page Count,Storage Used (Byte),Storage Allocated (Byte),Root Web Template,Report Period
```

### <a name="json"></a><span data-ttu-id="fa331-176">JSON</span><span class="sxs-lookup"><span data-stu-id="fa331-176">JSON</span></span>

<span data-ttu-id="fa331-177">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fa331-177">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="fa331-178">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fa331-178">Request</span></span>

<span data-ttu-id="fa331-179">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fa331-179">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagedetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="fa331-180">Antwort</span><span class="sxs-lookup"><span data-stu-id="fa331-180">Response</span></span>

<span data-ttu-id="fa331-181">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="fa331-181">The following is an example of the response.</span></span>

> <span data-ttu-id="fa331-p108">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="fa331-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharePointSiteUsageDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 484

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.sharePointSiteUsageDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteId": "siteId-value", 
      "siteUrl": "siteUrl-value", 
      "ownerDisplayName": "ownerDisplayName-value", 
      "isDeleted": false, 
      "lastActivityDate": "2017-09-01", 
      "fileCount": 170, 
      "activeFileCount": 25, 
      "pageViewCount": 7, 
      "visitedPageCount": 3, 
      "storageUsedInBytes": 63442116, 
      "storageAllocatedInBytes": 2748779094400, 
      "rootWebTemplate": "Publishing Site", 
      "reportPeriod": "7"
    }
  ]
}
```
