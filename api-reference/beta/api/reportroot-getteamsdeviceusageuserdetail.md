---
title: 'reportRoot: getTeamsDeviceUsageUserDetail'
description: Diese Methode ruft Details zur Microsoft Teams-Gerätenutzung ab, aufgeschlüsselt nach Benutzer.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 0e24a66905afa0ccb20c30fb4414e621cb4a1683
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522280"
---
# <a name="reportroot-getteamsdeviceusageuserdetail"></a><span data-ttu-id="2d980-103">reportRoot: getTeamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="2d980-103">reportRoot: getTeamsDeviceUsageUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d980-104">Diese Methode ruft Details zur Microsoft Teams-Gerätenutzung ab, aufgeschlüsselt nach Benutzer.</span><span class="sxs-lookup"><span data-stu-id="2d980-104">Get details about Microsoft Teams device usage by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="2d980-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2d980-105">Permissions</span></span>

<span data-ttu-id="2d980-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d980-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2d980-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2d980-108">Permission type</span></span>                        | <span data-ttu-id="2d980-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2d980-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="2d980-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2d980-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="2d980-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2d980-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="2d980-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2d980-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d980-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2d980-113">Not supported.</span></span>                           |
| <span data-ttu-id="2d980-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2d980-114">Application</span></span>                            | <span data-ttu-id="2d980-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2d980-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="2d980-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2d980-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageUserDetail(period='D7')
GET /reports/getTeamsDeviceUsageUserDetail(date=2017-09-01)
```

## <a name="function-parameters"></a><span data-ttu-id="2d980-117">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="2d980-117">Function parameters</span></span>

<span data-ttu-id="2d980-118">Geben Sie in der Anforderungs-URL einen der folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="2d980-118">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="2d980-119">Parameter</span><span class="sxs-lookup"><span data-stu-id="2d980-119">Parameter</span></span> | <span data-ttu-id="2d980-120">Typ</span><span class="sxs-lookup"><span data-stu-id="2d980-120">Type</span></span>   | <span data-ttu-id="2d980-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2d980-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="2d980-122">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="2d980-122">period</span></span>    | <span data-ttu-id="2d980-123">string</span><span class="sxs-lookup"><span data-stu-id="2d980-123">string</span></span> | <span data-ttu-id="2d980-124">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="2d980-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="2d980-125">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="2d980-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="2d980-126">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="2d980-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="2d980-127">date</span><span class="sxs-lookup"><span data-stu-id="2d980-127">date</span></span>      | <span data-ttu-id="2d980-128">Datum</span><span class="sxs-lookup"><span data-stu-id="2d980-128">Date</span></span>   | <span data-ttu-id="2d980-129">Gibt das Datum an, für das die Benutzer angezeigt werden sollen, die Aktivitäten durchgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="2d980-129">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="2d980-130">{date_value} muss im Format JJJJ-MM-TT vorliegen.</span><span class="sxs-lookup"><span data-stu-id="2d980-130">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="2d980-131">Da dieser Bericht nur für die letzten 30 Tage verfügbar ist, sollte {date_value} ein Datum aus diesem Zeitraum sein.</span><span class="sxs-lookup"><span data-stu-id="2d980-131">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="2d980-132">**Hinweis:** Sie müssen in der URL entweder einen Zeitraum oder ein Datum festlegen.</span><span class="sxs-lookup"><span data-stu-id="2d980-132">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="2d980-133">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) von  `$format`, `$top` und `$skipToken` zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2d980-133">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="2d980-134">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="2d980-134">The default output type is text/csv.</span></span> <span data-ttu-id="2d980-135">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="2d980-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2d980-136">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2d980-136">Request headers</span></span>

| <span data-ttu-id="2d980-137">Name</span><span class="sxs-lookup"><span data-stu-id="2d980-137">Name</span></span>          | <span data-ttu-id="2d980-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2d980-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="2d980-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d980-139">Authorization</span></span> | <span data-ttu-id="2d980-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2d980-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="2d980-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="2d980-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="2d980-143">CSV</span><span class="sxs-lookup"><span data-stu-id="2d980-143">CSV</span></span>

<span data-ttu-id="2d980-144">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="2d980-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="2d980-145">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2d980-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="2d980-146">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="2d980-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="2d980-147">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="2d980-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="2d980-148">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="2d980-148">Report Refresh Date</span></span>
- <span data-ttu-id="2d980-149">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="2d980-149">User Principal Name</span></span>
- <span data-ttu-id="2d980-150">Datum der letzten Aktivität</span><span class="sxs-lookup"><span data-stu-id="2d980-150">Last Activity Date</span></span>
- <span data-ttu-id="2d980-151">Ist gelöscht</span><span class="sxs-lookup"><span data-stu-id="2d980-151">Is Deleted</span></span>
- <span data-ttu-id="2d980-152">Deleted Date</span><span class="sxs-lookup"><span data-stu-id="2d980-152">Deleted Date</span></span>
- <span data-ttu-id="2d980-153">Used Web</span><span class="sxs-lookup"><span data-stu-id="2d980-153">Used Web</span></span>
- <span data-ttu-id="2d980-154">Used Windows Phone</span><span class="sxs-lookup"><span data-stu-id="2d980-154">Used Windows Phone</span></span>
- <span data-ttu-id="2d980-155">Used iOS</span><span class="sxs-lookup"><span data-stu-id="2d980-155">Used iOS</span></span>
- <span data-ttu-id="2d980-156">Used Mac</span><span class="sxs-lookup"><span data-stu-id="2d980-156">Used Mac</span></span>
- <span data-ttu-id="2d980-157">Used Android Phone</span><span class="sxs-lookup"><span data-stu-id="2d980-157">Used Android Phone</span></span>
- <span data-ttu-id="2d980-158">Used Windows</span><span class="sxs-lookup"><span data-stu-id="2d980-158">Used Windows</span></span>
- <span data-ttu-id="2d980-159">Report Period</span><span class="sxs-lookup"><span data-stu-id="2d980-159">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="2d980-160">JSON</span><span class="sxs-lookup"><span data-stu-id="2d980-160">JSON</span></span>

<span data-ttu-id="2d980-161">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines **[TeamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="2d980-161">If successful, this method returns a `200 OK` response code and a **[teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="2d980-162">Die Seite Standardgröße für diese Anforderung ist 2000 Elemente.</span><span class="sxs-lookup"><span data-stu-id="2d980-162">The default page size for this request is 2000 items.</span></span>

## <a name="example"></a><span data-ttu-id="2d980-163">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2d980-163">Example</span></span>

### <a name="csv"></a><span data-ttu-id="2d980-164">CSV</span><span class="sxs-lookup"><span data-stu-id="2d980-164">CSV</span></span>

<span data-ttu-id="2d980-165">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="2d980-165">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="2d980-166">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2d980-166">Request</span></span>

<span data-ttu-id="2d980-167">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2d980-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="2d980-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="2d980-168">Response</span></span>

<span data-ttu-id="2d980-169">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2d980-169">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="2d980-170">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="2d980-170">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Is Deleted,Deleted Date,Used Web,Used Windows Phone,Used iOS,Used Mac,Used Android Phone,Used Windows,Report Period
```

### <a name="json"></a><span data-ttu-id="2d980-171">JSON</span><span class="sxs-lookup"><span data-stu-id="2d980-171">JSON</span></span>

<span data-ttu-id="2d980-172">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2d980-172">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="2d980-173">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2d980-173">Request</span></span>

<span data-ttu-id="2d980-174">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2d980-174">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="2d980-175">Antwort</span><span class="sxs-lookup"><span data-stu-id="2d980-175">Response</span></span>

<span data-ttu-id="2d980-176">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2d980-176">The following is an example of the response.</span></span>

> <span data-ttu-id="2d980-p107">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="2d980-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 374

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsDeviceUsageUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "lastActivityDate": "2017-09-01", 
      "isDeleted": false, 
      "deletedDate": null, 
      "usedWeb": false, 
      "usedWindowsPhone": false, 
      "usediOS": true, 
      "usedMac": false, 
      "usedAndroidPhone": false, 
      "usedWindows": true, 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getteamsdeviceusageuserdetail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
