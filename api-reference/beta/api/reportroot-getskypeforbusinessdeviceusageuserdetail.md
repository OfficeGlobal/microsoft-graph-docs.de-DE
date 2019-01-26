---
title: 'reportRoot: getSkypeForBusinessDeviceUsageUserDetail'
description: Rufen Sie Details der Skype for Business-Gerätenutzung nach Benutzer ab.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 32b3a3e2ebf0d05440cb38a1bc0ef7fdda983258
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576094"
---
# <a name="reportroot-getskypeforbusinessdeviceusageuserdetail"></a><span data-ttu-id="254cc-103">reportRoot: getSkypeForBusinessDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="254cc-103">reportRoot: getSkypeForBusinessDeviceUsageUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="254cc-104">Rufen Sie Details der Skype for Business-Gerätenutzung nach Benutzer ab.</span><span class="sxs-lookup"><span data-stu-id="254cc-104">Get details about Skype for Business device usage by user.</span></span>

> <span data-ttu-id="254cc-105">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Verwendete Skype for Business-Clients](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span><span class="sxs-lookup"><span data-stu-id="254cc-105">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="254cc-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="254cc-106">Permissions</span></span>

<span data-ttu-id="254cc-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="254cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="254cc-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="254cc-109">Permission type</span></span>                        | <span data-ttu-id="254cc-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="254cc-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="254cc-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="254cc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="254cc-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="254cc-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="254cc-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="254cc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="254cc-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="254cc-114">Not supported.</span></span>                           |
| <span data-ttu-id="254cc-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="254cc-115">Application</span></span>                            | <span data-ttu-id="254cc-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="254cc-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="254cc-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="254cc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="254cc-118">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="254cc-118">Function parameters</span></span>

<span data-ttu-id="254cc-119">Geben Sie in der Anforderungs-URL einen der folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="254cc-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="254cc-120">Parameter</span><span class="sxs-lookup"><span data-stu-id="254cc-120">Parameter</span></span> | <span data-ttu-id="254cc-121">Typ</span><span class="sxs-lookup"><span data-stu-id="254cc-121">Type</span></span>   | <span data-ttu-id="254cc-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="254cc-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="254cc-123">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="254cc-123">period</span></span>    | <span data-ttu-id="254cc-124">string</span><span class="sxs-lookup"><span data-stu-id="254cc-124">string</span></span> | <span data-ttu-id="254cc-125">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="254cc-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="254cc-126">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="254cc-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="254cc-127">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="254cc-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="254cc-128">date</span><span class="sxs-lookup"><span data-stu-id="254cc-128">date</span></span>      | <span data-ttu-id="254cc-129">Datum</span><span class="sxs-lookup"><span data-stu-id="254cc-129">Date</span></span>   | <span data-ttu-id="254cc-130">Gibt das Datum an, für das die Benutzer angezeigt werden sollen, die Aktivitäten durchgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="254cc-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="254cc-131">{date_value} muss im Format JJJJ-MM-TT vorliegen.</span><span class="sxs-lookup"><span data-stu-id="254cc-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="254cc-132">Da dieser Bericht nur für die letzten 30 Tage verfügbar ist, sollte {date_value} ein Datum aus diesem Zeitraum sein.</span><span class="sxs-lookup"><span data-stu-id="254cc-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="254cc-133">**Hinweis:** Sie müssen in der URL entweder einen Zeitraum oder ein Datum festlegen.</span><span class="sxs-lookup"><span data-stu-id="254cc-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="254cc-134">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) von  `$format`, `$top` und `$skipToken` zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="254cc-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="254cc-135">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="254cc-135">The default output type is text/csv.</span></span> <span data-ttu-id="254cc-136">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="254cc-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="254cc-137">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="254cc-137">Request headers</span></span>

| <span data-ttu-id="254cc-138">Name</span><span class="sxs-lookup"><span data-stu-id="254cc-138">Name</span></span>          | <span data-ttu-id="254cc-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="254cc-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="254cc-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="254cc-140">Authorization</span></span> | <span data-ttu-id="254cc-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="254cc-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="254cc-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="254cc-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="254cc-144">CSV</span><span class="sxs-lookup"><span data-stu-id="254cc-144">CSV</span></span>

