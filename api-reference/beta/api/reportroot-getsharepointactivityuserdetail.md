---
title: 'reportRoot: getSharePointActivityUserDetail'
description: Rufen Sie Details zu SharePoint-Aktivitäten nach Benutzer ab.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: af63d1b995dd182ce37b0f39b6a0533c25f56f3d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521852"
---
# <a name="reportroot-getsharepointactivityuserdetail"></a><span data-ttu-id="2f6c0-103">reportRoot: getSharePointActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="2f6c0-103">reportRoot: getSharePointActivityUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f6c0-104">Rufen Sie Details zu SharePoint-Aktivitäten nach Benutzer ab.</span><span class="sxs-lookup"><span data-stu-id="2f6c0-104">Get details about SharePoint activity by user.</span></span>

> <span data-ttu-id="2f6c0-105">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – SharePoint-Aktivität](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="2f6c0-105">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="2f6c0-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2f6c0-106">Permissions</span></span>

<span data-ttu-id="2f6c0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f6c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2f6c0-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2f6c0-109">Permission type</span></span>                        | <span data-ttu-id="2f6c0-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2f6c0-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="2f6c0-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2f6c0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2f6c0-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f6c0-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="2f6c0-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2f6c0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f6c0-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2f6c0-114">Not supported.</span></span>                           |
| <span data-ttu-id="2f6c0-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2f6c0-115">Application</span></span>                            | <span data-ttu-id="2f6c0-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f6c0-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="2f6c0-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2f6c0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityUserDetail(period='{period_value}')
GET /reports/getSharePointActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="2f6c0-118">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="2f6c0-118">Function parameters</span></span>

<span data-ttu-id="2f6c0-119">Geben Sie in der Anforderungs-URL einen der folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="2f6c0-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="2f6c0-120">Parameter</span><span class="sxs-lookup"><span data-stu-id="2f6c0-120">Parameter</span></span> | <span data-ttu-id="2f6c0-121">Typ</span><span class="sxs-lookup"><span data-stu-id="2f6c0-121">Type</span></span>   | <span data-ttu-id="2f6c0-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2f6c0-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="2f6c0-123">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="2f6c0-123">period</span></span>    | <span data-ttu-id="2f6c0-124">string</span><span class="sxs-lookup"><span data-stu-id="2f6c0-124">string</span></span> | <span data-ttu-id="2f6c0-125">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="2f6c0-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="2f6c0-126">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="2f6c0-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="2f6c0-127">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="2f6c0-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="2f6c0-128">date</span><span class="sxs-lookup"><span data-stu-id="2f6c0-128">date</span></span>      | <span data-ttu-id="2f6c0-129">Datum</span><span class="sxs-lookup"><span data-stu-id="2f6c0-129">Date</span></span>   | <span data-ttu-id="2f6c0-130">Gibt das Datum an, für das die Benutzer angezeigt werden sollen, die Aktivitäten durchgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="2f6c0-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="2f6c0-131">{date_value} muss im Format JJJJ-MM-TT vorliegen.</span><span class="sxs-lookup"><span data-stu-id="2f6c0-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="2f6c0-132">Da dieser Bericht nur für die letzten 30 Tage verfügbar ist, sollte {date_value} ein Datum aus diesem Zeitraum sein.</span><span class="sxs-lookup"><span data-stu-id="2f6c0-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="2f6c0-133">**Hinweis:** Sie müssen in der URL entweder einen Zeitraum oder ein Datum festlegen.</span><span class="sxs-lookup"><span data-stu-id="2f6c0-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="2f6c0-134">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) von  `$format`, `$top` und `$skipToken` zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2f6c0-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="2f6c0-135">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="2f6c0-135">The default output type is text/csv.</span></span> <span data-ttu-id="2f6c0-136">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="2f6c0-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2f6c0-137">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2f6c0-137">Request headers</span></span>

| <span data-ttu-id="2f6c0-138">Name</span><span class="sxs-lookup"><span data-stu-id="2f6c0-138">Name</span></span>          | <span data-ttu-id="2f6c0-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2f6c0-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="2f6c0-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f6c0-140">Authorization</span></span> | <span data-ttu-id="2f6c0-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2f6c0-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="2f6c0-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="2f6c0-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="2f6c0-144">CSV</span><span class="sxs-lookup"><span data-stu-id="2f6c0-144">CSV</span></span>

<span data-ttu-id="2f6c0-145">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="2f6c0-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="2f6c0-146">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2f6c0-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="2f6c0-147">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="2f6c0-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="2f6c0-148">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="2f6c0-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="2f6c0-149">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="2f6c0-149">Report Refresh Date</span></span>
- <span data-ttu-id="2f6c0-150">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="2f6c0-150">User Principal Name</span></span>
- <span data-ttu-id="2f6c0-151">Ist gelöscht</span><span class="sxs-lookup"><span data-stu-id="2f6c0-151">Is Deleted</span></span>
- <span data-ttu-id="2f6c0-152">Gelöscht am</span><span class="sxs-lookup"><span data-stu-id="2f6c0-152">Deleted Date</span></span>
- <span data-ttu-id="2f6c0-153">Datum der letzten Aktivität</span><span class="sxs-lookup"><span data-stu-id="2f6c0-153">Last Activity Date</span></span>
- <span data-ttu-id="2f6c0-154">Anzahl der angezeigten oder bearbeiteten Dateien</span><span class="sxs-lookup"><span data-stu-id="2f6c0-154">Viewed Or Edited File Count</span></span>
- <span data-ttu-id="2f6c0-155">Anzahl der synchronisierten Dateien</span><span class="sxs-lookup"><span data-stu-id="2f6c0-155">Synced File Count</span></span>
- <span data-ttu-id="2f6c0-156">Anzahl der intern freigegebenen Dateien</span><span class="sxs-lookup"><span data-stu-id="2f6c0-156">Shared Internally File Count</span></span>
- <span data-ttu-id="2f6c0-157">Anzahl der extern freigegebenen Dateien</span><span class="sxs-lookup"><span data-stu-id="2f6c0-157">Shared Externally File Count</span></span>
- <span data-ttu-id="2f6c0-158">Anzahl der besuchten Seiten</span><span class="sxs-lookup"><span data-stu-id="2f6c0-158">Visited Page Count</span></span>
- <span data-ttu-id="2f6c0-159">Zugewiesene Produkte</span><span class="sxs-lookup"><span data-stu-id="2f6c0-159">Assigned Products</span></span>
- <span data-ttu-id="2f6c0-160">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="2f6c0-160">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="2f6c0-161">JSON</span><span class="sxs-lookup"><span data-stu-id="2f6c0-161">JSON</span></span>

<span data-ttu-id="2f6c0-162">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines **[SharePointActivityUserDetail](../resources/sharepointactivityuserdetail.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="2f6c0-162">If successful, this method returns a `200 OK` response code and a **[sharePointActivityUserDetail](../resources/sharepointactivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="2f6c0-163">Die Seite Standardgröße für diese Anforderung ist 200 Elemente.</span><span class="sxs-lookup"><span data-stu-id="2f6c0-163">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="2f6c0-164">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2f6c0-164">Example</span></span>

### <a name="csv"></a><span data-ttu-id="2f6c0-165">CSV</span><span class="sxs-lookup"><span data-stu-id="2f6c0-165">CSV</span></span>

<span data-ttu-id="2f6c0-166">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="2f6c0-166">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="2f6c0-167">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2f6c0-167">Request</span></span>

<span data-ttu-id="2f6c0-168">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2f6c0-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivityuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="2f6c0-169">Antwort</span><span class="sxs-lookup"><span data-stu-id="2f6c0-169">Response</span></span>

<span data-ttu-id="2f6c0-170">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2f6c0-170">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="2f6c0-171">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="2f6c0-171">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Is Deleted,Deleted Date,Last Activity Date,Viewed Or Edited File Count,Synced File Count,Shared Internally File Count,Shared Externally File Count,Visited Page Count,Assigned Products,Report Period
```

### <a name="json"></a><span data-ttu-id="2f6c0-172">JSON</span><span class="sxs-lookup"><span data-stu-id="2f6c0-172">JSON</span></span>

<span data-ttu-id="2f6c0-173">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2f6c0-173">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="2f6c0-174">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2f6c0-174">Request</span></span>

<span data-ttu-id="2f6c0-175">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2f6c0-175">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivityuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="2f6c0-176">Antwort</span><span class="sxs-lookup"><span data-stu-id="2f6c0-176">Response</span></span>

<span data-ttu-id="2f6c0-177">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2f6c0-177">The following is an example of the response.</span></span>

> <span data-ttu-id="2f6c0-p107">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="2f6c0-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharePointActivityUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 473

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.sharePointActivityUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "isDeleted": false, 
      "deletedDate": null, 
      "lastActivityDate": "2017-09-01", 
      "viewedOrEditedFileCount": 4, 
      "syncedFileCount": 0, 
      "sharedInternallyFileCount": 0, 
      "sharedExternallyFileCount": 0, 
      "visitedPageCount": 1, 
      "assignedProducts": [
        "OFFICE 365 ENTERPRISE E5"
      ], 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getsharepointactivityuserdetail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
