---
title: 'reportRoot: getOffice365ServicesUserCounts'
description: Rufen Sie die Anzahl der Benutzer nach Aktivitätstyp und Dienst ab.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: f04f892e3bcfe593ebd1d5a4ca04cf70f0dd38e7
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572808"
---
# <a name="reportroot-getoffice365servicesusercounts"></a><span data-ttu-id="976b6-103">reportRoot: getOffice365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="976b6-103">reportRoot: getOffice365ServicesUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="976b6-104">Rufen Sie die Anzahl der Benutzer nach Aktivitätstyp und Dienst ab.</span><span class="sxs-lookup"><span data-stu-id="976b6-104">Get the count of users by activity type and service.</span></span>

> <span data-ttu-id="976b6-105">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Aktive Benutzer](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="976b6-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="976b6-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="976b6-106">Permissions</span></span>

<span data-ttu-id="976b6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="976b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="976b6-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="976b6-109">Permission type</span></span>                        | <span data-ttu-id="976b6-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="976b6-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="976b6-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="976b6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="976b6-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="976b6-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="976b6-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="976b6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="976b6-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="976b6-114">Not supported.</span></span>                           |
| <span data-ttu-id="976b6-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="976b6-115">Application</span></span>                            | <span data-ttu-id="976b6-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="976b6-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="976b6-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="976b6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ServicesUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="976b6-118">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="976b6-118">Function parameters</span></span>

<span data-ttu-id="976b6-119">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="976b6-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="976b6-120">Parameter</span><span class="sxs-lookup"><span data-stu-id="976b6-120">Parameter</span></span> | <span data-ttu-id="976b6-121">Typ</span><span class="sxs-lookup"><span data-stu-id="976b6-121">Type</span></span>   | <span data-ttu-id="976b6-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="976b6-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="976b6-123">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="976b6-123">period</span></span>    | <span data-ttu-id="976b6-124">string</span><span class="sxs-lookup"><span data-stu-id="976b6-124">string</span></span> | <span data-ttu-id="976b6-125">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="976b6-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="976b6-126">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="976b6-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="976b6-127">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="976b6-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="976b6-128">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="976b6-128">Required.</span></span> |

<span data-ttu-id="976b6-129">Diese Methode unterstützt die `$format` [OData-Abfragezeichenfolgen-Parameter](/graph/query-parameters) zum Anpassen der Antwort.</span><span class="sxs-lookup"><span data-stu-id="976b6-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="976b6-130">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="976b6-130">The default output type is text/csv.</span></span> <span data-ttu-id="976b6-131">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="976b6-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="976b6-132">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="976b6-132">Request headers</span></span>

| <span data-ttu-id="976b6-133">Name</span><span class="sxs-lookup"><span data-stu-id="976b6-133">Name</span></span>          | <span data-ttu-id="976b6-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="976b6-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="976b6-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="976b6-135">Authorization</span></span> | <span data-ttu-id="976b6-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="976b6-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="976b6-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="976b6-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="976b6-139">CSV</span><span class="sxs-lookup"><span data-stu-id="976b6-139">CSV</span></span>

<span data-ttu-id="976b6-140">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="976b6-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="976b6-141">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="976b6-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="976b6-142">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="976b6-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="976b6-143">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="976b6-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="976b6-144">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="976b6-144">Report Refresh Date</span></span>
- <span data-ttu-id="976b6-145">Exchange aktiv</span><span class="sxs-lookup"><span data-stu-id="976b6-145">Exchange Active</span></span>
- <span data-ttu-id="976b6-146">Exchange inaktiv</span><span class="sxs-lookup"><span data-stu-id="976b6-146">Exchange Inactive</span></span>
- <span data-ttu-id="976b6-147">OneDrive aktiv</span><span class="sxs-lookup"><span data-stu-id="976b6-147">OneDrive Active</span></span>
- <span data-ttu-id="976b6-148">OneDrive inaktiv</span><span class="sxs-lookup"><span data-stu-id="976b6-148">OneDrive Inactive</span></span>
- <span data-ttu-id="976b6-149">SharePoint aktiv</span><span class="sxs-lookup"><span data-stu-id="976b6-149">SharePoint Active</span></span>
- <span data-ttu-id="976b6-150">SharePoint inaktiv</span><span class="sxs-lookup"><span data-stu-id="976b6-150">SharePoint Inactive</span></span>
- <span data-ttu-id="976b6-151">Skype for Business aktiv</span><span class="sxs-lookup"><span data-stu-id="976b6-151">Skype For Business Active</span></span>
- <span data-ttu-id="976b6-152">Skype for Business inaktiv</span><span class="sxs-lookup"><span data-stu-id="976b6-152">Skype For Business Inactive</span></span>
- <span data-ttu-id="976b6-153">Yammer aktiv</span><span class="sxs-lookup"><span data-stu-id="976b6-153">Yammer Active</span></span>
- <span data-ttu-id="976b6-154">Yammer inaktiv</span><span class="sxs-lookup"><span data-stu-id="976b6-154">Yammer Inactive</span></span>
- <span data-ttu-id="976b6-155">Teams aktiv</span><span class="sxs-lookup"><span data-stu-id="976b6-155">Teams Active</span></span>
- <span data-ttu-id="976b6-156">Teams inaktiv</span><span class="sxs-lookup"><span data-stu-id="976b6-156">Teams Inactive</span></span>
- <span data-ttu-id="976b6-157">Office 365 aktiv</span><span class="sxs-lookup"><span data-stu-id="976b6-157">Office 365 Active</span></span>
- <span data-ttu-id="976b6-158">Office 365 inaktiv</span><span class="sxs-lookup"><span data-stu-id="976b6-158">Office 365 Inactive</span></span>
- <span data-ttu-id="976b6-159">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="976b6-159">Report Period</span></span>

<span data-ttu-id="976b6-160">Die folgenden Spalten werden in Microsoft Graph China vom Dienst 21Vianet nicht unterstützt:</span><span class="sxs-lookup"><span data-stu-id="976b6-160">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="976b6-161">Yammer aktiv</span><span class="sxs-lookup"><span data-stu-id="976b6-161">Yammer Active</span></span>
- <span data-ttu-id="976b6-162">Yammer inaktiv</span><span class="sxs-lookup"><span data-stu-id="976b6-162">Yammer Inactive</span></span>
- <span data-ttu-id="976b6-163">Teams aktiv</span><span class="sxs-lookup"><span data-stu-id="976b6-163">Teams Active</span></span>
- <span data-ttu-id="976b6-164">Teams inaktiv</span><span class="sxs-lookup"><span data-stu-id="976b6-164">Teams Inactive</span></span>

### <a name="json"></a><span data-ttu-id="976b6-165">JSON</span><span class="sxs-lookup"><span data-stu-id="976b6-165">JSON</span></span>

<span data-ttu-id="976b6-166">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200 OK` Antwortcode und eines **[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="976b6-166">If successful, this method returns a `200 OK` response code and an **[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** object in the response body.</span></span>

<span data-ttu-id="976b6-167">Die folgenden Eigenschaften im **[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** -Objekt werden in Microsoft Graph China vom Dienst 21Vianet nicht unterstützt:</span><span class="sxs-lookup"><span data-stu-id="976b6-167">The following properties in **[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="976b6-168">yammerActive</span><span class="sxs-lookup"><span data-stu-id="976b6-168">yammerActive</span></span>
- <span data-ttu-id="976b6-169">yammerInactive</span><span class="sxs-lookup"><span data-stu-id="976b6-169">yammerInactive</span></span>
- <span data-ttu-id="976b6-170">teamsActive</span><span class="sxs-lookup"><span data-stu-id="976b6-170">teamsActive</span></span>
- <span data-ttu-id="976b6-171">teamsInactive</span><span class="sxs-lookup"><span data-stu-id="976b6-171">teamsInactive</span></span>

## <a name="example"></a><span data-ttu-id="976b6-172">Beispiel</span><span class="sxs-lookup"><span data-stu-id="976b6-172">Example</span></span>

### <a name="csv"></a><span data-ttu-id="976b6-173">CSV</span><span class="sxs-lookup"><span data-stu-id="976b6-173">CSV</span></span>

<span data-ttu-id="976b6-174">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="976b6-174">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="976b6-175">Anforderung</span><span class="sxs-lookup"><span data-stu-id="976b6-175">Request</span></span>

<span data-ttu-id="976b6-176">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="976b6-176">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365servicesusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ServicesUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="976b6-177">Antwort</span><span class="sxs-lookup"><span data-stu-id="976b6-177">Response</span></span>

<span data-ttu-id="976b6-178">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="976b6-178">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="976b6-179">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="976b6-179">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Exchange Active,Exchange Inactive,OneDrive Active,OneDrive Inactive,SharePoint Active,SharePoint Inactive,Skype For Business Active,Skype For Business Inactive,Yammer Active,Yammer Inactive,Teams Active,Teams Inactive,Report Period
```

### <a name="json"></a><span data-ttu-id="976b6-180">JSON</span><span class="sxs-lookup"><span data-stu-id="976b6-180">JSON</span></span> 

<span data-ttu-id="976b6-181">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="976b6-181">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="976b6-182">Anforderung</span><span class="sxs-lookup"><span data-stu-id="976b6-182">Request</span></span>

<span data-ttu-id="976b6-183">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="976b6-183">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365servicesusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ServicesUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="976b6-184">Antwort</span><span class="sxs-lookup"><span data-stu-id="976b6-184">Response</span></span>

<span data-ttu-id="976b6-185">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="976b6-185">The following is an example of the response.</span></span>

> <span data-ttu-id="976b6-p106">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="976b6-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ServicesUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 458

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365ServicesUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "exchangeActive": 2591, 
      "exchangeInactive": 1426, 
      "oneDriveActive": 1800, 
      "oneDriveInactive": 2451, 
      "sharePointActive": 2286, 
      "sharePointInactive": 1815, 
      "skypeForBusinessActive": 2463, 
      "skypeForBusinessInactive": 1947, 
      "yammerActive": 473, 
      "yammerInactive": 2526, 
      "teamsActive": 846, 
      "teamsInactive": 1960, 
      "office365Active": 2791,
      "office365Inactive": 503,
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getoffice365servicesusercounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