<span data-ttu-id="254cc-145">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="254cc-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="254cc-146">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="254cc-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="254cc-147">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="254cc-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="254cc-148">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="254cc-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="254cc-149">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="254cc-149">Report Refresh Date</span></span>
- <span data-ttu-id="254cc-150">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="254cc-150">User Principal Name</span></span>
- <span data-ttu-id="254cc-151">Datum der letzten Aktivität</span><span class="sxs-lookup"><span data-stu-id="254cc-151">Last Activity Date</span></span>
- <span data-ttu-id="254cc-152">Verwendetes Windows</span><span class="sxs-lookup"><span data-stu-id="254cc-152">Used Windows</span></span>
- <span data-ttu-id="254cc-153">Verwendetes Windows Phone</span><span class="sxs-lookup"><span data-stu-id="254cc-153">Used Windows Phone</span></span>
- <span data-ttu-id="254cc-154">Verwendetes Android Phone</span><span class="sxs-lookup"><span data-stu-id="254cc-154">Used Android Phone</span></span>
- <span data-ttu-id="254cc-155">Verwendetes iPhone</span><span class="sxs-lookup"><span data-stu-id="254cc-155">Used iPhone</span></span>
- <span data-ttu-id="254cc-156">Verwendetes iPad</span><span class="sxs-lookup"><span data-stu-id="254cc-156">Used iPad</span></span>
- <span data-ttu-id="254cc-157">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="254cc-157">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="254cc-158">JSON</span><span class="sxs-lookup"><span data-stu-id="254cc-158">JSON</span></span>

<span data-ttu-id="254cc-159">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines **[SkypeForBusinessDeviceUsageUserDetail](../resources/skypeforbusinessdeviceusageuserdetail.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="254cc-159">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessDeviceUsageUserDetail](../resources/skypeforbusinessdeviceusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="254cc-160">Die Seite Standardgröße für diese Anforderung ist 200 Elemente.</span><span class="sxs-lookup"><span data-stu-id="254cc-160">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="254cc-161">Beispiel</span><span class="sxs-lookup"><span data-stu-id="254cc-161">Example</span></span>

### <a name="csv"></a><span data-ttu-id="254cc-162">CSV</span><span class="sxs-lookup"><span data-stu-id="254cc-162">CSV</span></span>

<span data-ttu-id="254cc-163">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="254cc-163">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="254cc-164">Anforderung</span><span class="sxs-lookup"><span data-stu-id="254cc-164">Request</span></span>

<span data-ttu-id="254cc-165">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="254cc-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusageuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="254cc-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="254cc-166">Response</span></span>

<span data-ttu-id="254cc-167">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="254cc-167">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="254cc-168">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="254cc-168">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Used Windows,Used Windows Phone,Used Android Phone,Used iPhone,Used iPad,Report Period
```

### <a name="json"></a><span data-ttu-id="254cc-169">JSON</span><span class="sxs-lookup"><span data-stu-id="254cc-169">JSON</span></span>

<span data-ttu-id="254cc-170">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="254cc-170">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="254cc-171">Anforderung</span><span class="sxs-lookup"><span data-stu-id="254cc-171">Request</span></span>

<span data-ttu-id="254cc-172">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="254cc-172">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusageuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="254cc-173">Antwort</span><span class="sxs-lookup"><span data-stu-id="254cc-173">Response</span></span>

<span data-ttu-id="254cc-174">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="254cc-174">The following is an example of the response.</span></span>

> <span data-ttu-id="254cc-p107">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="254cc-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 356

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessDeviceUsageUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "lastActivityDate": "2017-09-01", 
      "usedWindows": true, 
      "usedWindowsPhone": false, 
      "usedAndroidPhone": false, 
      "usediPhone": false, 
      "usediPad": false, 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessdeviceusageuserdetail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
