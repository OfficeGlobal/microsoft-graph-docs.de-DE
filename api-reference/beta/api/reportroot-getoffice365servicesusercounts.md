---
title: 'reportRoot: getOffice365ServicesUserCounts'
description: Rufen Sie die Anzahl der Benutzer nach Aktivitätstyp und Dienst ab.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 90e295b8547074a72d907a0cbfda9583fb2218d1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513872"
---
# <a name="reportroot-getoffice365servicesusercounts"></a><span data-ttu-id="251a0-103">reportRoot: getOffice365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="251a0-103">reportRoot: getOffice365ServicesUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="251a0-104">Rufen Sie die Anzahl der Benutzer nach Aktivitätstyp und Dienst ab.</span><span class="sxs-lookup"><span data-stu-id="251a0-104">Get the count of users by activity type and service.</span></span>

> <span data-ttu-id="251a0-105">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Aktive Benutzer](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="251a0-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="251a0-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="251a0-106">Permissions</span></span>

<span data-ttu-id="251a0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="251a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="251a0-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="251a0-109">Permission type</span></span>                        | <span data-ttu-id="251a0-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="251a0-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="251a0-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="251a0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="251a0-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="251a0-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="251a0-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="251a0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="251a0-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="251a0-114">Not supported.</span></span>                           |
| <span data-ttu-id="251a0-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="251a0-115">Application</span></span>                            | <span data-ttu-id="251a0-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="251a0-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="251a0-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="251a0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ServicesUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="251a0-118">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="251a0-118">Function parameters</span></span>

<span data-ttu-id="251a0-119">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="251a0-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="251a0-120">Parameter</span><span class="sxs-lookup"><span data-stu-id="251a0-120">Parameter</span></span> | <span data-ttu-id="251a0-121">Typ</span><span class="sxs-lookup"><span data-stu-id="251a0-121">Type</span></span>   | <span data-ttu-id="251a0-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="251a0-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="251a0-123">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="251a0-123">period</span></span>    | <span data-ttu-id="251a0-124">string</span><span class="sxs-lookup"><span data-stu-id="251a0-124">string</span></span> | <span data-ttu-id="251a0-125">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="251a0-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="251a0-126">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="251a0-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="251a0-127">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="251a0-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="251a0-128">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="251a0-128">Required.</span></span> |

<span data-ttu-id="251a0-129">Diese Methode unterstützt die `$format` [OData-Abfragezeichenfolgen-Parameter](/graph/query-parameters) zum Anpassen der Antwort.</span><span class="sxs-lookup"><span data-stu-id="251a0-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="251a0-130">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="251a0-130">The default output type is text/csv.</span></span> <span data-ttu-id="251a0-131">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="251a0-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="251a0-132">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="251a0-132">Request headers</span></span>

| <span data-ttu-id="251a0-133">Name</span><span class="sxs-lookup"><span data-stu-id="251a0-133">Name</span></span>          | <span data-ttu-id="251a0-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="251a0-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="251a0-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="251a0-135">Authorization</span></span> | <span data-ttu-id="251a0-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="251a0-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="251a0-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="251a0-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="251a0-139">CSV</span><span class="sxs-lookup"><span data-stu-id="251a0-139">CSV</span></span>

<span data-ttu-id="251a0-140">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="251a0-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="251a0-141">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="251a0-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="251a0-142">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="251a0-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="251a0-143">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="251a0-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="251a0-144">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="251a0-144">Report Refresh Date</span></span>
- <span data-ttu-id="251a0-145">Exchange aktiv</span><span class="sxs-lookup"><span data-stu-id="251a0-145">Exchange Active</span></span>
- <span data-ttu-id="251a0-146">Exchange inaktiv</span><span class="sxs-lookup"><span data-stu-id="251a0-146">Exchange Inactive</span></span>
- <span data-ttu-id="251a0-147">OneDrive aktiv</span><span class="sxs-lookup"><span data-stu-id="251a0-147">OneDrive Active</span></span>
- <span data-ttu-id="251a0-148">OneDrive inaktiv</span><span class="sxs-lookup"><span data-stu-id="251a0-148">OneDrive Inactive</span></span>
- <span data-ttu-id="251a0-149">SharePoint aktiv</span><span class="sxs-lookup"><span data-stu-id="251a0-149">SharePoint Active</span></span>
- <span data-ttu-id="251a0-150">SharePoint inaktiv</span><span class="sxs-lookup"><span data-stu-id="251a0-150">SharePoint Inactive</span></span>
- <span data-ttu-id="251a0-151">Skype for Business aktiv</span><span class="sxs-lookup"><span data-stu-id="251a0-151">Skype For Business Active</span></span>
- <span data-ttu-id="251a0-152">Skype for Business inaktiv</span><span class="sxs-lookup"><span data-stu-id="251a0-152">Skype For Business Inactive</span></span>
- <span data-ttu-id="251a0-153">Yammer aktiv</span><span class="sxs-lookup"><span data-stu-id="251a0-153">Yammer Active</span></span>
- <span data-ttu-id="251a0-154">Yammer inaktiv</span><span class="sxs-lookup"><span data-stu-id="251a0-154">Yammer Inactive</span></span>
- <span data-ttu-id="251a0-155">Teams aktiv</span><span class="sxs-lookup"><span data-stu-id="251a0-155">Teams Active</span></span>
- <span data-ttu-id="251a0-156">Teams inaktiv</span><span class="sxs-lookup"><span data-stu-id="251a0-156">Teams Inactive</span></span>
- <span data-ttu-id="251a0-157">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="251a0-157">Report Period</span></span>

<span data-ttu-id="251a0-158">Die folgenden Spalten werden in Microsoft Graph China vom Dienst 21Vianet nicht unterstützt:</span><span class="sxs-lookup"><span data-stu-id="251a0-158">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="251a0-159">Yammer aktiv</span><span class="sxs-lookup"><span data-stu-id="251a0-159">Yammer Active</span></span>
- <span data-ttu-id="251a0-160">Yammer inaktiv</span><span class="sxs-lookup"><span data-stu-id="251a0-160">Yammer Inactive</span></span>
- <span data-ttu-id="251a0-161">Teams aktiv</span><span class="sxs-lookup"><span data-stu-id="251a0-161">Teams Active</span></span>
- <span data-ttu-id="251a0-162">Teams inaktiv</span><span class="sxs-lookup"><span data-stu-id="251a0-162">Teams Inactive</span></span>

### <a name="json"></a><span data-ttu-id="251a0-163">JSON</span><span class="sxs-lookup"><span data-stu-id="251a0-163">JSON</span></span>

<span data-ttu-id="251a0-164">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200 OK` Antwortcode und eines **[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="251a0-164">If successful, this method returns a `200 OK` response code and an **[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** object in the response body.</span></span>

<span data-ttu-id="251a0-165">Die folgenden Eigenschaften im **[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** -Objekt werden in Microsoft Graph China vom Dienst 21Vianet nicht unterstützt:</span><span class="sxs-lookup"><span data-stu-id="251a0-165">The following properties in **[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="251a0-166">yammerActive</span><span class="sxs-lookup"><span data-stu-id="251a0-166">yammerActive</span></span>
- <span data-ttu-id="251a0-167">yammerInactive</span><span class="sxs-lookup"><span data-stu-id="251a0-167">yammerInactive</span></span>
- <span data-ttu-id="251a0-168">teamsActive</span><span class="sxs-lookup"><span data-stu-id="251a0-168">teamsActive</span></span>
- <span data-ttu-id="251a0-169">teamsInactive</span><span class="sxs-lookup"><span data-stu-id="251a0-169">teamsInactive</span></span>

## <a name="example"></a><span data-ttu-id="251a0-170">Beispiel</span><span class="sxs-lookup"><span data-stu-id="251a0-170">Example</span></span>

### <a name="csv"></a><span data-ttu-id="251a0-171">CSV</span><span class="sxs-lookup"><span data-stu-id="251a0-171">CSV</span></span>

<span data-ttu-id="251a0-172">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="251a0-172">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="251a0-173">Anforderung</span><span class="sxs-lookup"><span data-stu-id="251a0-173">Request</span></span>

<span data-ttu-id="251a0-174">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="251a0-174">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365servicesusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ServicesUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="251a0-175">Antwort</span><span class="sxs-lookup"><span data-stu-id="251a0-175">Response</span></span>

<span data-ttu-id="251a0-176">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="251a0-176">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="251a0-177">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="251a0-177">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="251a0-178">JSON</span><span class="sxs-lookup"><span data-stu-id="251a0-178">JSON</span></span> 

<span data-ttu-id="251a0-179">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="251a0-179">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="251a0-180">Anforderung</span><span class="sxs-lookup"><span data-stu-id="251a0-180">Request</span></span>

<span data-ttu-id="251a0-181">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="251a0-181">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365servicesusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ServicesUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="251a0-182">Antwort</span><span class="sxs-lookup"><span data-stu-id="251a0-182">Response</span></span>

<span data-ttu-id="251a0-183">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="251a0-183">The following is an example of the response.</span></span>

> <span data-ttu-id="251a0-p106">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="251a0-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
