---
title: 'reportRoot: getYammerActivityUserDetail'
description: Rufen Sie Details zu Yammer-Aktivitäten nach Benutzer ab.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: e0a35141615bbe99a5c022f47ff2c111a93a3dec
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575639"
---
# <a name="reportroot-getyammeractivityuserdetail"></a><span data-ttu-id="f89ee-103">reportRoot: getYammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="f89ee-103">reportRoot: getYammerActivityUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f89ee-104">Rufen Sie Details zu Yammer-Aktivitäten nach Benutzer ab.</span><span class="sxs-lookup"><span data-stu-id="f89ee-104">Get details about Yammer activity by user.</span></span>

> <span data-ttu-id="f89ee-105">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Yammer-Aktivität](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span><span class="sxs-lookup"><span data-stu-id="f89ee-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="permissions"></a><span data-ttu-id="f89ee-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f89ee-106">Permissions</span></span>

<span data-ttu-id="f89ee-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f89ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f89ee-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f89ee-109">Permission type</span></span>                        | <span data-ttu-id="f89ee-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f89ee-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="f89ee-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f89ee-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f89ee-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f89ee-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="f89ee-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f89ee-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f89ee-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f89ee-114">Not supported.</span></span>                           |
| <span data-ttu-id="f89ee-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f89ee-115">Application</span></span>                            | <span data-ttu-id="f89ee-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f89ee-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="f89ee-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f89ee-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerActivityUserDetail(period='{period_value}')
GET /reports/getYammerActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="f89ee-118">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="f89ee-118">Function parameters</span></span>

<span data-ttu-id="f89ee-119">Geben Sie in der Anforderungs-URL einen der folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="f89ee-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="f89ee-120">Parameter</span><span class="sxs-lookup"><span data-stu-id="f89ee-120">Parameter</span></span> | <span data-ttu-id="f89ee-121">Typ</span><span class="sxs-lookup"><span data-stu-id="f89ee-121">Type</span></span>   | <span data-ttu-id="f89ee-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f89ee-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="f89ee-123">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="f89ee-123">period</span></span>    | <span data-ttu-id="f89ee-124">string</span><span class="sxs-lookup"><span data-stu-id="f89ee-124">string</span></span> | <span data-ttu-id="f89ee-125">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="f89ee-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="f89ee-126">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="f89ee-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="f89ee-127">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="f89ee-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="f89ee-128">date</span><span class="sxs-lookup"><span data-stu-id="f89ee-128">date</span></span>      | <span data-ttu-id="f89ee-129">Datum</span><span class="sxs-lookup"><span data-stu-id="f89ee-129">Date</span></span>   | <span data-ttu-id="f89ee-130">Gibt das Datum an, für das die Benutzer angezeigt werden sollen, die Aktivitäten durchgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="f89ee-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="f89ee-131">{date_value} muss im Format JJJJ-MM-TT vorliegen.</span><span class="sxs-lookup"><span data-stu-id="f89ee-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="f89ee-132">Da dieser Bericht nur für die letzten 30 Tage verfügbar ist, sollte {date_value} ein Datum aus diesem Zeitraum sein.</span><span class="sxs-lookup"><span data-stu-id="f89ee-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="f89ee-133">**Hinweis:** Sie müssen in der URL entweder einen Zeitraum oder ein Datum festlegen.</span><span class="sxs-lookup"><span data-stu-id="f89ee-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="f89ee-134">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) von  `$format`, `$top` und `$skipToken` zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f89ee-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="f89ee-135">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="f89ee-135">The default output type is text/csv.</span></span> <span data-ttu-id="f89ee-136">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="f89ee-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f89ee-137">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f89ee-137">Request headers</span></span>

| <span data-ttu-id="f89ee-138">Name</span><span class="sxs-lookup"><span data-stu-id="f89ee-138">Name</span></span>          | <span data-ttu-id="f89ee-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f89ee-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="f89ee-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="f89ee-140">Authorization</span></span> | <span data-ttu-id="f89ee-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f89ee-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="f89ee-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="f89ee-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="f89ee-144">CSV</span><span class="sxs-lookup"><span data-stu-id="f89ee-144">CSV</span></span>

<span data-ttu-id="f89ee-145">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="f89ee-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="f89ee-146">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f89ee-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="f89ee-147">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="f89ee-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="f89ee-148">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="f89ee-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="f89ee-149">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="f89ee-149">Report Refresh Date</span></span>
- <span data-ttu-id="f89ee-150">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="f89ee-150">User Principal Name</span></span>
- <span data-ttu-id="f89ee-151">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="f89ee-151">Display Name</span></span>
- <span data-ttu-id="f89ee-152">Benutzerstatus</span><span class="sxs-lookup"><span data-stu-id="f89ee-152">User State</span></span>
- <span data-ttu-id="f89ee-153">Datum der Statusänderung</span><span class="sxs-lookup"><span data-stu-id="f89ee-153">State Change Date</span></span>
- <span data-ttu-id="f89ee-154">Datum der letzten Aktivität</span><span class="sxs-lookup"><span data-stu-id="f89ee-154">Last Activity Date</span></span>
- <span data-ttu-id="f89ee-155">Anzahl veröffentlicht</span><span class="sxs-lookup"><span data-stu-id="f89ee-155">Posted Count</span></span>
- <span data-ttu-id="f89ee-156">Anzahl gelesen</span><span class="sxs-lookup"><span data-stu-id="f89ee-156">Read Count</span></span>
- <span data-ttu-id="f89ee-157">Anzahl gelikt</span><span class="sxs-lookup"><span data-stu-id="f89ee-157">Liked Count</span></span>
- <span data-ttu-id="f89ee-158">Zugewiesene Produkte</span><span class="sxs-lookup"><span data-stu-id="f89ee-158">Assigned Products</span></span>
- <span data-ttu-id="f89ee-159">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="f89ee-159">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="f89ee-160">JSON</span><span class="sxs-lookup"><span data-stu-id="f89ee-160">JSON</span></span>

<span data-ttu-id="f89ee-161">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines **[YammerActivityUserDetail](../resources/yammeractivityuserdetail.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="f89ee-161">If successful, this method returns a `200 OK` response code and a **[yammerActivityUserDetail](../resources/yammeractivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="f89ee-162">Die Seite Standardgröße für diese Anforderung ist 200 Elemente.</span><span class="sxs-lookup"><span data-stu-id="f89ee-162">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="f89ee-163">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f89ee-163">Example</span></span>

### <a name="csv"></a><span data-ttu-id="f89ee-164">CSV</span><span class="sxs-lookup"><span data-stu-id="f89ee-164">CSV</span></span>

<span data-ttu-id="f89ee-165">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="f89ee-165">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="f89ee-166">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f89ee-166">Request</span></span>

<span data-ttu-id="f89ee-167">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f89ee-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivityuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerActivityUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="f89ee-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="f89ee-168">Response</span></span>

<span data-ttu-id="f89ee-169">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f89ee-169">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="f89ee-170">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="f89ee-170">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,User State,State Change Date,Last Activity Date,Posted Count,Read Count,Liked Count,Assigned Products,Report Period
```

### <a name="json"></a><span data-ttu-id="f89ee-171">JSON</span><span class="sxs-lookup"><span data-stu-id="f89ee-171">JSON</span></span>

<span data-ttu-id="f89ee-172">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f89ee-172">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="f89ee-173">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f89ee-173">Request</span></span>

<span data-ttu-id="f89ee-174">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f89ee-174">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivityuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerActivityUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="f89ee-175">Antwort</span><span class="sxs-lookup"><span data-stu-id="f89ee-175">Response</span></span>

<span data-ttu-id="f89ee-176">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f89ee-176">The following is an example of the response.</span></span>

> <span data-ttu-id="f89ee-p107">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="f89ee-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerActivityUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 434

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerActivityUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "displayName": "displayName-value", 
      "userState": "active", 
      "stateChangeDate": "2015-08-26", 
      "lastActivityDate": "2017-09-01", 
      "postedCount": 2, 
      "readCount": 5, 
      "likedCount": 0, 
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
    "Error: /api-reference/beta/api/reportroot-getyammeractivityuserdetail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
