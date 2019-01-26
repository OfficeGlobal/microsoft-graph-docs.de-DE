---
title: 'reportRoot: getYammerDeviceUsageDistributionUserCounts'
description: Erhalten Sie die Anzahl der Benutzer nach Gerätetyp.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 407960889f20178b03ad3865959d99cb8a1a417b
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577312"
---
# <a name="reportroot-getyammerdeviceusagedistributionusercounts"></a><span data-ttu-id="3054d-103">reportRoot: getYammerDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="3054d-103">reportRoot: getYammerDeviceUsageDistributionUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3054d-104">Erhalten Sie die Anzahl der Benutzer nach Gerätetyp.</span><span class="sxs-lookup"><span data-stu-id="3054d-104">Get the number of users by device type.</span></span>

> <span data-ttu-id="3054d-105">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Yammer-Gerätenutzung](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="3054d-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="3054d-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3054d-106">Permissions</span></span>

<span data-ttu-id="3054d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3054d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3054d-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3054d-109">Permission type</span></span>                        | <span data-ttu-id="3054d-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3054d-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="3054d-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3054d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3054d-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3054d-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="3054d-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3054d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3054d-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3054d-114">Not supported.</span></span>                           |
| <span data-ttu-id="3054d-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3054d-115">Application</span></span>                            | <span data-ttu-id="3054d-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3054d-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="3054d-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3054d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="3054d-118">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="3054d-118">Function parameters</span></span>

<span data-ttu-id="3054d-119">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="3054d-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="3054d-120">Parameter</span><span class="sxs-lookup"><span data-stu-id="3054d-120">Parameter</span></span> | <span data-ttu-id="3054d-121">Typ</span><span class="sxs-lookup"><span data-stu-id="3054d-121">Type</span></span>   | <span data-ttu-id="3054d-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3054d-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="3054d-123">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="3054d-123">period</span></span>    | <span data-ttu-id="3054d-124">string</span><span class="sxs-lookup"><span data-stu-id="3054d-124">string</span></span> | <span data-ttu-id="3054d-125">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="3054d-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="3054d-126">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="3054d-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="3054d-127">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="3054d-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="3054d-128">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="3054d-128">Required.</span></span> |

<span data-ttu-id="3054d-129">Diese Methode unterstützt die `$format` [OData-Abfragezeichenfolgen-Parameter](/graph/query-parameters) zum Anpassen der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3054d-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="3054d-130">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="3054d-130">The default output type is text/csv.</span></span> <span data-ttu-id="3054d-131">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="3054d-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3054d-132">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3054d-132">Request headers</span></span>

| <span data-ttu-id="3054d-133">Name</span><span class="sxs-lookup"><span data-stu-id="3054d-133">Name</span></span>          | <span data-ttu-id="3054d-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3054d-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="3054d-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="3054d-135">Authorization</span></span> | <span data-ttu-id="3054d-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3054d-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="3054d-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="3054d-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="3054d-139">CSV</span><span class="sxs-lookup"><span data-stu-id="3054d-139">CSV</span></span>

<span data-ttu-id="3054d-140">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="3054d-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="3054d-141">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3054d-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="3054d-142">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="3054d-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="3054d-143">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="3054d-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="3054d-144">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="3054d-144">Report Refresh Date</span></span>
- <span data-ttu-id="3054d-145">Web</span><span class="sxs-lookup"><span data-stu-id="3054d-145">Web</span></span>
- <span data-ttu-id="3054d-146">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="3054d-146">Windows Phone</span></span>
- <span data-ttu-id="3054d-147">Android-Smartphone</span><span class="sxs-lookup"><span data-stu-id="3054d-147">Android Phone</span></span>
- <span data-ttu-id="3054d-148">iPhone</span><span class="sxs-lookup"><span data-stu-id="3054d-148">iPhone</span></span>
- <span data-ttu-id="3054d-149">iPad</span><span class="sxs-lookup"><span data-stu-id="3054d-149">iPad</span></span>
- <span data-ttu-id="3054d-150">Andere</span><span class="sxs-lookup"><span data-stu-id="3054d-150">Other</span></span>
- <span data-ttu-id="3054d-151">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="3054d-151">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="3054d-152">JSON</span><span class="sxs-lookup"><span data-stu-id="3054d-152">JSON</span></span>

<span data-ttu-id="3054d-153">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines **[YammerDeviceUsageDistributionUserCounts](../resources/yammerdeviceusagedistributionusercounts.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="3054d-153">If successful, this method returns a `200 OK` response code and a **[yammerDeviceUsageDistributionUserCounts](../resources/yammerdeviceusagedistributionusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3054d-154">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3054d-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="3054d-155">CSV</span><span class="sxs-lookup"><span data-stu-id="3054d-155">CSV</span></span>

<span data-ttu-id="3054d-156">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="3054d-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="3054d-157">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3054d-157">Request</span></span>

<span data-ttu-id="3054d-158">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3054d-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusagedistributionusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageDistributionUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="3054d-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="3054d-159">Response</span></span>

<span data-ttu-id="3054d-160">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3054d-160">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="3054d-161">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="3054d-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iPhone,iPad,Other,Report Period
```

### <a name="json"></a><span data-ttu-id="3054d-162">JSON</span><span class="sxs-lookup"><span data-stu-id="3054d-162">JSON</span></span>

<span data-ttu-id="3054d-163">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3054d-163">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="3054d-164">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3054d-164">Request</span></span>

<span data-ttu-id="3054d-165">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3054d-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusagedistributionusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageDistributionUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="3054d-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="3054d-166">Response</span></span>

<span data-ttu-id="3054d-167">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3054d-167">The following is an example of the response.</span></span>

> <span data-ttu-id="3054d-p106">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="3054d-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerDeviceUsageDistributionUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 271

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerDeviceUsageDistributionUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "web": 138, 
      "windowsPhone": 1, 
      "androidPhone": 29, 
      "iPhone": 40, 
      "iPad": 2, 
      "other": 2, 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getyammerdeviceusagedistributionusercounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
