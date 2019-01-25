---
title: 'reportRoot: getYammerDeviceUsageUserDetail function'
description: Rufen Sie Details zur Yammer-Gerätenutzung nach Benutzer ab.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 169a0b4850d3ddb72ad77e89833cf51133edc378
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524485"
---
# <a name="reportroot-getyammerdeviceusageuserdetail-function"></a><span data-ttu-id="41d83-103">reportRoot: getYammerDeviceUsageUserDetail function</span><span class="sxs-lookup"><span data-stu-id="41d83-103">reportRoot: getYammerDeviceUsageUserDetail function</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41d83-104">Rufen Sie Details zur Yammer-Gerätenutzung nach Benutzer ab.</span><span class="sxs-lookup"><span data-stu-id="41d83-104">Get details about Yammer device usage by user.</span></span>

> <span data-ttu-id="41d83-105">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Yammer-Gerätenutzung](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="41d83-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="41d83-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="41d83-106">Permissions</span></span>

<span data-ttu-id="41d83-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41d83-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="41d83-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="41d83-109">Permission type</span></span>                        | <span data-ttu-id="41d83-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="41d83-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="41d83-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="41d83-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="41d83-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="41d83-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="41d83-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="41d83-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41d83-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="41d83-114">Not supported.</span></span>                           |
| <span data-ttu-id="41d83-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="41d83-115">Application</span></span>                            | <span data-ttu-id="41d83-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="41d83-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="41d83-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="41d83-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageUserDetail(period='{period_value}')
GET /reports/getYammerDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="41d83-118">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="41d83-118">Function parameters</span></span>

<span data-ttu-id="41d83-119">Geben Sie in der Anforderungs-URL einen der folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="41d83-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="41d83-120">Parameter</span><span class="sxs-lookup"><span data-stu-id="41d83-120">Parameter</span></span> | <span data-ttu-id="41d83-121">Typ</span><span class="sxs-lookup"><span data-stu-id="41d83-121">Type</span></span>   | <span data-ttu-id="41d83-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="41d83-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="41d83-123">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="41d83-123">period</span></span>    | <span data-ttu-id="41d83-124">string</span><span class="sxs-lookup"><span data-stu-id="41d83-124">string</span></span> | <span data-ttu-id="41d83-125">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="41d83-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="41d83-126">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="41d83-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="41d83-127">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="41d83-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="41d83-128">date</span><span class="sxs-lookup"><span data-stu-id="41d83-128">date</span></span>      | <span data-ttu-id="41d83-129">Datum</span><span class="sxs-lookup"><span data-stu-id="41d83-129">Date</span></span>   | <span data-ttu-id="41d83-130">Gibt das Datum an, für das die Benutzer angezeigt werden sollen, die Aktivitäten durchgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="41d83-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="41d83-131">{date_value} muss im Format JJJJ-MM-TT vorliegen.</span><span class="sxs-lookup"><span data-stu-id="41d83-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="41d83-132">Da dieser Bericht nur für die letzten 30 Tage verfügbar ist, sollte {date_value} ein Datum aus diesem Zeitraum sein.</span><span class="sxs-lookup"><span data-stu-id="41d83-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="41d83-133">**Hinweis:** Sie müssen in der URL entweder einen Zeitraum oder ein Datum festlegen.</span><span class="sxs-lookup"><span data-stu-id="41d83-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="41d83-134">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) von  `$format`, `$top` und `$skipToken` zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="41d83-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="41d83-135">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="41d83-135">The default output type is text/csv.</span></span> <span data-ttu-id="41d83-136">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="41d83-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="41d83-137">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="41d83-137">Request headers</span></span>

| <span data-ttu-id="41d83-138">Name</span><span class="sxs-lookup"><span data-stu-id="41d83-138">Name</span></span>          | <span data-ttu-id="41d83-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="41d83-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="41d83-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="41d83-140">Authorization</span></span> | <span data-ttu-id="41d83-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="41d83-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="41d83-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="41d83-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="41d83-144">CSV</span><span class="sxs-lookup"><span data-stu-id="41d83-144">CSV</span></span>

