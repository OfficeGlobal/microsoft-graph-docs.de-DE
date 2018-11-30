---
title: 'reportRoot: getTeamsDeviceUsageDistributionUserCounts'
description: Abrufen der Anzahl der täglichen eindeutigen Benutzer des Microsoft Teams nach Gerätetyp im ausgewählten Zeitraum.
ms.openlocfilehash: b2416b8a4aa257f49807efb3f320fcf16cea4920
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063697"
---
# <a name="reportroot-getteamsdeviceusagedistributionusercounts"></a><span data-ttu-id="29821-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="29821-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span></span>

> <span data-ttu-id="29821-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="29821-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="29821-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="29821-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="29821-106">Abrufen der Anzahl der täglichen eindeutigen Benutzer des Microsoft Teams nach Gerätetyp im ausgewählten Zeitraum.</span><span class="sxs-lookup"><span data-stu-id="29821-106">Get the number of Microsoft Teams unique users by device type over the selected time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="29821-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="29821-107">Permissions</span></span>

<span data-ttu-id="29821-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29821-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="29821-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="29821-110">Permission type</span></span>                        | <span data-ttu-id="29821-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="29821-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="29821-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="29821-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="29821-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="29821-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="29821-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="29821-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29821-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="29821-115">Not supported.</span></span>                           |
| <span data-ttu-id="29821-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="29821-116">Application</span></span>                            | <span data-ttu-id="29821-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="29821-117">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="29821-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="29821-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="29821-119">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="29821-119">Function parameters</span></span>

<span data-ttu-id="29821-120">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="29821-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="29821-121">Parameter</span><span class="sxs-lookup"><span data-stu-id="29821-121">Parameter</span></span> | <span data-ttu-id="29821-122">Typ</span><span class="sxs-lookup"><span data-stu-id="29821-122">Type</span></span>   | <span data-ttu-id="29821-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="29821-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="29821-124">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="29821-124">period</span></span>    | <span data-ttu-id="29821-125">string</span><span class="sxs-lookup"><span data-stu-id="29821-125">string</span></span> | <span data-ttu-id="29821-126">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="29821-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="29821-127">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="29821-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="29821-128">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="29821-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="29821-129">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="29821-129">Required.</span></span> |

<span data-ttu-id="29821-130">Diese Methode unterstützt die `$format` [OData-Abfragezeichenfolgen-Parameter](/graph/query-parameters) zum Anpassen der Antwort.</span><span class="sxs-lookup"><span data-stu-id="29821-130">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="29821-131">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="29821-131">The default output type is text/csv.</span></span> <span data-ttu-id="29821-132">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="29821-132">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="29821-133">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="29821-133">Request headers</span></span>

| <span data-ttu-id="29821-134">Name</span><span class="sxs-lookup"><span data-stu-id="29821-134">Name</span></span>          | <span data-ttu-id="29821-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="29821-135">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="29821-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="29821-136">Authorization</span></span> | <span data-ttu-id="29821-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="29821-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="29821-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="29821-139">Response</span></span>

### <a name="csv"></a><span data-ttu-id="29821-140">CSV</span><span class="sxs-lookup"><span data-stu-id="29821-140">CSV</span></span>

<span data-ttu-id="29821-141">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="29821-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="29821-142">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="29821-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="29821-143">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="29821-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="29821-144">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="29821-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="29821-145">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="29821-145">Report Refresh Date</span></span>
- <span data-ttu-id="29821-146">Web</span><span class="sxs-lookup"><span data-stu-id="29821-146">Web</span></span>
- <span data-ttu-id="29821-147">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="29821-147">Windows Phone</span></span>
- <span data-ttu-id="29821-148">Android-Smartphone</span><span class="sxs-lookup"><span data-stu-id="29821-148">Android Phone</span></span>
- <span data-ttu-id="29821-149">iOS</span><span class="sxs-lookup"><span data-stu-id="29821-149">iOS</span></span>
- <span data-ttu-id="29821-150">Mac</span><span class="sxs-lookup"><span data-stu-id="29821-150">Mac</span></span>
- <span data-ttu-id="29821-151">Windows</span><span class="sxs-lookup"><span data-stu-id="29821-151">Windows</span></span>
- <span data-ttu-id="29821-152">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="29821-152">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="29821-153">JSON</span><span class="sxs-lookup"><span data-stu-id="29821-153">JSON</span></span>

<span data-ttu-id="29821-154">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines **[TeamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="29821-154">If successful, this method returns a `200 OK` response code and a **[teamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29821-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="29821-155">Example</span></span>

### <a name="csv"></a><span data-ttu-id="29821-156">CSV</span><span class="sxs-lookup"><span data-stu-id="29821-156">CSV</span></span>

<span data-ttu-id="29821-157">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="29821-157">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="29821-158">Anforderung</span><span class="sxs-lookup"><span data-stu-id="29821-158">Request</span></span>

<span data-ttu-id="29821-159">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="29821-159">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="29821-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="29821-160">Response</span></span>

<span data-ttu-id="29821-161">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="29821-161">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="29821-162">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="29821-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iOS,Mac,Windows,Report Period
```

### <a name="json"></a><span data-ttu-id="29821-163">JSON</span><span class="sxs-lookup"><span data-stu-id="29821-163">JSON</span></span>

<span data-ttu-id="29821-164">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="29821-164">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="29821-165">Anforderung</span><span class="sxs-lookup"><span data-stu-id="29821-165">Request</span></span>

<span data-ttu-id="29821-166">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="29821-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="29821-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="29821-167">Response</span></span>

<span data-ttu-id="29821-168">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="29821-168">The following is an example of the response.</span></span>

> <span data-ttu-id="29821-p107">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="29821-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsDeviceUsageDistributionUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 243

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsDeviceUsageDistributionUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "web": 51, 
      "windowsPhone": 2, 
      "androidPhone": 34, 
      "ios": 76, 
      "mac": 40, 
      "windows": 491, 
      "reportPeriod": "7"
    }
  ]
}
```
