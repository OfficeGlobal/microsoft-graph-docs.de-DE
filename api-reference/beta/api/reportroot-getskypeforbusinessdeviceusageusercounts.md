---
title: 'reportRoot: getSkypeForBusinessDeviceUsageUserCounts'
description: Erfahren Sie mehr über Auslastungstrends, indem Sie sich ansehen, wie viele Benutzer in Ihrer Organisation sich über die Skype for Business-App verbunden haben. Außerdem erhalten Sie eine Auflistung des Gerätetyps (Windows, Windows Phone, Android-Smartphone, iPhone oder iPad) auf dem die Skype for Business-Client-App installiert und in Ihrer Organisation verwendet wird.
ms.openlocfilehash: 21f8746a94860834ad6fdb2465a672f264fee145
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058156"
---
# <a name="reportroot-getskypeforbusinessdeviceusageusercounts"></a><span data-ttu-id="44e32-104">reportRoot: getSkypeForBusinessDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="44e32-104">reportRoot: getSkypeForBusinessDeviceUsageUserCounts</span></span>

> <span data-ttu-id="44e32-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="44e32-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="44e32-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="44e32-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="44e32-107">Erfahren Sie mehr über Auslastungstrends, indem Sie sich ansehen, wie viele Benutzer in Ihrer Organisation sich über die Skype for Business-App verbunden haben.</span><span class="sxs-lookup"><span data-stu-id="44e32-107">Get the usage trends on how many users in your organization have connected using the Skype for Business app.</span></span> <span data-ttu-id="44e32-108">Außerdem erhalten Sie eine Auflistung des Gerätetyps (Windows, Windows Phone, Android-Smartphone, iPhone oder iPad) auf dem die Skype for Business-Client-App installiert und in Ihrer Organisation verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="44e32-108">You will also get a breakdown by the type of device (Windows, Windows phone, Android phone, iPhone, or iPad) on which the Skype for Business client app is installed and used across your organization.</span></span>

> <span data-ttu-id="44e32-109">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Verwendete Skype for Business-Clients](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span><span class="sxs-lookup"><span data-stu-id="44e32-109">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="44e32-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="44e32-110">Permissions</span></span>

<span data-ttu-id="44e32-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44e32-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="44e32-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="44e32-113">Permission type</span></span>                        | <span data-ttu-id="44e32-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="44e32-114">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="44e32-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="44e32-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="44e32-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="44e32-116">Reports.Read.All</span></span>                         |
| <span data-ttu-id="44e32-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="44e32-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44e32-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="44e32-118">Not supported.</span></span>                           |
| <span data-ttu-id="44e32-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="44e32-119">Application</span></span>                            | <span data-ttu-id="44e32-120">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="44e32-120">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="44e32-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="44e32-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="44e32-122">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="44e32-122">Function parameters</span></span>

<span data-ttu-id="44e32-123">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="44e32-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="44e32-124">Parameter</span><span class="sxs-lookup"><span data-stu-id="44e32-124">Parameter</span></span> | <span data-ttu-id="44e32-125">Typ</span><span class="sxs-lookup"><span data-stu-id="44e32-125">Type</span></span>   | <span data-ttu-id="44e32-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="44e32-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="44e32-127">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="44e32-127">period</span></span>    | <span data-ttu-id="44e32-128">string</span><span class="sxs-lookup"><span data-stu-id="44e32-128">string</span></span> | <span data-ttu-id="44e32-129">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="44e32-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="44e32-130">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="44e32-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="44e32-131">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="44e32-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="44e32-132">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="44e32-132">Required.</span></span> |

<span data-ttu-id="44e32-133">Diese Methode unterstützt die `$format` [OData-Abfragezeichenfolgen-Parameter](/graph/query-parameters) zum Anpassen der Antwort.</span><span class="sxs-lookup"><span data-stu-id="44e32-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="44e32-134">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="44e32-134">The default output type is text/csv.</span></span> <span data-ttu-id="44e32-135">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="44e32-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="44e32-136">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="44e32-136">Request headers</span></span>

| <span data-ttu-id="44e32-137">Name</span><span class="sxs-lookup"><span data-stu-id="44e32-137">Name</span></span>          | <span data-ttu-id="44e32-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="44e32-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="44e32-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="44e32-139">Authorization</span></span> | <span data-ttu-id="44e32-p107">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="44e32-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="44e32-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="44e32-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="44e32-143">CSV</span><span class="sxs-lookup"><span data-stu-id="44e32-143">CSV</span></span>

<span data-ttu-id="44e32-144">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="44e32-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="44e32-145">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="44e32-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="44e32-146">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="44e32-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="44e32-147">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="44e32-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="44e32-148">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="44e32-148">Report Refresh Date</span></span>
- <span data-ttu-id="44e32-149">Windows</span><span class="sxs-lookup"><span data-stu-id="44e32-149">Windows</span></span>
- <span data-ttu-id="44e32-150">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="44e32-150">Windows Phone</span></span>
- <span data-ttu-id="44e32-151">Android-Smartphone</span><span class="sxs-lookup"><span data-stu-id="44e32-151">Android Phone</span></span>
- <span data-ttu-id="44e32-152">iPhone</span><span class="sxs-lookup"><span data-stu-id="44e32-152">iPhone</span></span>
- <span data-ttu-id="44e32-153">iPad</span><span class="sxs-lookup"><span data-stu-id="44e32-153">iPad</span></span>
- <span data-ttu-id="44e32-154">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="44e32-154">Report Date</span></span>
- <span data-ttu-id="44e32-155">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="44e32-155">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="44e32-156">JSON</span><span class="sxs-lookup"><span data-stu-id="44e32-156">JSON</span></span>

<span data-ttu-id="44e32-157">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines **[SkypeForBusinessDeviceUsageUserCounts](../resources/skypeforbusinessdeviceusageusercounts.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="44e32-157">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessDeviceUsageUserCounts](../resources/skypeforbusinessdeviceusageusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44e32-158">Beispiel</span><span class="sxs-lookup"><span data-stu-id="44e32-158">Example</span></span>

### <a name="csv"></a><span data-ttu-id="44e32-159">CSV</span><span class="sxs-lookup"><span data-stu-id="44e32-159">CSV</span></span>

<span data-ttu-id="44e32-160">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="44e32-160">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="44e32-161">Anforderung</span><span class="sxs-lookup"><span data-stu-id="44e32-161">Request</span></span>

<span data-ttu-id="44e32-162">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="44e32-162">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusageusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="44e32-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="44e32-163">Response</span></span>

<span data-ttu-id="44e32-164">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="44e32-164">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="44e32-165">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="44e32-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Windows,Windows Phone,Android Phone,iPhone,iPad,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="44e32-166">JSON</span><span class="sxs-lookup"><span data-stu-id="44e32-166">JSON</span></span>

<span data-ttu-id="44e32-167">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="44e32-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="44e32-168">Anforderung</span><span class="sxs-lookup"><span data-stu-id="44e32-168">Request</span></span>

<span data-ttu-id="44e32-169">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="44e32-169">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusageusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="44e32-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="44e32-170">Response</span></span>

<span data-ttu-id="44e32-171">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="44e32-171">The following is an example of the response.</span></span>

> <span data-ttu-id="44e32-p109">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="44e32-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 289

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessDeviceUsageUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "windows": 403, 
      "windowsPhone": 2, 
      "androidPhone": 13, 
      "iPhone": 26, 
      "iPad": 0, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
