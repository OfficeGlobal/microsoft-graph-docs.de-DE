---
title: 'reportRoot: getOffice365ActiveUserCounts'
description: Rufen Sie die Anzahl der im Berichtszeitraum täglich aktiven Benutzer nach Produkt ab.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 9b24008a3ea13308f0d83a2ac6a6ef31ece32469
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575314"
---
# <a name="reportroot-getoffice365activeusercounts"></a><span data-ttu-id="b9570-103">reportRoot: getOffice365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="b9570-103">reportRoot: getOffice365ActiveUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9570-104">Rufen Sie die Anzahl der im Berichtszeitraum täglich aktiven Benutzer nach Produkt ab.</span><span class="sxs-lookup"><span data-stu-id="b9570-104">Get the count of daily active users in the reporting period by product.</span></span>

> <span data-ttu-id="b9570-105">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Aktive Benutzer](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="b9570-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="b9570-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b9570-106">Permissions</span></span>

<span data-ttu-id="b9570-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9570-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b9570-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b9570-109">Permission type</span></span>                        | <span data-ttu-id="b9570-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b9570-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b9570-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b9570-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b9570-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9570-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b9570-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b9570-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9570-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b9570-114">Not supported.</span></span>                           |
| <span data-ttu-id="b9570-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b9570-115">Application</span></span>                            | <span data-ttu-id="b9570-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9570-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="b9570-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b9570-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="b9570-118">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="b9570-118">Function parameters</span></span>

<span data-ttu-id="b9570-119">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="b9570-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="b9570-120">Parameter</span><span class="sxs-lookup"><span data-stu-id="b9570-120">Parameter</span></span> | <span data-ttu-id="b9570-121">Typ</span><span class="sxs-lookup"><span data-stu-id="b9570-121">Type</span></span>   | <span data-ttu-id="b9570-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b9570-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="b9570-123">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="b9570-123">period</span></span>    | <span data-ttu-id="b9570-124">string</span><span class="sxs-lookup"><span data-stu-id="b9570-124">string</span></span> | <span data-ttu-id="b9570-125">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="b9570-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="b9570-126">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="b9570-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="b9570-127">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="b9570-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="b9570-128">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="b9570-128">Required.</span></span> |

<span data-ttu-id="b9570-129">Diese Methode unterstützt die `$format` [OData-Abfragezeichenfolgen-Parameter](/graph/query-parameters) zum Anpassen der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b9570-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="b9570-130">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="b9570-130">The default output type is text/csv.</span></span> <span data-ttu-id="b9570-131">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="b9570-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b9570-132">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b9570-132">Request headers</span></span>

| <span data-ttu-id="b9570-133">Name</span><span class="sxs-lookup"><span data-stu-id="b9570-133">Name</span></span>          | <span data-ttu-id="b9570-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b9570-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="b9570-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9570-135">Authorization</span></span> | <span data-ttu-id="b9570-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b9570-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="b9570-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="b9570-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="b9570-139">CSV</span><span class="sxs-lookup"><span data-stu-id="b9570-139">CSV</span></span>

<span data-ttu-id="b9570-140">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="b9570-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b9570-141">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b9570-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b9570-142">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="b9570-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b9570-143">Die CSV-Datei verfügt über die folgenden Spaltenheader:</span><span class="sxs-lookup"><span data-stu-id="b9570-143">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="b9570-144">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="b9570-144">Report Refresh Date</span></span>
- <span data-ttu-id="b9570-145">Office 365</span><span class="sxs-lookup"><span data-stu-id="b9570-145">Office 365</span></span>
- <span data-ttu-id="b9570-146">Exchange</span><span class="sxs-lookup"><span data-stu-id="b9570-146">Exchange</span></span>
- <span data-ttu-id="b9570-147">OneDrive</span><span class="sxs-lookup"><span data-stu-id="b9570-147">OneDrive</span></span>
- <span data-ttu-id="b9570-148">SharePoint</span><span class="sxs-lookup"><span data-stu-id="b9570-148">SharePoint</span></span>
- <span data-ttu-id="b9570-149">Skype for Business</span><span class="sxs-lookup"><span data-stu-id="b9570-149">Skype For Business</span></span> 
- <span data-ttu-id="b9570-150">Yammer</span><span class="sxs-lookup"><span data-stu-id="b9570-150">Yammer</span></span>
- <span data-ttu-id="b9570-151">Teams</span><span class="sxs-lookup"><span data-stu-id="b9570-151">Teams</span></span>
- <span data-ttu-id="b9570-152">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="b9570-152">Report Date</span></span>
- <span data-ttu-id="b9570-153">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="b9570-153">Report Period</span></span>

<span data-ttu-id="b9570-154">Die folgenden Spalten werden in Microsoft Graph China vom Dienst 21Vianet nicht unterstützt:</span><span class="sxs-lookup"><span data-stu-id="b9570-154">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="b9570-155">Yammer</span><span class="sxs-lookup"><span data-stu-id="b9570-155">Yammer</span></span>
- <span data-ttu-id="b9570-156">Teams</span><span class="sxs-lookup"><span data-stu-id="b9570-156">Teams</span></span>

### <a name="json"></a><span data-ttu-id="b9570-157">JSON</span><span class="sxs-lookup"><span data-stu-id="b9570-157">JSON</span></span>

<span data-ttu-id="b9570-158">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200 OK` Antwortcode und eines **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="b9570-158">If successful, this method returns a `200 OK` response code and an **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** object in the response body.</span></span>

<span data-ttu-id="b9570-159">Die folgenden Eigenschaften im **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** -Objekt werden in Microsoft Graph China vom Dienst 21Vianet nicht unterstützt:</span><span class="sxs-lookup"><span data-stu-id="b9570-159">The following properties in **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="b9570-160">Yammer</span><span class="sxs-lookup"><span data-stu-id="b9570-160">yammer</span></span>
- <span data-ttu-id="b9570-161">Teams</span><span class="sxs-lookup"><span data-stu-id="b9570-161">teams</span></span>

## <a name="example"></a><span data-ttu-id="b9570-162">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b9570-162">Example</span></span>

### <a name="csv"></a><span data-ttu-id="b9570-163">CSV</span><span class="sxs-lookup"><span data-stu-id="b9570-163">CSV</span></span>

<span data-ttu-id="b9570-164">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="b9570-164">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="b9570-165">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b9570-165">Request</span></span>

<span data-ttu-id="b9570-166">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b9570-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="b9570-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="b9570-167">Response</span></span>

<span data-ttu-id="b9570-168">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b9570-168">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="b9570-169">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="b9570-169">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Office 365,Exchange,OneDrive,SharePoint,Skype For Business,Yammer,Teams,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="b9570-170">JSON</span><span class="sxs-lookup"><span data-stu-id="b9570-170">JSON</span></span>

<span data-ttu-id="b9570-171">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b9570-171">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="b9570-172">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b9570-172">Request</span></span>

<span data-ttu-id="b9570-173">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b9570-173">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="b9570-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="b9570-174">Response</span></span>

<span data-ttu-id="b9570-175">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b9570-175">The following is an example of the response.</span></span>

> <span data-ttu-id="b9570-p106">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="b9570-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ActiveUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 317

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365ActiveUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "office365": 1718, 
      "exchange": 1429, 
      "oneDrive": 350, 
      "sharePoint": 795, 
      "skypeForBusiness": 251, 
      "yammer": 47, 
      "teams": 10, 
      "reportDate": "2017-08-29", 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getoffice365activeusercounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
