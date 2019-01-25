---
title: 'reportRoot: getYammerGroupsActivityDetail'
description: Rufen Sie Details zur Yammer-Gruppenaktivität nach Gruppe ab.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 26df83b7e453c1e51edfccb2c8fd31df37917933
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512843"
---
# <a name="reportroot-getyammergroupsactivitydetail"></a><span data-ttu-id="e0e94-103">reportRoot: getYammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="e0e94-103">reportRoot: getYammerGroupsActivityDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0e94-104">Rufen Sie Details zur Yammer-Gruppenaktivität nach Gruppe ab.</span><span class="sxs-lookup"><span data-stu-id="e0e94-104">Get details about Yammer groups activity by group.</span></span>

> <span data-ttu-id="e0e94-105">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Yammer-Gruppenaktivität](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span><span class="sxs-lookup"><span data-stu-id="e0e94-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="permissions"></a><span data-ttu-id="e0e94-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e0e94-106">Permissions</span></span>

<span data-ttu-id="e0e94-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0e94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e0e94-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e0e94-109">Permission type</span></span>                        | <span data-ttu-id="e0e94-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e0e94-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="e0e94-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e0e94-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e0e94-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e0e94-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="e0e94-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e0e94-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0e94-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e0e94-114">Not supported.</span></span>                           |
| <span data-ttu-id="e0e94-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e0e94-115">Application</span></span>                            | <span data-ttu-id="e0e94-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e0e94-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="e0e94-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e0e94-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerGroupsActivityDetail(period='{period_value}')
GET /reports/getYammerGroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="e0e94-118">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="e0e94-118">Function parameters</span></span>

<span data-ttu-id="e0e94-119">Geben Sie in der Anforderungs-URL einen der folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="e0e94-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="e0e94-120">Parameter</span><span class="sxs-lookup"><span data-stu-id="e0e94-120">Parameter</span></span> | <span data-ttu-id="e0e94-121">Typ</span><span class="sxs-lookup"><span data-stu-id="e0e94-121">Type</span></span>   | <span data-ttu-id="e0e94-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e0e94-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="e0e94-123">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="e0e94-123">period</span></span>    | <span data-ttu-id="e0e94-124">string</span><span class="sxs-lookup"><span data-stu-id="e0e94-124">string</span></span> | <span data-ttu-id="e0e94-125">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="e0e94-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="e0e94-126">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="e0e94-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="e0e94-127">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="e0e94-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="e0e94-128">date</span><span class="sxs-lookup"><span data-stu-id="e0e94-128">date</span></span>      | <span data-ttu-id="e0e94-129">Datum</span><span class="sxs-lookup"><span data-stu-id="e0e94-129">Date</span></span>   | <span data-ttu-id="e0e94-130">Gibt das Datum an, für das die Benutzer angezeigt werden sollen, die Aktivitäten durchgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="e0e94-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="e0e94-131">{date_value} muss im Format JJJJ-MM-TT vorliegen.</span><span class="sxs-lookup"><span data-stu-id="e0e94-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="e0e94-132">Da dieser Bericht nur für die letzten 30 Tage verfügbar ist, sollte {date_value} ein Datum aus diesem Zeitraum sein.</span><span class="sxs-lookup"><span data-stu-id="e0e94-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="e0e94-133">**Hinweis:** Sie müssen in der URL entweder einen Zeitraum oder ein Datum festlegen.</span><span class="sxs-lookup"><span data-stu-id="e0e94-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="e0e94-134">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) von  `$format`, `$top` und `$skipToken` zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e0e94-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="e0e94-135">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="e0e94-135">The default output type is text/csv.</span></span> <span data-ttu-id="e0e94-136">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="e0e94-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e0e94-137">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e0e94-137">Request headers</span></span>

| <span data-ttu-id="e0e94-138">Name</span><span class="sxs-lookup"><span data-stu-id="e0e94-138">Name</span></span>          | <span data-ttu-id="e0e94-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e0e94-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="e0e94-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0e94-140">Authorization</span></span> | <span data-ttu-id="e0e94-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e0e94-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="e0e94-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="e0e94-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="e0e94-144">CSV</span><span class="sxs-lookup"><span data-stu-id="e0e94-144">CSV</span></span>

<span data-ttu-id="e0e94-145">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="e0e94-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="e0e94-146">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e0e94-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="e0e94-147">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="e0e94-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="e0e94-148">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="e0e94-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="e0e94-149">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="e0e94-149">Report Refresh Date</span></span>
- <span data-ttu-id="e0e94-150">Gruppenanzeigename</span><span class="sxs-lookup"><span data-stu-id="e0e94-150">Group Display Name</span></span>
- <span data-ttu-id="e0e94-151">Ist gelöscht</span><span class="sxs-lookup"><span data-stu-id="e0e94-151">Is Deleted</span></span>
- <span data-ttu-id="e0e94-152">Besitzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="e0e94-152">Owner Principal Name</span></span>
- <span data-ttu-id="e0e94-153">Datum der letzten Aktivität</span><span class="sxs-lookup"><span data-stu-id="e0e94-153">Last Activity Date</span></span>
- <span data-ttu-id="e0e94-154">Gruppentyp</span><span class="sxs-lookup"><span data-stu-id="e0e94-154">Group Type</span></span>
- <span data-ttu-id="e0e94-155">Mit Office 365 verbunden</span><span class="sxs-lookup"><span data-stu-id="e0e94-155">Office 365 Connected</span></span>
- <span data-ttu-id="e0e94-156">Mitgliederzahl</span><span class="sxs-lookup"><span data-stu-id="e0e94-156">Member Count</span></span>
- <span data-ttu-id="e0e94-157">Anzahl veröffentlicht</span><span class="sxs-lookup"><span data-stu-id="e0e94-157">Posted Count</span></span>
- <span data-ttu-id="e0e94-158">Anzahl gelesen</span><span class="sxs-lookup"><span data-stu-id="e0e94-158">Read Count</span></span>
- <span data-ttu-id="e0e94-159">Anzahl gelikt</span><span class="sxs-lookup"><span data-stu-id="e0e94-159">Liked Count</span></span>
- <span data-ttu-id="e0e94-160">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="e0e94-160">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="e0e94-161">JSON</span><span class="sxs-lookup"><span data-stu-id="e0e94-161">JSON</span></span>

<span data-ttu-id="e0e94-162">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines **[YammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="e0e94-162">If successful, this method returns a `200 OK` response code and a **[yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md)** object in the response body.</span></span>

<span data-ttu-id="e0e94-163">Die Seite Standardgröße für diese Anforderung ist 200 Elemente.</span><span class="sxs-lookup"><span data-stu-id="e0e94-163">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="e0e94-164">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e0e94-164">Example</span></span>

### <a name="csv"></a><span data-ttu-id="e0e94-165">CSV</span><span class="sxs-lookup"><span data-stu-id="e0e94-165">CSV</span></span>

<span data-ttu-id="e0e94-166">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="e0e94-166">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="e0e94-167">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e0e94-167">Request</span></span>

<span data-ttu-id="e0e94-168">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e0e94-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitydetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="e0e94-169">Antwort</span><span class="sxs-lookup"><span data-stu-id="e0e94-169">Response</span></span>

<span data-ttu-id="e0e94-170">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e0e94-170">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="e0e94-171">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="e0e94-171">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Group Display Name,Is Deleted,Owner Principal Name,Last Activity Date,Group Type,Office 365 Connected,Member Count,Posted Count,Read Count,Liked Count,Report Period
```

### <a name="json"></a><span data-ttu-id="e0e94-172">JSON</span><span class="sxs-lookup"><span data-stu-id="e0e94-172">JSON</span></span>

<span data-ttu-id="e0e94-173">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e0e94-173">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="e0e94-174">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e0e94-174">Request</span></span>

<span data-ttu-id="e0e94-175">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e0e94-175">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitydetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="e0e94-176">Antwort</span><span class="sxs-lookup"><span data-stu-id="e0e94-176">Response</span></span>

<span data-ttu-id="e0e94-177">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e0e94-177">The following is an example of the response.</span></span>

> <span data-ttu-id="e0e94-p107">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="e0e94-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerGroupsActivityDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 441

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerGroupsActivityDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "groupDisplayName": "groupDisplayName-value", 
      "isDeleted": false, 
      "ownerPrincipalName": "ownerPrincipalName-value", 
      "lastActivityDate": "2017-08-30", 
      "groupType": "private", 
      "office365Connected": true, 
      "memberCount": 176, 
      "postedCount": 15, 
      "readCount": 24, 
      "likedCount": 3, 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getyammergroupsactivitydetail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
