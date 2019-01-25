---
title: 'reportRoot: getSkypeForBusinessDeviceUsageUserCounts'
description: Erfahren Sie mehr über Auslastungstrends, indem Sie sich ansehen, wie viele Benutzer in Ihrer Organisation sich über die Skype for Business-App verbunden haben. Außerdem erhalten Sie eine Auflistung des Gerätetyps (Windows, Windows Phone, Android-Smartphone, iPhone oder iPad) auf dem die Skype for Business-Client-App installiert und in Ihrer Organisation verwendet wird.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 4191f398ee4a230a5ec3cce8123079f6fe1a3465
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514488"
---
# <a name="reportroot-getskypeforbusinessdeviceusageusercounts"></a><span data-ttu-id="64550-104">reportRoot: getSkypeForBusinessDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="64550-104">reportRoot: getSkypeForBusinessDeviceUsageUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64550-105">Erfahren Sie mehr über Auslastungstrends, indem Sie sich ansehen, wie viele Benutzer in Ihrer Organisation sich über die Skype for Business-App verbunden haben.</span><span class="sxs-lookup"><span data-stu-id="64550-105">Get the usage trends on how many users in your organization have connected using the Skype for Business app.</span></span> <span data-ttu-id="64550-106">Außerdem erhalten Sie eine Auflistung des Gerätetyps (Windows, Windows Phone, Android-Smartphone, iPhone oder iPad) auf dem die Skype for Business-Client-App installiert und in Ihrer Organisation verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="64550-106">You will also get a breakdown by the type of device (Windows, Windows phone, Android phone, iPhone, or iPad) on which the Skype for Business client app is installed and used across your organization.</span></span>

> <span data-ttu-id="64550-107">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Verwendete Skype for Business-Clients](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span><span class="sxs-lookup"><span data-stu-id="64550-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="64550-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="64550-108">Permissions</span></span>

<span data-ttu-id="64550-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64550-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="64550-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="64550-111">Permission type</span></span>                        | <span data-ttu-id="64550-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="64550-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="64550-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="64550-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="64550-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="64550-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="64550-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="64550-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64550-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="64550-116">Not supported.</span></span>                           |
| <span data-ttu-id="64550-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="64550-117">Application</span></span>                            | <span data-ttu-id="64550-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="64550-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="64550-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="64550-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="64550-120">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="64550-120">Function parameters</span></span>

<span data-ttu-id="64550-121">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="64550-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="64550-122">Parameter</span><span class="sxs-lookup"><span data-stu-id="64550-122">Parameter</span></span> | <span data-ttu-id="64550-123">Typ</span><span class="sxs-lookup"><span data-stu-id="64550-123">Type</span></span>   | <span data-ttu-id="64550-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="64550-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="64550-125">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="64550-125">period</span></span>    | <span data-ttu-id="64550-126">string</span><span class="sxs-lookup"><span data-stu-id="64550-126">string</span></span> | <span data-ttu-id="64550-127">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="64550-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="64550-128">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="64550-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="64550-129">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="64550-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="64550-130">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="64550-130">Required.</span></span> |

<span data-ttu-id="64550-131">Diese Methode unterstützt die `$format` [OData-Abfragezeichenfolgen-Parameter](/graph/query-parameters) zum Anpassen der Antwort.</span><span class="sxs-lookup"><span data-stu-id="64550-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="64550-132">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="64550-132">The default output type is text/csv.</span></span> <span data-ttu-id="64550-133">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="64550-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="64550-134">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="64550-134">Request headers</span></span>

| <span data-ttu-id="64550-135">Name</span><span class="sxs-lookup"><span data-stu-id="64550-135">Name</span></span>          | <span data-ttu-id="64550-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="64550-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="64550-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="64550-137">Authorization</span></span> | <span data-ttu-id="64550-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="64550-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="64550-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="64550-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="64550-141">CSV</span><span class="sxs-lookup"><span data-stu-id="64550-141">CSV</span></span>

<span data-ttu-id="64550-142">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="64550-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="64550-143">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="64550-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="64550-144">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="64550-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="64550-145">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="64550-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="64550-146">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="64550-146">Report Refresh Date</span></span>
- <span data-ttu-id="64550-147">Windows</span><span class="sxs-lookup"><span data-stu-id="64550-147">Windows</span></span>
- <span data-ttu-id="64550-148">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="64550-148">Windows Phone</span></span>
- <span data-ttu-id="64550-149">Android-Smartphone</span><span class="sxs-lookup"><span data-stu-id="64550-149">Android Phone</span></span>
- <span data-ttu-id="64550-150">iPhone</span><span class="sxs-lookup"><span data-stu-id="64550-150">iPhone</span></span>
- <span data-ttu-id="64550-151">iPad</span><span class="sxs-lookup"><span data-stu-id="64550-151">iPad</span></span>
- <span data-ttu-id="64550-152">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="64550-152">Report Date</span></span>
- <span data-ttu-id="64550-153">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="64550-153">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="64550-154">JSON</span><span class="sxs-lookup"><span data-stu-id="64550-154">JSON</span></span>

<span data-ttu-id="64550-155">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines **[SkypeForBusinessDeviceUsageUserCounts](../resources/skypeforbusinessdeviceusageusercounts.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="64550-155">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessDeviceUsageUserCounts](../resources/skypeforbusinessdeviceusageusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64550-156">Beispiel</span><span class="sxs-lookup"><span data-stu-id="64550-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="64550-157">CSV</span><span class="sxs-lookup"><span data-stu-id="64550-157">CSV</span></span>

<span data-ttu-id="64550-158">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="64550-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="64550-159">Anforderung</span><span class="sxs-lookup"><span data-stu-id="64550-159">Request</span></span>

<span data-ttu-id="64550-160">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="64550-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusageusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="64550-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="64550-161">Response</span></span>

<span data-ttu-id="64550-162">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="64550-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="64550-163">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="64550-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="64550-164">JSON</span><span class="sxs-lookup"><span data-stu-id="64550-164">JSON</span></span>

<span data-ttu-id="64550-165">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="64550-165">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="64550-166">Anforderung</span><span class="sxs-lookup"><span data-stu-id="64550-166">Request</span></span>

<span data-ttu-id="64550-167">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="64550-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusageusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="64550-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="64550-168">Response</span></span>

<span data-ttu-id="64550-169">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="64550-169">The following is an example of the response.</span></span>

> <span data-ttu-id="64550-p108">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="64550-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessdeviceusageusercounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
