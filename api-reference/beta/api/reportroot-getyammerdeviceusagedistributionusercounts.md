---
title: 'reportRoot: getYammerDeviceUsageDistributionUserCounts'
description: Erhalten Sie die Anzahl der Benutzer nach Gerätetyp.
localization_priority: Normal
ms.openlocfilehash: 96e379c63f2f00ef3c6616df0405ae779f6bc8ff
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886177"
---
# <a name="reportroot-getyammerdeviceusagedistributionusercounts"></a><span data-ttu-id="00ecc-103">reportRoot: getYammerDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="00ecc-103">reportRoot: getYammerDeviceUsageDistributionUserCounts</span></span>

> <span data-ttu-id="00ecc-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="00ecc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="00ecc-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="00ecc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="00ecc-106">Erhalten Sie die Anzahl der Benutzer nach Gerätetyp.</span><span class="sxs-lookup"><span data-stu-id="00ecc-106">Get the number of users by device type.</span></span>

> <span data-ttu-id="00ecc-107">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Yammer-Gerätenutzung](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="00ecc-107">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="00ecc-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="00ecc-108">Permissions</span></span>

<span data-ttu-id="00ecc-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00ecc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="00ecc-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="00ecc-111">Permission type</span></span>                        | <span data-ttu-id="00ecc-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="00ecc-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="00ecc-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="00ecc-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="00ecc-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="00ecc-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="00ecc-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="00ecc-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00ecc-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="00ecc-116">Not supported.</span></span>                           |
| <span data-ttu-id="00ecc-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="00ecc-117">Application</span></span>                            | <span data-ttu-id="00ecc-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="00ecc-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="00ecc-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="00ecc-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="00ecc-120">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="00ecc-120">Function parameters</span></span>

<span data-ttu-id="00ecc-121">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="00ecc-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="00ecc-122">Parameter</span><span class="sxs-lookup"><span data-stu-id="00ecc-122">Parameter</span></span> | <span data-ttu-id="00ecc-123">Typ</span><span class="sxs-lookup"><span data-stu-id="00ecc-123">Type</span></span>   | <span data-ttu-id="00ecc-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="00ecc-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="00ecc-125">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="00ecc-125">period</span></span>    | <span data-ttu-id="00ecc-126">string</span><span class="sxs-lookup"><span data-stu-id="00ecc-126">string</span></span> | <span data-ttu-id="00ecc-127">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="00ecc-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="00ecc-128">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="00ecc-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="00ecc-129">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="00ecc-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="00ecc-130">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="00ecc-130">Required.</span></span> |

<span data-ttu-id="00ecc-131">Diese Methode unterstützt die `$format` [OData-Abfragezeichenfolgen-Parameter](/graph/query-parameters) zum Anpassen der Antwort.</span><span class="sxs-lookup"><span data-stu-id="00ecc-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="00ecc-132">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="00ecc-132">The default output type is text/csv.</span></span> <span data-ttu-id="00ecc-133">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="00ecc-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="00ecc-134">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="00ecc-134">Request headers</span></span>

| <span data-ttu-id="00ecc-135">Name</span><span class="sxs-lookup"><span data-stu-id="00ecc-135">Name</span></span>          | <span data-ttu-id="00ecc-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="00ecc-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="00ecc-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="00ecc-137">Authorization</span></span> | <span data-ttu-id="00ecc-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="00ecc-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="00ecc-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="00ecc-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="00ecc-141">CSV</span><span class="sxs-lookup"><span data-stu-id="00ecc-141">CSV</span></span>

<span data-ttu-id="00ecc-142">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="00ecc-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="00ecc-143">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="00ecc-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="00ecc-144">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="00ecc-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="00ecc-145">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="00ecc-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="00ecc-146">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="00ecc-146">Report Refresh Date</span></span>
- <span data-ttu-id="00ecc-147">Web</span><span class="sxs-lookup"><span data-stu-id="00ecc-147">Web</span></span>
- <span data-ttu-id="00ecc-148">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="00ecc-148">Windows Phone</span></span>
- <span data-ttu-id="00ecc-149">Android-Smartphone</span><span class="sxs-lookup"><span data-stu-id="00ecc-149">Android Phone</span></span>
- <span data-ttu-id="00ecc-150">iPhone</span><span class="sxs-lookup"><span data-stu-id="00ecc-150">iPhone</span></span>
- <span data-ttu-id="00ecc-151">iPad</span><span class="sxs-lookup"><span data-stu-id="00ecc-151">iPad</span></span>
- <span data-ttu-id="00ecc-152">Andere</span><span class="sxs-lookup"><span data-stu-id="00ecc-152">Other</span></span>
- <span data-ttu-id="00ecc-153">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="00ecc-153">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="00ecc-154">JSON</span><span class="sxs-lookup"><span data-stu-id="00ecc-154">JSON</span></span>

<span data-ttu-id="00ecc-155">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines **[YammerDeviceUsageDistributionUserCounts](../resources/yammerdeviceusagedistributionusercounts.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="00ecc-155">If successful, this method returns a `200 OK` response code and a **[yammerDeviceUsageDistributionUserCounts](../resources/yammerdeviceusagedistributionusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00ecc-156">Beispiel</span><span class="sxs-lookup"><span data-stu-id="00ecc-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="00ecc-157">CSV</span><span class="sxs-lookup"><span data-stu-id="00ecc-157">CSV</span></span>

<span data-ttu-id="00ecc-158">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="00ecc-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="00ecc-159">Anforderung</span><span class="sxs-lookup"><span data-stu-id="00ecc-159">Request</span></span>

<span data-ttu-id="00ecc-160">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="00ecc-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusagedistributionusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageDistributionUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="00ecc-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="00ecc-161">Response</span></span>

<span data-ttu-id="00ecc-162">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="00ecc-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="00ecc-163">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="00ecc-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="00ecc-164">JSON</span><span class="sxs-lookup"><span data-stu-id="00ecc-164">JSON</span></span>

<span data-ttu-id="00ecc-165">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="00ecc-165">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="00ecc-166">Anforderung</span><span class="sxs-lookup"><span data-stu-id="00ecc-166">Request</span></span>

<span data-ttu-id="00ecc-167">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="00ecc-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusagedistributionusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageDistributionUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="00ecc-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="00ecc-168">Response</span></span>

<span data-ttu-id="00ecc-169">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="00ecc-169">The following is an example of the response.</span></span>

> <span data-ttu-id="00ecc-p107">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="00ecc-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
