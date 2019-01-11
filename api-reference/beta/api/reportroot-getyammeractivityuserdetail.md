---
title: 'reportRoot: getYammerActivityUserDetail'
description: Rufen Sie Details zu Yammer-Aktivitäten nach Benutzer ab.
localization_priority: Normal
ms.openlocfilehash: da1337d6b925c7b729c950eeac35cc3a8981596e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839620"
---
# <a name="reportroot-getyammeractivityuserdetail"></a><span data-ttu-id="7ae67-103">reportRoot: getYammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="7ae67-103">reportRoot: getYammerActivityUserDetail</span></span>

> <span data-ttu-id="7ae67-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7ae67-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7ae67-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7ae67-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7ae67-106">Rufen Sie Details zu Yammer-Aktivitäten nach Benutzer ab.</span><span class="sxs-lookup"><span data-stu-id="7ae67-106">Get details about Yammer activity by user.</span></span>

> <span data-ttu-id="7ae67-107">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Yammer-Aktivität](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span><span class="sxs-lookup"><span data-stu-id="7ae67-107">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="permissions"></a><span data-ttu-id="7ae67-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7ae67-108">Permissions</span></span>

<span data-ttu-id="7ae67-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ae67-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7ae67-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7ae67-111">Permission type</span></span>                        | <span data-ttu-id="7ae67-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7ae67-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="7ae67-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7ae67-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="7ae67-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7ae67-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="7ae67-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7ae67-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ae67-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7ae67-116">Not supported.</span></span>                           |
| <span data-ttu-id="7ae67-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7ae67-117">Application</span></span>                            | <span data-ttu-id="7ae67-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7ae67-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="7ae67-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7ae67-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerActivityUserDetail(period='{period_value}')
GET /reports/getYammerActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="7ae67-120">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="7ae67-120">Function parameters</span></span>

<span data-ttu-id="7ae67-121">Geben Sie in der Anforderungs-URL einen der folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="7ae67-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="7ae67-122">Parameter</span><span class="sxs-lookup"><span data-stu-id="7ae67-122">Parameter</span></span> | <span data-ttu-id="7ae67-123">Typ</span><span class="sxs-lookup"><span data-stu-id="7ae67-123">Type</span></span>   | <span data-ttu-id="7ae67-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7ae67-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="7ae67-125">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="7ae67-125">period</span></span>    | <span data-ttu-id="7ae67-126">string</span><span class="sxs-lookup"><span data-stu-id="7ae67-126">string</span></span> | <span data-ttu-id="7ae67-127">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="7ae67-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="7ae67-128">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="7ae67-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="7ae67-129">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="7ae67-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="7ae67-130">date</span><span class="sxs-lookup"><span data-stu-id="7ae67-130">date</span></span>      | <span data-ttu-id="7ae67-131">Datum</span><span class="sxs-lookup"><span data-stu-id="7ae67-131">Date</span></span>   | <span data-ttu-id="7ae67-132">Gibt das Datum an, für das die Benutzer angezeigt werden sollen, die Aktivitäten durchgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="7ae67-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="7ae67-133">{date_value} muss im Format JJJJ-MM-TT vorliegen.</span><span class="sxs-lookup"><span data-stu-id="7ae67-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="7ae67-134">Da dieser Bericht nur für die letzten 30 Tage verfügbar ist, sollte {date_value} ein Datum aus diesem Zeitraum sein.</span><span class="sxs-lookup"><span data-stu-id="7ae67-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="7ae67-135">**Hinweis:** Sie müssen in der URL entweder einen Zeitraum oder ein Datum festlegen.</span><span class="sxs-lookup"><span data-stu-id="7ae67-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="7ae67-136">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) von  `$format`, `$top` und `$skipToken` zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7ae67-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="7ae67-137">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="7ae67-137">The default output type is text/csv.</span></span> <span data-ttu-id="7ae67-138">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="7ae67-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7ae67-139">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7ae67-139">Request headers</span></span>

| <span data-ttu-id="7ae67-140">Name</span><span class="sxs-lookup"><span data-stu-id="7ae67-140">Name</span></span>          | <span data-ttu-id="7ae67-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7ae67-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="7ae67-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ae67-142">Authorization</span></span> | <span data-ttu-id="7ae67-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7ae67-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="7ae67-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="7ae67-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="7ae67-146">CSV</span><span class="sxs-lookup"><span data-stu-id="7ae67-146">CSV</span></span>

<span data-ttu-id="7ae67-147">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="7ae67-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="7ae67-148">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7ae67-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="7ae67-149">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="7ae67-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="7ae67-150">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="7ae67-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="7ae67-151">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="7ae67-151">Report Refresh Date</span></span>
- <span data-ttu-id="7ae67-152">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="7ae67-152">User Principal Name</span></span>
- <span data-ttu-id="7ae67-153">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="7ae67-153">Display Name</span></span>
- <span data-ttu-id="7ae67-154">Benutzerstatus</span><span class="sxs-lookup"><span data-stu-id="7ae67-154">User State</span></span>
- <span data-ttu-id="7ae67-155">Datum der Statusänderung</span><span class="sxs-lookup"><span data-stu-id="7ae67-155">State Change Date</span></span>
- <span data-ttu-id="7ae67-156">Datum der letzten Aktivität</span><span class="sxs-lookup"><span data-stu-id="7ae67-156">Last Activity Date</span></span>
- <span data-ttu-id="7ae67-157">Anzahl veröffentlicht</span><span class="sxs-lookup"><span data-stu-id="7ae67-157">Posted Count</span></span>
- <span data-ttu-id="7ae67-158">Anzahl gelesen</span><span class="sxs-lookup"><span data-stu-id="7ae67-158">Read Count</span></span>
- <span data-ttu-id="7ae67-159">Anzahl gelikt</span><span class="sxs-lookup"><span data-stu-id="7ae67-159">Liked Count</span></span>
- <span data-ttu-id="7ae67-160">Zugewiesene Produkte</span><span class="sxs-lookup"><span data-stu-id="7ae67-160">Assigned Products</span></span>
- <span data-ttu-id="7ae67-161">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="7ae67-161">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="7ae67-162">JSON</span><span class="sxs-lookup"><span data-stu-id="7ae67-162">JSON</span></span>

<span data-ttu-id="7ae67-163">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines **[YammerActivityUserDetail](../resources/yammeractivityuserdetail.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="7ae67-163">If successful, this method returns a `200 OK` response code and a **[yammerActivityUserDetail](../resources/yammeractivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="7ae67-164">Die Seite Standardgröße für diese Anforderung ist 200 Elemente.</span><span class="sxs-lookup"><span data-stu-id="7ae67-164">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="7ae67-165">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7ae67-165">Example</span></span>

### <a name="csv"></a><span data-ttu-id="7ae67-166">CSV</span><span class="sxs-lookup"><span data-stu-id="7ae67-166">CSV</span></span>

<span data-ttu-id="7ae67-167">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="7ae67-167">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="7ae67-168">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7ae67-168">Request</span></span>

<span data-ttu-id="7ae67-169">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7ae67-169">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivityuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerActivityUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="7ae67-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="7ae67-170">Response</span></span>

<span data-ttu-id="7ae67-171">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7ae67-171">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="7ae67-172">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="7ae67-172">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="7ae67-173">JSON</span><span class="sxs-lookup"><span data-stu-id="7ae67-173">JSON</span></span>

<span data-ttu-id="7ae67-174">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7ae67-174">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="7ae67-175">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7ae67-175">Request</span></span>

<span data-ttu-id="7ae67-176">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7ae67-176">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivityuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerActivityUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="7ae67-177">Antwort</span><span class="sxs-lookup"><span data-stu-id="7ae67-177">Response</span></span>

<span data-ttu-id="7ae67-178">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7ae67-178">The following is an example of the response.</span></span>

> <span data-ttu-id="7ae67-p108">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="7ae67-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
