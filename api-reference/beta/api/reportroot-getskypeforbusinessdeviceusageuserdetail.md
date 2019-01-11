---
title: 'reportRoot: getSkypeForBusinessDeviceUsageUserDetail'
description: Rufen Sie Details der Skype for Business-Gerätenutzung nach Benutzer ab.
localization_priority: Normal
ms.openlocfilehash: 6fcf60b248b34c097b59139901e3d0204808034d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27881991"
---
# <a name="reportroot-getskypeforbusinessdeviceusageuserdetail"></a><span data-ttu-id="0e86e-103">reportRoot: getSkypeForBusinessDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="0e86e-103">reportRoot: getSkypeForBusinessDeviceUsageUserDetail</span></span>

> <span data-ttu-id="0e86e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0e86e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0e86e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0e86e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0e86e-106">Rufen Sie Details der Skype for Business-Gerätenutzung nach Benutzer ab.</span><span class="sxs-lookup"><span data-stu-id="0e86e-106">Get details about Skype for Business device usage by user.</span></span>

> <span data-ttu-id="0e86e-107">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Verwendete Skype for Business-Clients](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span><span class="sxs-lookup"><span data-stu-id="0e86e-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="0e86e-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0e86e-108">Permissions</span></span>

<span data-ttu-id="0e86e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e86e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0e86e-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0e86e-111">Permission type</span></span>                        | <span data-ttu-id="0e86e-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0e86e-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="0e86e-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0e86e-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="0e86e-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0e86e-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="0e86e-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0e86e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e86e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0e86e-116">Not supported.</span></span>                           |
| <span data-ttu-id="0e86e-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0e86e-117">Application</span></span>                            | <span data-ttu-id="0e86e-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0e86e-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="0e86e-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0e86e-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="0e86e-120">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="0e86e-120">Function parameters</span></span>

<span data-ttu-id="0e86e-121">Geben Sie in der Anforderungs-URL einen der folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="0e86e-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="0e86e-122">Parameter</span><span class="sxs-lookup"><span data-stu-id="0e86e-122">Parameter</span></span> | <span data-ttu-id="0e86e-123">Typ</span><span class="sxs-lookup"><span data-stu-id="0e86e-123">Type</span></span>   | <span data-ttu-id="0e86e-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0e86e-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="0e86e-125">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="0e86e-125">period</span></span>    | <span data-ttu-id="0e86e-126">string</span><span class="sxs-lookup"><span data-stu-id="0e86e-126">string</span></span> | <span data-ttu-id="0e86e-127">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="0e86e-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="0e86e-128">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="0e86e-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="0e86e-129">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="0e86e-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="0e86e-130">date</span><span class="sxs-lookup"><span data-stu-id="0e86e-130">date</span></span>      | <span data-ttu-id="0e86e-131">Datum</span><span class="sxs-lookup"><span data-stu-id="0e86e-131">Date</span></span>   | <span data-ttu-id="0e86e-132">Gibt das Datum an, für das die Benutzer angezeigt werden sollen, die Aktivitäten durchgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="0e86e-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="0e86e-133">{date_value} muss im Format JJJJ-MM-TT vorliegen.</span><span class="sxs-lookup"><span data-stu-id="0e86e-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="0e86e-134">Da dieser Bericht nur für die letzten 30 Tage verfügbar ist, sollte {date_value} ein Datum aus diesem Zeitraum sein.</span><span class="sxs-lookup"><span data-stu-id="0e86e-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="0e86e-135">**Hinweis:** Sie müssen in der URL entweder einen Zeitraum oder ein Datum festlegen.</span><span class="sxs-lookup"><span data-stu-id="0e86e-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="0e86e-136">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) von  `$format`, `$top` und `$skipToken` zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0e86e-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="0e86e-137">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="0e86e-137">The default output type is text/csv.</span></span> <span data-ttu-id="0e86e-138">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="0e86e-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0e86e-139">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0e86e-139">Request headers</span></span>

| <span data-ttu-id="0e86e-140">Name</span><span class="sxs-lookup"><span data-stu-id="0e86e-140">Name</span></span>          | <span data-ttu-id="0e86e-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0e86e-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="0e86e-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e86e-142">Authorization</span></span> | <span data-ttu-id="0e86e-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0e86e-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="0e86e-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="0e86e-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="0e86e-146">CSV</span><span class="sxs-lookup"><span data-stu-id="0e86e-146">CSV</span></span>

<span data-ttu-id="0e86e-147">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="0e86e-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="0e86e-148">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0e86e-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="0e86e-149">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="0e86e-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="0e86e-150">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="0e86e-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="0e86e-151">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="0e86e-151">Report Refresh Date</span></span>
- <span data-ttu-id="0e86e-152">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="0e86e-152">User Principal Name</span></span>
- <span data-ttu-id="0e86e-153">Datum der letzten Aktivität</span><span class="sxs-lookup"><span data-stu-id="0e86e-153">Last Activity Date</span></span>
- <span data-ttu-id="0e86e-154">Verwendetes Windows</span><span class="sxs-lookup"><span data-stu-id="0e86e-154">Used Windows</span></span>
- <span data-ttu-id="0e86e-155">Verwendetes Windows Phone</span><span class="sxs-lookup"><span data-stu-id="0e86e-155">Used Windows Phone</span></span>
- <span data-ttu-id="0e86e-156">Verwendetes Android Phone</span><span class="sxs-lookup"><span data-stu-id="0e86e-156">Used Android Phone</span></span>
- <span data-ttu-id="0e86e-157">Verwendetes iPhone</span><span class="sxs-lookup"><span data-stu-id="0e86e-157">Used iPhone</span></span>
- <span data-ttu-id="0e86e-158">Verwendetes iPad</span><span class="sxs-lookup"><span data-stu-id="0e86e-158">Used iPad</span></span>
- <span data-ttu-id="0e86e-159">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="0e86e-159">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="0e86e-160">JSON</span><span class="sxs-lookup"><span data-stu-id="0e86e-160">JSON</span></span>

<span data-ttu-id="0e86e-161">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines **[SkypeForBusinessDeviceUsageUserDetail](../resources/skypeforbusinessdeviceusageuserdetail.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="0e86e-161">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessDeviceUsageUserDetail](../resources/skypeforbusinessdeviceusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="0e86e-162">Die Seite Standardgröße für diese Anforderung ist 200 Elemente.</span><span class="sxs-lookup"><span data-stu-id="0e86e-162">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="0e86e-163">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0e86e-163">Example</span></span>

### <a name="csv"></a><span data-ttu-id="0e86e-164">CSV</span><span class="sxs-lookup"><span data-stu-id="0e86e-164">CSV</span></span>

<span data-ttu-id="0e86e-165">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="0e86e-165">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="0e86e-166">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0e86e-166">Request</span></span>

<span data-ttu-id="0e86e-167">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0e86e-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusageuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="0e86e-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="0e86e-168">Response</span></span>

<span data-ttu-id="0e86e-169">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0e86e-169">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="0e86e-170">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="0e86e-170">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="0e86e-171">JSON</span><span class="sxs-lookup"><span data-stu-id="0e86e-171">JSON</span></span>

<span data-ttu-id="0e86e-172">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0e86e-172">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="0e86e-173">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0e86e-173">Request</span></span>

<span data-ttu-id="0e86e-174">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0e86e-174">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusageuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="0e86e-175">Antwort</span><span class="sxs-lookup"><span data-stu-id="0e86e-175">Response</span></span>

<span data-ttu-id="0e86e-176">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0e86e-176">The following is an example of the response.</span></span>

> <span data-ttu-id="0e86e-p108">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="0e86e-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
