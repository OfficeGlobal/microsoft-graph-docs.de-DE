---
title: 'reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts'
description: Rufen Sie die Anzahl der Benutzer ab, die eigene Geräte in Ihrer Organisation verwenden. Der Bericht enthält die Anzahl der Benutzer pro Gerät, einschließlich Windows, Windows Phone, Android-Smartphone, iPhone und iPad.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: c31dd67e40d1fc4933847db874cfdf81f72479bf
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574901"
---
# <a name="reportroot-getskypeforbusinessdeviceusagedistributionusercounts"></a><span data-ttu-id="aa3d1-104">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="aa3d1-104">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa3d1-105">Rufen Sie die Anzahl der Benutzer ab, die eigene Geräte in Ihrer Organisation verwenden.</span><span class="sxs-lookup"><span data-stu-id="aa3d1-105">Get the number of users using unique devices in your organization.</span></span> <span data-ttu-id="aa3d1-106">Der Bericht enthält die Anzahl der Benutzer pro Gerät, einschließlich Windows, Windows Phone, Android-Smartphone, iPhone und iPad.</span><span class="sxs-lookup"><span data-stu-id="aa3d1-106">The report will show you the number of users per device including Windows, Windows phone, Android phone, iPhone, and iPad.</span></span>

> <span data-ttu-id="aa3d1-107">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Verwendete Skype for Business-Clients](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span><span class="sxs-lookup"><span data-stu-id="aa3d1-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="aa3d1-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="aa3d1-108">Permissions</span></span>

<span data-ttu-id="aa3d1-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa3d1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="aa3d1-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="aa3d1-111">Permission type</span></span>                        | <span data-ttu-id="aa3d1-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="aa3d1-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="aa3d1-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="aa3d1-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="aa3d1-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="aa3d1-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="aa3d1-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="aa3d1-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa3d1-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="aa3d1-116">Not supported.</span></span>                           |
| <span data-ttu-id="aa3d1-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="aa3d1-117">Application</span></span>                            | <span data-ttu-id="aa3d1-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="aa3d1-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="aa3d1-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="aa3d1-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="aa3d1-120">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="aa3d1-120">Function parameters</span></span>

<span data-ttu-id="aa3d1-121">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="aa3d1-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="aa3d1-122">Parameter</span><span class="sxs-lookup"><span data-stu-id="aa3d1-122">Parameter</span></span> | <span data-ttu-id="aa3d1-123">Typ</span><span class="sxs-lookup"><span data-stu-id="aa3d1-123">Type</span></span>   | <span data-ttu-id="aa3d1-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aa3d1-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="aa3d1-125">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="aa3d1-125">period</span></span>    | <span data-ttu-id="aa3d1-126">string</span><span class="sxs-lookup"><span data-stu-id="aa3d1-126">string</span></span> | <span data-ttu-id="aa3d1-127">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="aa3d1-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="aa3d1-128">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="aa3d1-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="aa3d1-129">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="aa3d1-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="aa3d1-130">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="aa3d1-130">Required.</span></span> |

<span data-ttu-id="aa3d1-131">Diese Methode unterstützt die `$format` [OData-Abfragezeichenfolgen-Parameter](/graph/query-parameters) zum Anpassen der Antwort.</span><span class="sxs-lookup"><span data-stu-id="aa3d1-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="aa3d1-132">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="aa3d1-132">The default output type is text/csv.</span></span> <span data-ttu-id="aa3d1-133">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="aa3d1-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aa3d1-134">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="aa3d1-134">Request headers</span></span>

| <span data-ttu-id="aa3d1-135">Name</span><span class="sxs-lookup"><span data-stu-id="aa3d1-135">Name</span></span>          | <span data-ttu-id="aa3d1-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aa3d1-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="aa3d1-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa3d1-137">Authorization</span></span> | <span data-ttu-id="aa3d1-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="aa3d1-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="aa3d1-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="aa3d1-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="aa3d1-141">CSV</span><span class="sxs-lookup"><span data-stu-id="aa3d1-141">CSV</span></span>

<span data-ttu-id="aa3d1-142">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="aa3d1-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="aa3d1-143">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="aa3d1-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="aa3d1-144">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="aa3d1-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="aa3d1-145">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="aa3d1-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="aa3d1-146">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="aa3d1-146">Report Refresh Date</span></span>
- <span data-ttu-id="aa3d1-147">Windows</span><span class="sxs-lookup"><span data-stu-id="aa3d1-147">Windows</span></span>
- <span data-ttu-id="aa3d1-148">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="aa3d1-148">Windows Phone</span></span>
- <span data-ttu-id="aa3d1-149">Android-Smartphone</span><span class="sxs-lookup"><span data-stu-id="aa3d1-149">Android Phone</span></span>
- <span data-ttu-id="aa3d1-150">iPhone</span><span class="sxs-lookup"><span data-stu-id="aa3d1-150">iPhone</span></span>
- <span data-ttu-id="aa3d1-151">iPad</span><span class="sxs-lookup"><span data-stu-id="aa3d1-151">iPad</span></span>
- <span data-ttu-id="aa3d1-152">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="aa3d1-152">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="aa3d1-153">JSON</span><span class="sxs-lookup"><span data-stu-id="aa3d1-153">JSON</span></span>

<span data-ttu-id="aa3d1-154">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines **[SkypeForBusinessDeviceUsageDistributionUserCounts](../resources/skypeforbusinessdeviceusagedistributionusercounts.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="aa3d1-154">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessDeviceUsageDistributionUserCounts](../resources/skypeforbusinessdeviceusagedistributionusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa3d1-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="aa3d1-155">Example</span></span>

### <a name="csv"></a><span data-ttu-id="aa3d1-156">CSV</span><span class="sxs-lookup"><span data-stu-id="aa3d1-156">CSV</span></span>

<span data-ttu-id="aa3d1-157">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="aa3d1-157">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="aa3d1-158">Anforderung</span><span class="sxs-lookup"><span data-stu-id="aa3d1-158">Request</span></span>

<span data-ttu-id="aa3d1-159">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="aa3d1-159">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusagedistributionusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="aa3d1-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="aa3d1-160">Response</span></span>

<span data-ttu-id="aa3d1-161">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="aa3d1-161">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="aa3d1-162">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="aa3d1-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Windows,Windows Phone,Android Phone,iPhone,iPad,Report Period
```

### <a name="json"></a><span data-ttu-id="aa3d1-163">JSON</span><span class="sxs-lookup"><span data-stu-id="aa3d1-163">JSON</span></span>

<span data-ttu-id="aa3d1-164">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aa3d1-164">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="aa3d1-165">Anforderung</span><span class="sxs-lookup"><span data-stu-id="aa3d1-165">Request</span></span>

<span data-ttu-id="aa3d1-166">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="aa3d1-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusagedistributionusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="aa3d1-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="aa3d1-167">Response</span></span>

<span data-ttu-id="aa3d1-168">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="aa3d1-168">The following is an example of the response.</span></span>

> <span data-ttu-id="aa3d1-p108">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="aa3d1-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageDistributionUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 275

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessDeviceUsageDistributionUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "windows": 122, 
      "windowsPhone": 8, 
      "androidPhone": 19, 
      "iPhone": 28, 
      "iPad": 1, 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessdeviceusagedistributionusercounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
