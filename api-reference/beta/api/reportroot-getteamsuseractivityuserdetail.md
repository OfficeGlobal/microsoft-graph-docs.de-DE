---
title: 'reportRoot: getTeamsUserActivityUserDetail'
description: Abrufen von Details zur Microsoft Teams-Benutzeraktivität nach Benutzer.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: eb884bce47943da0f3f0a3047a65295353fa3252
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521537"
---
# <a name="reportroot-getteamsuseractivityuserdetail"></a><span data-ttu-id="0012e-103">reportRoot: getTeamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="0012e-103">reportRoot: getTeamsUserActivityUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0012e-104">Abrufen von Details zur Microsoft Teams-Benutzeraktivität nach Benutzer.</span><span class="sxs-lookup"><span data-stu-id="0012e-104">Get details about Microsoft Teams user activity by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="0012e-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0012e-105">Permissions</span></span>

<span data-ttu-id="0012e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0012e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0012e-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0012e-108">Permission type</span></span>                        | <span data-ttu-id="0012e-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0012e-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="0012e-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0012e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="0012e-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0012e-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="0012e-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0012e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0012e-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0012e-113">Not supported.</span></span>                           |
| <span data-ttu-id="0012e-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0012e-114">Application</span></span>                            | <span data-ttu-id="0012e-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0012e-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="0012e-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0012e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserDetail(period='D7')
GET /reports/getTeamsUserActivityUserDetail(date=2017-09-01)
```

## <a name="function-parameters"></a><span data-ttu-id="0012e-117">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="0012e-117">Function parameters</span></span>

<span data-ttu-id="0012e-118">Geben Sie in der Anforderungs-URL einen der folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="0012e-118">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="0012e-119">Parameter</span><span class="sxs-lookup"><span data-stu-id="0012e-119">Parameter</span></span> | <span data-ttu-id="0012e-120">Typ</span><span class="sxs-lookup"><span data-stu-id="0012e-120">Type</span></span>   | <span data-ttu-id="0012e-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0012e-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="0012e-122">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="0012e-122">period</span></span>    | <span data-ttu-id="0012e-123">string</span><span class="sxs-lookup"><span data-stu-id="0012e-123">string</span></span> | <span data-ttu-id="0012e-124">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="0012e-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="0012e-125">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="0012e-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="0012e-126">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="0012e-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="0012e-127">date</span><span class="sxs-lookup"><span data-stu-id="0012e-127">date</span></span>      | <span data-ttu-id="0012e-128">Datum</span><span class="sxs-lookup"><span data-stu-id="0012e-128">Date</span></span>   | <span data-ttu-id="0012e-129">Gibt das Datum an, für das die Benutzer angezeigt werden sollen, die Aktivitäten durchgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="0012e-129">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="0012e-130">{date_value} muss im Format JJJJ-MM-TT vorliegen.</span><span class="sxs-lookup"><span data-stu-id="0012e-130">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="0012e-131">Da dieser Bericht nur für die letzten 30 Tage verfügbar ist, sollte {date_value} ein Datum aus diesem Zeitraum sein.</span><span class="sxs-lookup"><span data-stu-id="0012e-131">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="0012e-132">**Hinweis:** Sie müssen in der URL entweder einen Zeitraum oder ein Datum festlegen.</span><span class="sxs-lookup"><span data-stu-id="0012e-132">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="0012e-133">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) von  `$format`, `$top` und `$skipToken` zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0012e-133">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="0012e-134">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="0012e-134">The default output type is text/csv.</span></span> <span data-ttu-id="0012e-135">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="0012e-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0012e-136">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0012e-136">Request headers</span></span>

| <span data-ttu-id="0012e-137">Name</span><span class="sxs-lookup"><span data-stu-id="0012e-137">Name</span></span>          | <span data-ttu-id="0012e-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0012e-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="0012e-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="0012e-139">Authorization</span></span> | <span data-ttu-id="0012e-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0012e-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="0012e-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="0012e-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="0012e-143">CSV</span><span class="sxs-lookup"><span data-stu-id="0012e-143">CSV</span></span>

<span data-ttu-id="0012e-144">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="0012e-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="0012e-145">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0012e-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="0012e-146">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="0012e-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="0012e-147">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="0012e-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="0012e-148">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="0012e-148">Report Refresh Date</span></span>
- <span data-ttu-id="0012e-149">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="0012e-149">User Principal Name</span></span>
- <span data-ttu-id="0012e-150">Datum der letzten Aktivität</span><span class="sxs-lookup"><span data-stu-id="0012e-150">Last Activity Date</span></span>
- <span data-ttu-id="0012e-151">Ist gelöscht</span><span class="sxs-lookup"><span data-stu-id="0012e-151">Is Deleted</span></span>
- <span data-ttu-id="0012e-152">Gelöscht am</span><span class="sxs-lookup"><span data-stu-id="0012e-152">Deleted Date</span></span>
- <span data-ttu-id="0012e-153">Zugewiesene Produkte</span><span class="sxs-lookup"><span data-stu-id="0012e-153">Assigned Products</span></span>
- <span data-ttu-id="0012e-154">Anzahl der Team-Chatnachrichten</span><span class="sxs-lookup"><span data-stu-id="0012e-154">Team Chat Message Count</span></span>
- <span data-ttu-id="0012e-155">Anzahl der privaten Chatnachrichten</span><span class="sxs-lookup"><span data-stu-id="0012e-155">Private Chat Message Count</span></span>
- <span data-ttu-id="0012e-156">Anzahl der Anrufe</span><span class="sxs-lookup"><span data-stu-id="0012e-156">Call Count</span></span>
- <span data-ttu-id="0012e-157">Anzahl der Besprechung</span><span class="sxs-lookup"><span data-stu-id="0012e-157">Meeting Count</span></span>
- <span data-ttu-id="0012e-158">Andere Aktion</span><span class="sxs-lookup"><span data-stu-id="0012e-158">Has Other Action</span></span>
- <span data-ttu-id="0012e-159">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="0012e-159">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="0012e-160">JSON</span><span class="sxs-lookup"><span data-stu-id="0012e-160">JSON</span></span>

<span data-ttu-id="0012e-161">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines **[TeamsUserActivityUserDetail](../resources/teamsuseractivityuserdetail.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="0012e-161">If successful, this method returns a `200 OK` response code and a **[teamsUserActivityUserDetail](../resources/teamsuseractivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="0012e-162">Die Seite Standardgröße für diese Anforderung ist 2000 Elemente.</span><span class="sxs-lookup"><span data-stu-id="0012e-162">The default page size for this request is 2000 items.</span></span>

## <a name="example"></a><span data-ttu-id="0012e-163">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0012e-163">Example</span></span>

### <a name="csv"></a><span data-ttu-id="0012e-164">CSV</span><span class="sxs-lookup"><span data-stu-id="0012e-164">CSV</span></span>

<span data-ttu-id="0012e-165">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="0012e-165">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="0012e-166">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0012e-166">Request</span></span>

<span data-ttu-id="0012e-167">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0012e-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="0012e-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="0012e-168">Response</span></span>

<span data-ttu-id="0012e-169">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0012e-169">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="0012e-170">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="0012e-170">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Is Deleted,Deleted Date,Assigned Products,Team Chat Message Count,Private Chat Message Count,Call Count,Meeting Count,Has Other Action,Report Period
```

### <a name="json"></a><span data-ttu-id="0012e-171">JSON</span><span class="sxs-lookup"><span data-stu-id="0012e-171">JSON</span></span>

<span data-ttu-id="0012e-172">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0012e-172">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="0012e-173">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0012e-173">Request</span></span>

<span data-ttu-id="0012e-174">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0012e-174">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="0012e-175">Antwort</span><span class="sxs-lookup"><span data-stu-id="0012e-175">Response</span></span>

<span data-ttu-id="0012e-176">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0012e-176">The following is an example of the response.</span></span>

> <span data-ttu-id="0012e-p107">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="0012e-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsUserActivityUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 452

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsUserActivityUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "lastActivityDate": "2017-09-01", 
      "isDeleted": false, 
      "deletedDate": null, 
      "assignedProducts": [
        "OFFICE 365 ENTERPRISE E5"
      ], 
      "teamChatMessageCount": 0, 
      "privateChatMessageCount": 49, 
      "callCount": 2, 
      "meetingCount": 0, 
      "hasOtherAction": true, 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getteamsuseractivityuserdetail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
