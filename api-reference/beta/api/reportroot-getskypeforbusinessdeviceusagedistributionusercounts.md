---
title: 'reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts'
description: Rufen Sie die Anzahl der Benutzer ab, die eigene Geräte in Ihrer Organisation verwenden. Der Bericht enthält die Anzahl der Benutzer pro Gerät, einschließlich Windows, Windows Phone, Android-Smartphone, iPhone und iPad.
localization_priority: Normal
ms.openlocfilehash: 87385d36b6af3451b71a7886c9da7187b4a2c1ba
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831801"
---
# <a name="reportroot-getskypeforbusinessdeviceusagedistributionusercounts"></a><span data-ttu-id="ed210-104">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="ed210-104">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span></span>

> <span data-ttu-id="ed210-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ed210-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ed210-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ed210-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ed210-107">Rufen Sie die Anzahl der Benutzer ab, die eigene Geräte in Ihrer Organisation verwenden.</span><span class="sxs-lookup"><span data-stu-id="ed210-107">Get the number of users using unique devices in your organization.</span></span> <span data-ttu-id="ed210-108">Der Bericht enthält die Anzahl der Benutzer pro Gerät, einschließlich Windows, Windows Phone, Android-Smartphone, iPhone und iPad.</span><span class="sxs-lookup"><span data-stu-id="ed210-108">The report will show you the number of users per device including Windows, Windows phone, Android phone, iPhone, and iPad.</span></span>

> <span data-ttu-id="ed210-109">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Verwendete Skype for Business-Clients](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span><span class="sxs-lookup"><span data-stu-id="ed210-109">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="ed210-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ed210-110">Permissions</span></span>

<span data-ttu-id="ed210-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed210-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ed210-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ed210-113">Permission type</span></span>                        | <span data-ttu-id="ed210-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ed210-114">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ed210-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ed210-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="ed210-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ed210-116">Reports.Read.All</span></span>                         |
| <span data-ttu-id="ed210-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ed210-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed210-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ed210-118">Not supported.</span></span>                           |
| <span data-ttu-id="ed210-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ed210-119">Application</span></span>                            | <span data-ttu-id="ed210-120">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ed210-120">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="ed210-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ed210-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="ed210-122">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="ed210-122">Function parameters</span></span>

<span data-ttu-id="ed210-123">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="ed210-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="ed210-124">Parameter</span><span class="sxs-lookup"><span data-stu-id="ed210-124">Parameter</span></span> | <span data-ttu-id="ed210-125">Typ</span><span class="sxs-lookup"><span data-stu-id="ed210-125">Type</span></span>   | <span data-ttu-id="ed210-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ed210-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="ed210-127">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="ed210-127">period</span></span>    | <span data-ttu-id="ed210-128">string</span><span class="sxs-lookup"><span data-stu-id="ed210-128">string</span></span> | <span data-ttu-id="ed210-129">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="ed210-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="ed210-130">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="ed210-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="ed210-131">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="ed210-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="ed210-132">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="ed210-132">Required.</span></span> |

<span data-ttu-id="ed210-133">Diese Methode unterstützt die `$format` [OData-Abfragezeichenfolgen-Parameter](/graph/query-parameters) zum Anpassen der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ed210-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="ed210-134">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="ed210-134">The default output type is text/csv.</span></span> <span data-ttu-id="ed210-135">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="ed210-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ed210-136">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ed210-136">Request headers</span></span>

| <span data-ttu-id="ed210-137">Name</span><span class="sxs-lookup"><span data-stu-id="ed210-137">Name</span></span>          | <span data-ttu-id="ed210-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ed210-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="ed210-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed210-139">Authorization</span></span> | <span data-ttu-id="ed210-p107">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ed210-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="ed210-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="ed210-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="ed210-143">CSV</span><span class="sxs-lookup"><span data-stu-id="ed210-143">CSV</span></span>

<span data-ttu-id="ed210-144">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="ed210-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ed210-145">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ed210-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ed210-146">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="ed210-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="ed210-147">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="ed210-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="ed210-148">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="ed210-148">Report Refresh Date</span></span>
- <span data-ttu-id="ed210-149">Windows</span><span class="sxs-lookup"><span data-stu-id="ed210-149">Windows</span></span>
- <span data-ttu-id="ed210-150">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="ed210-150">Windows Phone</span></span>
- <span data-ttu-id="ed210-151">Android-Smartphone</span><span class="sxs-lookup"><span data-stu-id="ed210-151">Android Phone</span></span>
- <span data-ttu-id="ed210-152">iPhone</span><span class="sxs-lookup"><span data-stu-id="ed210-152">iPhone</span></span>
- <span data-ttu-id="ed210-153">iPad</span><span class="sxs-lookup"><span data-stu-id="ed210-153">iPad</span></span>
- <span data-ttu-id="ed210-154">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="ed210-154">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="ed210-155">JSON</span><span class="sxs-lookup"><span data-stu-id="ed210-155">JSON</span></span>

<span data-ttu-id="ed210-156">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines **[SkypeForBusinessDeviceUsageDistributionUserCounts](../resources/skypeforbusinessdeviceusagedistributionusercounts.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="ed210-156">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessDeviceUsageDistributionUserCounts](../resources/skypeforbusinessdeviceusagedistributionusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed210-157">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ed210-157">Example</span></span>

### <a name="csv"></a><span data-ttu-id="ed210-158">CSV</span><span class="sxs-lookup"><span data-stu-id="ed210-158">CSV</span></span>

<span data-ttu-id="ed210-159">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="ed210-159">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="ed210-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ed210-160">Request</span></span>

<span data-ttu-id="ed210-161">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ed210-161">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusagedistributionusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="ed210-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="ed210-162">Response</span></span>

<span data-ttu-id="ed210-163">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ed210-163">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="ed210-164">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="ed210-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="ed210-165">JSON</span><span class="sxs-lookup"><span data-stu-id="ed210-165">JSON</span></span>

<span data-ttu-id="ed210-166">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ed210-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="ed210-167">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ed210-167">Request</span></span>

<span data-ttu-id="ed210-168">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ed210-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusagedistributionusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="ed210-169">Antwort</span><span class="sxs-lookup"><span data-stu-id="ed210-169">Response</span></span>

<span data-ttu-id="ed210-170">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ed210-170">The following is an example of the response.</span></span>

> <span data-ttu-id="ed210-p109">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="ed210-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
