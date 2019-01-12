---
title: 'reportRoot: getTeamsUserActivityUserDetail'
description: Abrufen von Details zur Microsoft Teams-Benutzeraktivität nach Benutzer.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 558e142eb9b8afd74ba30657e5b21726f283df2b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962961"
---
# <a name="reportroot-getteamsuseractivityuserdetail"></a><span data-ttu-id="d5595-103">reportRoot: getTeamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="d5595-103">reportRoot: getTeamsUserActivityUserDetail</span></span>

> <span data-ttu-id="d5595-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d5595-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d5595-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d5595-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d5595-106">Abrufen von Details zur Microsoft Teams-Benutzeraktivität nach Benutzer.</span><span class="sxs-lookup"><span data-stu-id="d5595-106">Get details about Microsoft Teams user activity by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="d5595-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d5595-107">Permissions</span></span>

<span data-ttu-id="d5595-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5595-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d5595-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d5595-110">Permission type</span></span>                        | <span data-ttu-id="d5595-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d5595-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="d5595-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d5595-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="d5595-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5595-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="d5595-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d5595-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5595-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d5595-115">Not supported.</span></span>                           |
| <span data-ttu-id="d5595-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d5595-116">Application</span></span>                            | <span data-ttu-id="d5595-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5595-117">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="d5595-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d5595-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserDetail(period='D7')
GET /reports/getTeamsUserActivityUserDetail(date=2017-09-01)
```

## <a name="function-parameters"></a><span data-ttu-id="d5595-119">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="d5595-119">Function parameters</span></span>

<span data-ttu-id="d5595-120">Geben Sie in der Anforderungs-URL einen der folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="d5595-120">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="d5595-121">Parameter</span><span class="sxs-lookup"><span data-stu-id="d5595-121">Parameter</span></span> | <span data-ttu-id="d5595-122">Typ</span><span class="sxs-lookup"><span data-stu-id="d5595-122">Type</span></span>   | <span data-ttu-id="d5595-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d5595-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="d5595-124">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="d5595-124">period</span></span>    | <span data-ttu-id="d5595-125">string</span><span class="sxs-lookup"><span data-stu-id="d5595-125">string</span></span> | <span data-ttu-id="d5595-126">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="d5595-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="d5595-127">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="d5595-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="d5595-128">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="d5595-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="d5595-129">date</span><span class="sxs-lookup"><span data-stu-id="d5595-129">date</span></span>      | <span data-ttu-id="d5595-130">Datum</span><span class="sxs-lookup"><span data-stu-id="d5595-130">Date</span></span>   | <span data-ttu-id="d5595-131">Gibt das Datum an, für das die Benutzer angezeigt werden sollen, die Aktivitäten durchgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="d5595-131">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="d5595-132">{date_value} muss im Format JJJJ-MM-TT vorliegen.</span><span class="sxs-lookup"><span data-stu-id="d5595-132">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="d5595-133">Da dieser Bericht nur für die letzten 30 Tage verfügbar ist, sollte {date_value} ein Datum aus diesem Zeitraum sein.</span><span class="sxs-lookup"><span data-stu-id="d5595-133">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="d5595-134">**Hinweis:** Sie müssen in der URL entweder einen Zeitraum oder ein Datum festlegen.</span><span class="sxs-lookup"><span data-stu-id="d5595-134">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="d5595-135">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) von  `$format`, `$top` und `$skipToken` zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d5595-135">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="d5595-136">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="d5595-136">The default output type is text/csv.</span></span> <span data-ttu-id="d5595-137">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="d5595-137">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d5595-138">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d5595-138">Request headers</span></span>

| <span data-ttu-id="d5595-139">Name</span><span class="sxs-lookup"><span data-stu-id="d5595-139">Name</span></span>          | <span data-ttu-id="d5595-140">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d5595-140">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="d5595-141">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5595-141">Authorization</span></span> | <span data-ttu-id="d5595-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d5595-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="d5595-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="d5595-144">Response</span></span>

### <a name="csv"></a><span data-ttu-id="d5595-145">CSV</span><span class="sxs-lookup"><span data-stu-id="d5595-145">CSV</span></span>

<span data-ttu-id="d5595-146">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="d5595-146">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="d5595-147">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d5595-147">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="d5595-148">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="d5595-148">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="d5595-149">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="d5595-149">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="d5595-150">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="d5595-150">Report Refresh Date</span></span>
- <span data-ttu-id="d5595-151">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="d5595-151">User Principal Name</span></span>
- <span data-ttu-id="d5595-152">Datum der letzten Aktivität</span><span class="sxs-lookup"><span data-stu-id="d5595-152">Last Activity Date</span></span>
- <span data-ttu-id="d5595-153">Ist gelöscht</span><span class="sxs-lookup"><span data-stu-id="d5595-153">Is Deleted</span></span>
- <span data-ttu-id="d5595-154">Gelöscht am</span><span class="sxs-lookup"><span data-stu-id="d5595-154">Deleted Date</span></span>
- <span data-ttu-id="d5595-155">Zugewiesene Produkte</span><span class="sxs-lookup"><span data-stu-id="d5595-155">Assigned Products</span></span>
- <span data-ttu-id="d5595-156">Anzahl der Team-Chatnachrichten</span><span class="sxs-lookup"><span data-stu-id="d5595-156">Team Chat Message Count</span></span>
- <span data-ttu-id="d5595-157">Anzahl der privaten Chatnachrichten</span><span class="sxs-lookup"><span data-stu-id="d5595-157">Private Chat Message Count</span></span>
- <span data-ttu-id="d5595-158">Anzahl der Anrufe</span><span class="sxs-lookup"><span data-stu-id="d5595-158">Call Count</span></span>
- <span data-ttu-id="d5595-159">Anzahl der Besprechung</span><span class="sxs-lookup"><span data-stu-id="d5595-159">Meeting Count</span></span>
- <span data-ttu-id="d5595-160">Andere Aktion</span><span class="sxs-lookup"><span data-stu-id="d5595-160">Has Other Action</span></span>
- <span data-ttu-id="d5595-161">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="d5595-161">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="d5595-162">JSON</span><span class="sxs-lookup"><span data-stu-id="d5595-162">JSON</span></span>

<span data-ttu-id="d5595-163">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines **[TeamsUserActivityUserDetail](../resources/teamsuseractivityuserdetail.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="d5595-163">If successful, this method returns a `200 OK` response code and a **[teamsUserActivityUserDetail](../resources/teamsuseractivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="d5595-164">Die Seite Standardgröße für diese Anforderung ist 2000 Elemente.</span><span class="sxs-lookup"><span data-stu-id="d5595-164">The default page size for this request is 2000 items.</span></span>

## <a name="example"></a><span data-ttu-id="d5595-165">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d5595-165">Example</span></span>

### <a name="csv"></a><span data-ttu-id="d5595-166">CSV</span><span class="sxs-lookup"><span data-stu-id="d5595-166">CSV</span></span>

<span data-ttu-id="d5595-167">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="d5595-167">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="d5595-168">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d5595-168">Request</span></span>

<span data-ttu-id="d5595-169">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d5595-169">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="d5595-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="d5595-170">Response</span></span>

<span data-ttu-id="d5595-171">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d5595-171">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="d5595-172">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="d5595-172">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="d5595-173">JSON</span><span class="sxs-lookup"><span data-stu-id="d5595-173">JSON</span></span>

<span data-ttu-id="d5595-174">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d5595-174">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="d5595-175">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d5595-175">Request</span></span>

<span data-ttu-id="d5595-176">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d5595-176">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="d5595-177">Antwort</span><span class="sxs-lookup"><span data-stu-id="d5595-177">Response</span></span>

<span data-ttu-id="d5595-178">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d5595-178">The following is an example of the response.</span></span>

> <span data-ttu-id="d5595-p108">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="d5595-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
