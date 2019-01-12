---
title: 'reportRoot: getEmailActivityUserDetail'
description: Erhalten Sie detaillierte Informationen über die von Benutzern ausgeführten E-Mail-Aktivitäten.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 7cb3545b5bf0571e8b7ce45347dfd9931b3095ec
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921913"
---
# <a name="reportroot-getemailactivityuserdetail"></a><span data-ttu-id="39a0e-103">reportRoot: getEmailActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="39a0e-103">reportRoot: getEmailActivityUserDetail</span></span>

> <span data-ttu-id="39a0e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="39a0e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="39a0e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="39a0e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="39a0e-106">Erhalten Sie detaillierte Informationen über die von Benutzern ausgeführten E-Mail-Aktivitäten.</span><span class="sxs-lookup"><span data-stu-id="39a0e-106">Get details about email activity users have performed.</span></span>

> <span data-ttu-id="39a0e-107">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – E-Mail-Aktivität](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span><span class="sxs-lookup"><span data-stu-id="39a0e-107">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="permissions"></a><span data-ttu-id="39a0e-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="39a0e-108">Permissions</span></span>

<span data-ttu-id="39a0e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39a0e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="39a0e-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="39a0e-111">Permission type</span></span>                        | <span data-ttu-id="39a0e-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="39a0e-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="39a0e-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="39a0e-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="39a0e-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="39a0e-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="39a0e-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="39a0e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39a0e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="39a0e-116">Not supported.</span></span>                           |
| <span data-ttu-id="39a0e-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="39a0e-117">Application</span></span>                            | <span data-ttu-id="39a0e-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="39a0e-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="39a0e-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="39a0e-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailActivityUserDetail(period='{period_value}')
GET /reports/getEmailActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="39a0e-120">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="39a0e-120">Function parameters</span></span>

<span data-ttu-id="39a0e-121">Geben Sie in der Anforderungs-URL einen der folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="39a0e-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="39a0e-122">Parameter</span><span class="sxs-lookup"><span data-stu-id="39a0e-122">Parameter</span></span> | <span data-ttu-id="39a0e-123">Typ</span><span class="sxs-lookup"><span data-stu-id="39a0e-123">Type</span></span>   | <span data-ttu-id="39a0e-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="39a0e-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="39a0e-125">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="39a0e-125">period</span></span>    | <span data-ttu-id="39a0e-126">string</span><span class="sxs-lookup"><span data-stu-id="39a0e-126">string</span></span> | <span data-ttu-id="39a0e-127">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="39a0e-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="39a0e-128">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="39a0e-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="39a0e-129">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="39a0e-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="39a0e-130">date</span><span class="sxs-lookup"><span data-stu-id="39a0e-130">date</span></span>      | <span data-ttu-id="39a0e-131">Datum</span><span class="sxs-lookup"><span data-stu-id="39a0e-131">Date</span></span>   | <span data-ttu-id="39a0e-132">Gibt das Datum an, für das die Benutzer angezeigt werden sollen, die Aktivitäten durchgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="39a0e-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="39a0e-133">{date_value} muss im Format JJJJ-MM-TT vorliegen.</span><span class="sxs-lookup"><span data-stu-id="39a0e-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="39a0e-134">Da dieser Bericht nur für die letzten 30 Tage verfügbar ist, sollte {date_value} ein Datum aus diesem Zeitraum sein.</span><span class="sxs-lookup"><span data-stu-id="39a0e-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="39a0e-135">**Hinweis:** Sie müssen in der URL entweder einen Zeitraum oder ein Datum festlegen.</span><span class="sxs-lookup"><span data-stu-id="39a0e-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="39a0e-136">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) von  `$format`, `$top` und `$skipToken` zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="39a0e-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="39a0e-137">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="39a0e-137">The default output type is text/csv.</span></span> <span data-ttu-id="39a0e-138">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="39a0e-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="39a0e-139">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="39a0e-139">Request headers</span></span>

| <span data-ttu-id="39a0e-140">Name</span><span class="sxs-lookup"><span data-stu-id="39a0e-140">Name</span></span>          | <span data-ttu-id="39a0e-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="39a0e-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="39a0e-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="39a0e-142">Authorization</span></span> | <span data-ttu-id="39a0e-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="39a0e-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="39a0e-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="39a0e-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="39a0e-146">CSV</span><span class="sxs-lookup"><span data-stu-id="39a0e-146">CSV</span></span>

