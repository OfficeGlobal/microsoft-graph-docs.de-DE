---
title: 'reportRoot: getOneDriveUsageAccountDetail'
description: Rufen Sie Details zur OneDrive-Nutzung nach Konto ab.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 0cdc6e0ccdd79484a5edf964213883640e85de6a
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571457"
---
# <a name="reportroot-getonedriveusageaccountdetail"></a><span data-ttu-id="43a4f-103">reportRoot: getOneDriveUsageAccountDetail</span><span class="sxs-lookup"><span data-stu-id="43a4f-103">reportRoot: getOneDriveUsageAccountDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="43a4f-104">Rufen Sie Details zur OneDrive-Nutzung nach Konto ab.</span><span class="sxs-lookup"><span data-stu-id="43a4f-104">Get details about OneDrive usage by account.</span></span>

> <span data-ttu-id="43a4f-105">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – OneDrive for Business-Nutzung](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span><span class="sxs-lookup"><span data-stu-id="43a4f-105">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="43a4f-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="43a4f-106">Permissions</span></span>

<span data-ttu-id="43a4f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43a4f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="43a4f-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="43a4f-109">Permission type</span></span>                        | <span data-ttu-id="43a4f-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="43a4f-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="43a4f-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="43a4f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="43a4f-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="43a4f-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="43a4f-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="43a4f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="43a4f-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="43a4f-114">Not supported.</span></span>                           |
| <span data-ttu-id="43a4f-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="43a4f-115">Application</span></span>                            | <span data-ttu-id="43a4f-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="43a4f-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="43a4f-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="43a4f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageAccountDetail(period='{period_value}')
GET /reports/getOneDriveUsageAccountDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="43a4f-118">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="43a4f-118">Function parameters</span></span>

<span data-ttu-id="43a4f-119">Geben Sie in der Anforderungs-URL einen der folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="43a4f-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="43a4f-120">Parameter</span><span class="sxs-lookup"><span data-stu-id="43a4f-120">Parameter</span></span> | <span data-ttu-id="43a4f-121">Typ</span><span class="sxs-lookup"><span data-stu-id="43a4f-121">Type</span></span>   | <span data-ttu-id="43a4f-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="43a4f-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="43a4f-123">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="43a4f-123">period</span></span>    | <span data-ttu-id="43a4f-124">string</span><span class="sxs-lookup"><span data-stu-id="43a4f-124">string</span></span> | <span data-ttu-id="43a4f-125">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="43a4f-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="43a4f-126">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="43a4f-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="43a4f-127">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="43a4f-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="43a4f-128">date</span><span class="sxs-lookup"><span data-stu-id="43a4f-128">date</span></span>      | <span data-ttu-id="43a4f-129">Datum</span><span class="sxs-lookup"><span data-stu-id="43a4f-129">Date</span></span>   | <span data-ttu-id="43a4f-130">Gibt das Datum an, für das die Benutzer angezeigt werden sollen, die Aktivitäten durchgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="43a4f-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="43a4f-131">{date_value} muss im Format JJJJ-MM-TT vorliegen.</span><span class="sxs-lookup"><span data-stu-id="43a4f-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="43a4f-132">Da dieser Bericht nur für die letzten 30 Tage verfügbar ist, sollte {date_value} ein Datum aus diesem Zeitraum sein.</span><span class="sxs-lookup"><span data-stu-id="43a4f-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="43a4f-133">**Hinweis:** Sie müssen in der URL entweder einen Zeitraum oder ein Datum festlegen.</span><span class="sxs-lookup"><span data-stu-id="43a4f-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="43a4f-134">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) von  `$format`, `$top` und `$skipToken` zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="43a4f-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="43a4f-135">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="43a4f-135">The default output type is text/csv.</span></span> <span data-ttu-id="43a4f-136">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="43a4f-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="43a4f-137">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="43a4f-137">Request headers</span></span>

| <span data-ttu-id="43a4f-138">Name</span><span class="sxs-lookup"><span data-stu-id="43a4f-138">Name</span></span>          | <span data-ttu-id="43a4f-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="43a4f-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="43a4f-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="43a4f-140">Authorization</span></span> | <span data-ttu-id="43a4f-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="43a4f-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="43a4f-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="43a4f-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="43a4f-144">CSV</span><span class="sxs-lookup"><span data-stu-id="43a4f-144">CSV</span></span>

