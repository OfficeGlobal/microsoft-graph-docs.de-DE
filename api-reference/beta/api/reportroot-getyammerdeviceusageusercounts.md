---
title: 'reportRoot: getYammerDeviceUsageUserCounts'
description: Erhalten Sie die Anzahl der täglichen Benutzer nach Gerätetyp.
localization_priority: Normal
ms.openlocfilehash: 78c17de276e45b12936fcdf0f4b58c975388d101
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812621"
---
# <a name="reportroot-getyammerdeviceusageusercounts"></a><span data-ttu-id="960f6-103">reportRoot: getYammerDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="960f6-103">reportRoot: getYammerDeviceUsageUserCounts</span></span>

> <span data-ttu-id="960f6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="960f6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="960f6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="960f6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="960f6-106">Erhalten Sie die Anzahl der täglichen Benutzer nach Gerätetyp.</span><span class="sxs-lookup"><span data-stu-id="960f6-106">Get the number of daily users by device type.</span></span>

> <span data-ttu-id="960f6-107">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Yammer-Gerätenutzung](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="960f6-107">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="960f6-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="960f6-108">Permissions</span></span>

<span data-ttu-id="960f6-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="960f6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="960f6-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="960f6-111">Permission type</span></span>                        | <span data-ttu-id="960f6-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="960f6-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="960f6-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="960f6-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="960f6-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="960f6-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="960f6-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="960f6-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="960f6-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="960f6-116">Not supported.</span></span>                           |
| <span data-ttu-id="960f6-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="960f6-117">Application</span></span>                            | <span data-ttu-id="960f6-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="960f6-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="960f6-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="960f6-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="960f6-120">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="960f6-120">Function parameters</span></span>

<span data-ttu-id="960f6-121">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="960f6-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="960f6-122">Parameter</span><span class="sxs-lookup"><span data-stu-id="960f6-122">Parameter</span></span> | <span data-ttu-id="960f6-123">Typ</span><span class="sxs-lookup"><span data-stu-id="960f6-123">Type</span></span>   | <span data-ttu-id="960f6-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="960f6-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="960f6-125">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="960f6-125">period</span></span>    | <span data-ttu-id="960f6-126">string</span><span class="sxs-lookup"><span data-stu-id="960f6-126">string</span></span> | <span data-ttu-id="960f6-127">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="960f6-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="960f6-128">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="960f6-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="960f6-129">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="960f6-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="960f6-130">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="960f6-130">Required.</span></span> |

<span data-ttu-id="960f6-131">Diese Methode unterstützt die `$format` [OData-Abfragezeichenfolgen-Parameter](/graph/query-parameters) zum Anpassen der Antwort.</span><span class="sxs-lookup"><span data-stu-id="960f6-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="960f6-132">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="960f6-132">The default output type is text/csv.</span></span> <span data-ttu-id="960f6-133">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="960f6-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="960f6-134">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="960f6-134">Request headers</span></span>

| <span data-ttu-id="960f6-135">Name</span><span class="sxs-lookup"><span data-stu-id="960f6-135">Name</span></span>          | <span data-ttu-id="960f6-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="960f6-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="960f6-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="960f6-137">Authorization</span></span> | <span data-ttu-id="960f6-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="960f6-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="960f6-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="960f6-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="960f6-141">CSV</span><span class="sxs-lookup"><span data-stu-id="960f6-141">CSV</span></span>

<span data-ttu-id="960f6-142">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="960f6-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="960f6-143">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="960f6-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="960f6-144">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="960f6-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="960f6-145">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="960f6-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="960f6-146">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="960f6-146">Report Refresh Date</span></span>
- <span data-ttu-id="960f6-147">Web</span><span class="sxs-lookup"><span data-stu-id="960f6-147">Web</span></span>
- <span data-ttu-id="960f6-148">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="960f6-148">Windows Phone</span></span>
- <span data-ttu-id="960f6-149">Android-Smartphone</span><span class="sxs-lookup"><span data-stu-id="960f6-149">Android Phone</span></span>
- <span data-ttu-id="960f6-150">iPhone</span><span class="sxs-lookup"><span data-stu-id="960f6-150">iPhone</span></span>
- <span data-ttu-id="960f6-151">iPad</span><span class="sxs-lookup"><span data-stu-id="960f6-151">iPad</span></span>
- <span data-ttu-id="960f6-152">Andere</span><span class="sxs-lookup"><span data-stu-id="960f6-152">Other</span></span>
- <span data-ttu-id="960f6-153">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="960f6-153">Report Date</span></span>
- <span data-ttu-id="960f6-154">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="960f6-154">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="960f6-155">JSON</span><span class="sxs-lookup"><span data-stu-id="960f6-155">JSON</span></span>

<span data-ttu-id="960f6-156">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines **[YammerDeviceUsageUserCounts](../resources/yammerdeviceusageusercounts.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="960f6-156">If successful, this method returns a `200 OK` response code and a **[yammerDeviceUsageUserCounts](../resources/yammerdeviceusageusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="960f6-157">Beispiel</span><span class="sxs-lookup"><span data-stu-id="960f6-157">Example</span></span>

### <a name="csv"></a><span data-ttu-id="960f6-158">CSV</span><span class="sxs-lookup"><span data-stu-id="960f6-158">CSV</span></span>

<span data-ttu-id="960f6-159">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="960f6-159">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="960f6-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="960f6-160">Request</span></span>

<span data-ttu-id="960f6-161">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="960f6-161">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusageusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="960f6-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="960f6-162">Response</span></span>

<span data-ttu-id="960f6-163">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="960f6-163">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="960f6-164">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="960f6-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iPhone,iPad,Other,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="960f6-165">JSON</span><span class="sxs-lookup"><span data-stu-id="960f6-165">JSON</span></span>

<span data-ttu-id="960f6-166">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="960f6-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="960f6-167">Anforderung</span><span class="sxs-lookup"><span data-stu-id="960f6-167">Request</span></span>

<span data-ttu-id="960f6-168">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="960f6-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusageusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="960f6-169">Antwort</span><span class="sxs-lookup"><span data-stu-id="960f6-169">Response</span></span>

<span data-ttu-id="960f6-170">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="960f6-170">The following is an example of the response.</span></span>

> <span data-ttu-id="960f6-p107">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="960f6-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerDeviceUsageUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 284

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerDeviceUsageUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "web": 63, 
      "windowsPhone": 1, 
      "androidPhone": 17, 
      "iPhone": 23, 
      "iPad": 1, 
      "other": 2, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