<span data-ttu-id="39a0e-147">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="39a0e-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="39a0e-148">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="39a0e-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="39a0e-149">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="39a0e-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="39a0e-150">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="39a0e-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="39a0e-151">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="39a0e-151">Report Refresh Date</span></span>
- <span data-ttu-id="39a0e-152">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="39a0e-152">User Principal Name</span></span>
- <span data-ttu-id="39a0e-153">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="39a0e-153">Display Name</span></span>
- <span data-ttu-id="39a0e-154">Ist gelöscht</span><span class="sxs-lookup"><span data-stu-id="39a0e-154">Is Deleted</span></span>
- <span data-ttu-id="39a0e-155">Gelöscht am</span><span class="sxs-lookup"><span data-stu-id="39a0e-155">Deleted Date</span></span>
- <span data-ttu-id="39a0e-156">Datum der letzten Aktivität</span><span class="sxs-lookup"><span data-stu-id="39a0e-156">Last Activity Date</span></span>
- <span data-ttu-id="39a0e-157">Anzahl gesendet</span><span class="sxs-lookup"><span data-stu-id="39a0e-157">Send Count</span></span>
- <span data-ttu-id="39a0e-158">Anzahl empfangen</span><span class="sxs-lookup"><span data-stu-id="39a0e-158">Receive Count</span></span>
- <span data-ttu-id="39a0e-159">Anzahl gelesen</span><span class="sxs-lookup"><span data-stu-id="39a0e-159">Read Count</span></span>
- <span data-ttu-id="39a0e-160">Zugewiesene Produkte</span><span class="sxs-lookup"><span data-stu-id="39a0e-160">Assigned Products</span></span>
- <span data-ttu-id="39a0e-161">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="39a0e-161">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="39a0e-162">JSON</span><span class="sxs-lookup"><span data-stu-id="39a0e-162">JSON</span></span>

<span data-ttu-id="39a0e-163">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200 OK` Antwortcode und eines **[EmailActivityUserDetail](../resources/emailactivityuserdetail.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="39a0e-163">If successful, this method returns a `200 OK` response code and an **[emailActivityUserDetail](../resources/emailactivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="39a0e-164">Die Seite Standardgröße für diese Anforderung ist 200 Elemente.</span><span class="sxs-lookup"><span data-stu-id="39a0e-164">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="39a0e-165">Beispiel</span><span class="sxs-lookup"><span data-stu-id="39a0e-165">Example</span></span>

### <a name="csv"></a><span data-ttu-id="39a0e-166">CSV</span><span class="sxs-lookup"><span data-stu-id="39a0e-166">CSV</span></span>

<span data-ttu-id="39a0e-167">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="39a0e-167">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="39a0e-168">Anforderung</span><span class="sxs-lookup"><span data-stu-id="39a0e-168">Request</span></span>

<span data-ttu-id="39a0e-169">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="39a0e-169">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailactivityuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailActivityUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="39a0e-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="39a0e-170">Response</span></span>

<span data-ttu-id="39a0e-171">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="39a0e-171">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="39a0e-172">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="39a0e-172">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Last Activity Date,Send Count,Receive Count,Read Count,Assigned Products,Report Period
```

### <a name="json"></a><span data-ttu-id="39a0e-173">JSON</span><span class="sxs-lookup"><span data-stu-id="39a0e-173">JSON</span></span>

<span data-ttu-id="39a0e-174">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="39a0e-174">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="39a0e-175">Anforderung</span><span class="sxs-lookup"><span data-stu-id="39a0e-175">Request</span></span>

<span data-ttu-id="39a0e-176">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="39a0e-176">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailactivityuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailActivityUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="39a0e-177">Antwort</span><span class="sxs-lookup"><span data-stu-id="39a0e-177">Response</span></span>

<span data-ttu-id="39a0e-178">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="39a0e-178">The following is an example of the response.</span></span>

> <span data-ttu-id="39a0e-p108">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="39a0e-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailActivityUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 424

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailActivityUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "displayName": "displayName-value", 
      "isDeleted": false, 
      "deletedDate": null, 
      "lastActivityDate": "2017-09-01", 
      "sendCount": 86, 
      "receiveCount": 3198, 
      "readCount": 388, 
      "assignedProducts": [
        "OFFICE 365 ENTERPRISE E5"
      ], 
      "reportPeriod": "7"
    }
  ]
}
```
