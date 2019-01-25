---
title: 'reportRoot: getTeamsDeviceUsageDistributionUserCounts'
description: Abrufen der Anzahl der täglichen eindeutigen Benutzer des Microsoft Teams nach Gerätetyp im ausgewählten Zeitraum.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: c1098bdda5d832aa98934b91c501f4e91a3512dc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522546"
---
# <a name="reportroot-getteamsdeviceusagedistributionusercounts"></a><span data-ttu-id="84cb2-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="84cb2-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84cb2-104">Abrufen der Anzahl der täglichen eindeutigen Benutzer des Microsoft Teams nach Gerätetyp im ausgewählten Zeitraum.</span><span class="sxs-lookup"><span data-stu-id="84cb2-104">Get the number of Microsoft Teams unique users by device type over the selected time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="84cb2-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="84cb2-105">Permissions</span></span>

<span data-ttu-id="84cb2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84cb2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="84cb2-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="84cb2-108">Permission type</span></span>                        | <span data-ttu-id="84cb2-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="84cb2-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="84cb2-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="84cb2-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="84cb2-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="84cb2-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="84cb2-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="84cb2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84cb2-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="84cb2-113">Not supported.</span></span>                           |
| <span data-ttu-id="84cb2-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="84cb2-114">Application</span></span>                            | <span data-ttu-id="84cb2-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="84cb2-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="84cb2-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="84cb2-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="84cb2-117">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="84cb2-117">Function parameters</span></span>

<span data-ttu-id="84cb2-118">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="84cb2-118">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="84cb2-119">Parameter</span><span class="sxs-lookup"><span data-stu-id="84cb2-119">Parameter</span></span> | <span data-ttu-id="84cb2-120">Typ</span><span class="sxs-lookup"><span data-stu-id="84cb2-120">Type</span></span>   | <span data-ttu-id="84cb2-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="84cb2-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="84cb2-122">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="84cb2-122">period</span></span>    | <span data-ttu-id="84cb2-123">string</span><span class="sxs-lookup"><span data-stu-id="84cb2-123">string</span></span> | <span data-ttu-id="84cb2-124">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="84cb2-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="84cb2-125">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="84cb2-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="84cb2-126">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="84cb2-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="84cb2-127">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="84cb2-127">Required.</span></span> |

<span data-ttu-id="84cb2-128">Diese Methode unterstützt die `$format` [OData-Abfragezeichenfolgen-Parameter](/graph/query-parameters) zum Anpassen der Antwort.</span><span class="sxs-lookup"><span data-stu-id="84cb2-128">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="84cb2-129">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="84cb2-129">The default output type is text/csv.</span></span> <span data-ttu-id="84cb2-130">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="84cb2-130">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="84cb2-131">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="84cb2-131">Request headers</span></span>

| <span data-ttu-id="84cb2-132">Name</span><span class="sxs-lookup"><span data-stu-id="84cb2-132">Name</span></span>          | <span data-ttu-id="84cb2-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="84cb2-133">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="84cb2-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="84cb2-134">Authorization</span></span> | <span data-ttu-id="84cb2-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="84cb2-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="84cb2-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="84cb2-137">Response</span></span>

### <a name="csv"></a><span data-ttu-id="84cb2-138">CSV</span><span class="sxs-lookup"><span data-stu-id="84cb2-138">CSV</span></span>

<span data-ttu-id="84cb2-139">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="84cb2-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="84cb2-140">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="84cb2-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="84cb2-141">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="84cb2-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="84cb2-142">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="84cb2-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="84cb2-143">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="84cb2-143">Report Refresh Date</span></span>
- <span data-ttu-id="84cb2-144">Web</span><span class="sxs-lookup"><span data-stu-id="84cb2-144">Web</span></span>
- <span data-ttu-id="84cb2-145">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="84cb2-145">Windows Phone</span></span>
- <span data-ttu-id="84cb2-146">Android-Smartphone</span><span class="sxs-lookup"><span data-stu-id="84cb2-146">Android Phone</span></span>
- <span data-ttu-id="84cb2-147">iOS</span><span class="sxs-lookup"><span data-stu-id="84cb2-147">iOS</span></span>
- <span data-ttu-id="84cb2-148">Mac</span><span class="sxs-lookup"><span data-stu-id="84cb2-148">Mac</span></span>
- <span data-ttu-id="84cb2-149">Windows</span><span class="sxs-lookup"><span data-stu-id="84cb2-149">Windows</span></span>
- <span data-ttu-id="84cb2-150">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="84cb2-150">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="84cb2-151">JSON</span><span class="sxs-lookup"><span data-stu-id="84cb2-151">JSON</span></span>

<span data-ttu-id="84cb2-152">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines **[TeamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="84cb2-152">If successful, this method returns a `200 OK` response code and a **[teamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84cb2-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="84cb2-153">Example</span></span>

### <a name="csv"></a><span data-ttu-id="84cb2-154">CSV</span><span class="sxs-lookup"><span data-stu-id="84cb2-154">CSV</span></span>

<span data-ttu-id="84cb2-155">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="84cb2-155">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="84cb2-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="84cb2-156">Request</span></span>

<span data-ttu-id="84cb2-157">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="84cb2-157">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="84cb2-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="84cb2-158">Response</span></span>

<span data-ttu-id="84cb2-159">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="84cb2-159">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="84cb2-160">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="84cb2-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="84cb2-161">JSON</span><span class="sxs-lookup"><span data-stu-id="84cb2-161">JSON</span></span>

<span data-ttu-id="84cb2-162">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="84cb2-162">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="84cb2-163">Anforderung</span><span class="sxs-lookup"><span data-stu-id="84cb2-163">Request</span></span>

<span data-ttu-id="84cb2-164">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="84cb2-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="84cb2-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="84cb2-165">Response</span></span>

<span data-ttu-id="84cb2-166">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="84cb2-166">The following is an example of the response.</span></span>

> <span data-ttu-id="84cb2-p106">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="84cb2-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getteamsdeviceusagedistributionusercounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