<span data-ttu-id="43a4f-145">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="43a4f-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="43a4f-146">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="43a4f-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="43a4f-147">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="43a4f-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="43a4f-148">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="43a4f-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="43a4f-149">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="43a4f-149">Report Refresh Date</span></span>
- <span data-ttu-id="43a4f-150">Website-URL</span><span class="sxs-lookup"><span data-stu-id="43a4f-150">Site URL</span></span>
- <span data-ttu-id="43a4f-151">Anzeigename des Besitzers</span><span class="sxs-lookup"><span data-stu-id="43a4f-151">Owner Display Name</span></span>
- <span data-ttu-id="43a4f-152">Ist gelöscht</span><span class="sxs-lookup"><span data-stu-id="43a4f-152">Is Deleted</span></span>
- <span data-ttu-id="43a4f-153">Datum der letzten Aktivität</span><span class="sxs-lookup"><span data-stu-id="43a4f-153">Last Activity Date</span></span>
- <span data-ttu-id="43a4f-154">Anzahl der Dateien</span><span class="sxs-lookup"><span data-stu-id="43a4f-154">File Count</span></span>
- <span data-ttu-id="43a4f-155">Anzahl der aktiven Datei</span><span class="sxs-lookup"><span data-stu-id="43a4f-155">Active File Count</span></span>
- <span data-ttu-id="43a4f-156">Verwendeter Speicherplatz (Byte)</span><span class="sxs-lookup"><span data-stu-id="43a4f-156">Storage Used (Byte)</span></span>
- <span data-ttu-id="43a4f-157">Zugewiesener Speicherplatz (Byte)</span><span class="sxs-lookup"><span data-stu-id="43a4f-157">Storage Allocated (Byte)</span></span>
- <span data-ttu-id="43a4f-158">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="43a4f-158">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="43a4f-159">JSON</span><span class="sxs-lookup"><span data-stu-id="43a4f-159">JSON</span></span>

<span data-ttu-id="43a4f-160">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines **[OneDriveUsageAccountDetail](../resources/onedriveusageaccountdetail.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="43a4f-160">If successful, this method returns a `200 OK` response code and a **[oneDriveUsageAccountDetail](../resources/onedriveusageaccountdetail.md)** object in the response body.</span></span>

<span data-ttu-id="43a4f-161">Die Seite Standardgröße für diese Anforderung ist 200 Elemente.</span><span class="sxs-lookup"><span data-stu-id="43a4f-161">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="43a4f-162">Beispiel</span><span class="sxs-lookup"><span data-stu-id="43a4f-162">Example</span></span>

<span data-ttu-id="43a4f-163">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="43a4f-163">The following is an example that outputs CSV.</span></span>

### <a name="csv"></a><span data-ttu-id="43a4f-164">CSV</span><span class="sxs-lookup"><span data-stu-id="43a4f-164">CSV</span></span>

#### <a name="request"></a><span data-ttu-id="43a4f-165">Anforderung</span><span class="sxs-lookup"><span data-stu-id="43a4f-165">Request</span></span>

<span data-ttu-id="43a4f-166">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="43a4f-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="43a4f-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="43a4f-167">Response</span></span>

<span data-ttu-id="43a4f-168">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="43a4f-168">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="43a4f-169">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="43a4f-169">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site URL,Owner Display Name,Is Deleted,Last Activity Date,File Count,Active File Count,Storage Used (Byte),Storage Allocated (Byte),Report Period
```

### <a name="json"></a><span data-ttu-id="43a4f-170">JSON</span><span class="sxs-lookup"><span data-stu-id="43a4f-170">JSON</span></span>

<span data-ttu-id="43a4f-171">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="43a4f-171">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="43a4f-172">Anforderung</span><span class="sxs-lookup"><span data-stu-id="43a4f-172">Request</span></span>

<span data-ttu-id="43a4f-173">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="43a4f-173">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="43a4f-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="43a4f-174">Response</span></span>

<span data-ttu-id="43a4f-175">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="43a4f-175">The following is an example of the response.</span></span>

> <span data-ttu-id="43a4f-p107">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="43a4f-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oneDriveUsageAccountDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 400

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.oneDriveUsageAccountDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteUrl": "siteUrl-value", 
      "ownerDisplayName": "ownerDisplayName-value", 
      "isDeleted": false, 
      "lastActivityDate": "2017-09-01", 
      "fileCount": 9, 
      "activeFileCount": 5, 
      "storageUsedInBytes": 12190375, 
      "storageAllocatedInBytes": 549755813880, 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getonedriveusageaccountdetail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
