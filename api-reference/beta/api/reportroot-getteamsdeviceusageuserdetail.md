---
title: 'reportRoot: getTeamsDeviceUsageUserDetail'
description: Diese Methode ruft Details zur Microsoft Teams-Gerätenutzung ab, aufgeschlüsselt nach Benutzer.
localization_priority: Normal
ms.openlocfilehash: ade8bbcd2ce680bb7103bd0e9dbb09f3d49d1b03
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842210"
---
# <a name="reportroot-getteamsdeviceusageuserdetail"></a><span data-ttu-id="5b81e-103">reportRoot: getTeamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="5b81e-103">reportRoot: getTeamsDeviceUsageUserDetail</span></span>

> <span data-ttu-id="5b81e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5b81e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5b81e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5b81e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5b81e-106">Diese Methode ruft Details zur Microsoft Teams-Gerätenutzung ab, aufgeschlüsselt nach Benutzer.</span><span class="sxs-lookup"><span data-stu-id="5b81e-106">Get details about Microsoft Teams device usage by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="5b81e-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5b81e-107">Permissions</span></span>

<span data-ttu-id="5b81e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b81e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5b81e-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5b81e-110">Permission type</span></span>                        | <span data-ttu-id="5b81e-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5b81e-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="5b81e-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5b81e-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="5b81e-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b81e-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="5b81e-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5b81e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b81e-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5b81e-115">Not supported.</span></span>                           |
| <span data-ttu-id="5b81e-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5b81e-116">Application</span></span>                            | <span data-ttu-id="5b81e-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b81e-117">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="5b81e-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5b81e-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageUserDetail(period='D7')
GET /reports/getTeamsDeviceUsageUserDetail(date=2017-09-01)
```

## <a name="function-parameters"></a><span data-ttu-id="5b81e-119">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="5b81e-119">Function parameters</span></span>

<span data-ttu-id="5b81e-120">Geben Sie in der Anforderungs-URL einen der folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="5b81e-120">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="5b81e-121">Parameter</span><span class="sxs-lookup"><span data-stu-id="5b81e-121">Parameter</span></span> | <span data-ttu-id="5b81e-122">Typ</span><span class="sxs-lookup"><span data-stu-id="5b81e-122">Type</span></span>   | <span data-ttu-id="5b81e-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5b81e-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="5b81e-124">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="5b81e-124">period</span></span>    | <span data-ttu-id="5b81e-125">string</span><span class="sxs-lookup"><span data-stu-id="5b81e-125">string</span></span> | <span data-ttu-id="5b81e-126">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="5b81e-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="5b81e-127">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="5b81e-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="5b81e-128">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="5b81e-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="5b81e-129">date</span><span class="sxs-lookup"><span data-stu-id="5b81e-129">date</span></span>      | <span data-ttu-id="5b81e-130">Datum</span><span class="sxs-lookup"><span data-stu-id="5b81e-130">Date</span></span>   | <span data-ttu-id="5b81e-131">Gibt das Datum an, für das die Benutzer angezeigt werden sollen, die Aktivitäten durchgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="5b81e-131">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="5b81e-132">{date_value} muss im Format JJJJ-MM-TT vorliegen.</span><span class="sxs-lookup"><span data-stu-id="5b81e-132">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="5b81e-133">Da dieser Bericht nur für die letzten 30 Tage verfügbar ist, sollte {date_value} ein Datum aus diesem Zeitraum sein.</span><span class="sxs-lookup"><span data-stu-id="5b81e-133">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="5b81e-134">**Hinweis:** Sie müssen in der URL entweder einen Zeitraum oder ein Datum festlegen.</span><span class="sxs-lookup"><span data-stu-id="5b81e-134">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="5b81e-135">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) von  `$format`, `$top` und `$skipToken` zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5b81e-135">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="5b81e-136">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="5b81e-136">The default output type is text/csv.</span></span> <span data-ttu-id="5b81e-137">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="5b81e-137">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5b81e-138">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5b81e-138">Request headers</span></span>

| <span data-ttu-id="5b81e-139">Name</span><span class="sxs-lookup"><span data-stu-id="5b81e-139">Name</span></span>          | <span data-ttu-id="5b81e-140">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5b81e-140">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="5b81e-141">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b81e-141">Authorization</span></span> | <span data-ttu-id="5b81e-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5b81e-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="5b81e-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="5b81e-144">Response</span></span>

### <a name="csv"></a><span data-ttu-id="5b81e-145">CSV</span><span class="sxs-lookup"><span data-stu-id="5b81e-145">CSV</span></span>

<span data-ttu-id="5b81e-146">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="5b81e-146">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="5b81e-147">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5b81e-147">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="5b81e-148">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="5b81e-148">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="5b81e-149">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="5b81e-149">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="5b81e-150">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="5b81e-150">Report Refresh Date</span></span>
- <span data-ttu-id="5b81e-151">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="5b81e-151">User Principal Name</span></span>
- <span data-ttu-id="5b81e-152">Datum der letzten Aktivität</span><span class="sxs-lookup"><span data-stu-id="5b81e-152">Last Activity Date</span></span>
- <span data-ttu-id="5b81e-153">Ist gelöscht</span><span class="sxs-lookup"><span data-stu-id="5b81e-153">Is Deleted</span></span>
- <span data-ttu-id="5b81e-154">Deleted Date</span><span class="sxs-lookup"><span data-stu-id="5b81e-154">Deleted Date</span></span>
- <span data-ttu-id="5b81e-155">Used Web</span><span class="sxs-lookup"><span data-stu-id="5b81e-155">Used Web</span></span>
- <span data-ttu-id="5b81e-156">Used Windows Phone</span><span class="sxs-lookup"><span data-stu-id="5b81e-156">Used Windows Phone</span></span>
- <span data-ttu-id="5b81e-157">Used iOS</span><span class="sxs-lookup"><span data-stu-id="5b81e-157">Used iOS</span></span>
- <span data-ttu-id="5b81e-158">Used Mac</span><span class="sxs-lookup"><span data-stu-id="5b81e-158">Used Mac</span></span>
- <span data-ttu-id="5b81e-159">Used Android Phone</span><span class="sxs-lookup"><span data-stu-id="5b81e-159">Used Android Phone</span></span>
- <span data-ttu-id="5b81e-160">Used Windows</span><span class="sxs-lookup"><span data-stu-id="5b81e-160">Used Windows</span></span>
- <span data-ttu-id="5b81e-161">Report Period</span><span class="sxs-lookup"><span data-stu-id="5b81e-161">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="5b81e-162">JSON</span><span class="sxs-lookup"><span data-stu-id="5b81e-162">JSON</span></span>

<span data-ttu-id="5b81e-163">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines **[TeamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="5b81e-163">If successful, this method returns a `200 OK` response code and a **[teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="5b81e-164">Die Seite Standardgröße für diese Anforderung ist 2000 Elemente.</span><span class="sxs-lookup"><span data-stu-id="5b81e-164">The default page size for this request is 2000 items.</span></span>

## <a name="example"></a><span data-ttu-id="5b81e-165">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5b81e-165">Example</span></span>

### <a name="csv"></a><span data-ttu-id="5b81e-166">CSV</span><span class="sxs-lookup"><span data-stu-id="5b81e-166">CSV</span></span>

<span data-ttu-id="5b81e-167">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="5b81e-167">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="5b81e-168">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5b81e-168">Request</span></span>

<span data-ttu-id="5b81e-169">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5b81e-169">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="5b81e-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="5b81e-170">Response</span></span>

<span data-ttu-id="5b81e-171">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5b81e-171">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="5b81e-172">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="5b81e-172">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="5b81e-173">JSON</span><span class="sxs-lookup"><span data-stu-id="5b81e-173">JSON</span></span>

<span data-ttu-id="5b81e-174">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5b81e-174">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="5b81e-175">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5b81e-175">Request</span></span>

<span data-ttu-id="5b81e-176">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5b81e-176">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="5b81e-177">Antwort</span><span class="sxs-lookup"><span data-stu-id="5b81e-177">Response</span></span>

<span data-ttu-id="5b81e-178">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5b81e-178">The following is an example of the response.</span></span>

> <span data-ttu-id="5b81e-p108">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="5b81e-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