<span data-ttu-id="41d83-145">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="41d83-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="41d83-146">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="41d83-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="41d83-147">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="41d83-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="41d83-148">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="41d83-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="41d83-149">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="41d83-149">Report Refresh Date</span></span>
- <span data-ttu-id="41d83-150">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="41d83-150">User Principal Name</span></span>
- <span data-ttu-id="41d83-151">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="41d83-151">Display Name</span></span>
- <span data-ttu-id="41d83-152">Benutzerstatus</span><span class="sxs-lookup"><span data-stu-id="41d83-152">User State</span></span>
- <span data-ttu-id="41d83-153">Datum der Statusänderung</span><span class="sxs-lookup"><span data-stu-id="41d83-153">State Change Date</span></span>
- <span data-ttu-id="41d83-154">Datum der letzten Aktivität</span><span class="sxs-lookup"><span data-stu-id="41d83-154">Last Activity Date</span></span>
- <span data-ttu-id="41d83-155">Verwendetes Web</span><span class="sxs-lookup"><span data-stu-id="41d83-155">Used Web</span></span>
- <span data-ttu-id="41d83-156">Verwendetes Windows Phone</span><span class="sxs-lookup"><span data-stu-id="41d83-156">Used Windows Phone</span></span>
- <span data-ttu-id="41d83-157">Verwendetes Android Phone</span><span class="sxs-lookup"><span data-stu-id="41d83-157">Used Android Phone</span></span>
- <span data-ttu-id="41d83-158">Verwendetes iPhone</span><span class="sxs-lookup"><span data-stu-id="41d83-158">Used iPhone</span></span>
- <span data-ttu-id="41d83-159">Verwendetes iPad</span><span class="sxs-lookup"><span data-stu-id="41d83-159">Used iPad</span></span>
- <span data-ttu-id="41d83-160">Andere verwendet</span><span class="sxs-lookup"><span data-stu-id="41d83-160">Used Others</span></span>
- <span data-ttu-id="41d83-161">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="41d83-161">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="41d83-162">JSON</span><span class="sxs-lookup"><span data-stu-id="41d83-162">JSON</span></span>

<span data-ttu-id="41d83-163">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines **[YammerDeviceUsageUserDetail](../resources/yammerdeviceusageuserdetail.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="41d83-163">If successful, this method returns a `200 OK` response code and a **[yammerDeviceUsageUserDetail](../resources/yammerdeviceusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="41d83-164">Die Seite Standardgröße für diese Anforderung ist 200 Elemente.</span><span class="sxs-lookup"><span data-stu-id="41d83-164">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="41d83-165">Beispiel</span><span class="sxs-lookup"><span data-stu-id="41d83-165">Example</span></span>

### <a name="csv"></a><span data-ttu-id="41d83-166">CSV</span><span class="sxs-lookup"><span data-stu-id="41d83-166">CSV</span></span>

<span data-ttu-id="41d83-167">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="41d83-167">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="41d83-168">Anforderung</span><span class="sxs-lookup"><span data-stu-id="41d83-168">Request</span></span>

<span data-ttu-id="41d83-169">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="41d83-169">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusageuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="41d83-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="41d83-170">Response</span></span>

<span data-ttu-id="41d83-171">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="41d83-171">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="41d83-172">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="41d83-172">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,User State,State Change Date,Last Activity Date,Used Web,Used Windows Phone,Used Android Phone,Used iPhone,Used iPad,Used Others,Report Period
```

### <a name="json"></a><span data-ttu-id="41d83-173">JSON</span><span class="sxs-lookup"><span data-stu-id="41d83-173">JSON</span></span>

<span data-ttu-id="41d83-174">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="41d83-174">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="41d83-175">Anforderung</span><span class="sxs-lookup"><span data-stu-id="41d83-175">Request</span></span>

<span data-ttu-id="41d83-176">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="41d83-176">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusageuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="41d83-177">Antwort</span><span class="sxs-lookup"><span data-stu-id="41d83-177">Response</span></span>

<span data-ttu-id="41d83-178">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="41d83-178">The following is an example of the response.</span></span>

> <span data-ttu-id="41d83-p107">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="41d83-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerDeviceUsageUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 442

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerDeviceUsageUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-06", 
      "userPrincipalName": "userPrincipalName-value", 
      "displayName": "displayName-value", 
      "userState": "active", 
      "stateChangeDate": "2012-06-26", 
      "lastActivityDate": "2017-09-06", 
      "usedWeb": true, 
      "usedWindowsPhone": false, 
      "usedAndroidPhone": false, 
      "usediPhone": false, 
      "usediPad": false, 
      "usedOthers": false, 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getyammerdeviceusageuserdetail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
