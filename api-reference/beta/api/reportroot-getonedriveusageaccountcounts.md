---
title: 'reportRoot: getOneDriveUsageAccountCounts'
description: Rufen Sie die Anzahl der aktiven OneDrive for Business-Benutzer ab. Jede Website, über die Benutzer Dateien angezeigt, geändert, hochgeladen, heruntergeladen, freigegeben oder synchronisiert haben, wird als aktive Website betrachtet.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 76b489a4ceb1fb721ec7ebb4d8892e6e11fc53d2
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576458"
---
# <a name="reportroot-getonedriveusageaccountcounts"></a><span data-ttu-id="4be7b-104">reportRoot: getOneDriveUsageAccountCounts</span><span class="sxs-lookup"><span data-stu-id="4be7b-104">reportRoot: getOneDriveUsageAccountCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4be7b-105">Rufen Sie die Anzahl der aktiven OneDrive for Business-Benutzer ab.</span><span class="sxs-lookup"><span data-stu-id="4be7b-105">Get the trend in the number of active OneDrive for Business sites.</span></span> <span data-ttu-id="4be7b-106">Jede Website, über die Benutzer Dateien angezeigt, geändert, hochgeladen, heruntergeladen, freigegeben oder synchronisiert haben, wird als aktive Website betrachtet.</span><span class="sxs-lookup"><span data-stu-id="4be7b-106">Any site on which users viewed, modified, uploaded, downloaded, shared, or synced files is considered an active site.</span></span>

> <span data-ttu-id="4be7b-107">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – OneDrive for Business-Nutzung](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span><span class="sxs-lookup"><span data-stu-id="4be7b-107">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="4be7b-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4be7b-108">Permissions</span></span>

<span data-ttu-id="4be7b-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4be7b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4be7b-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4be7b-111">Permission type</span></span>                        | <span data-ttu-id="4be7b-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4be7b-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="4be7b-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4be7b-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="4be7b-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4be7b-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="4be7b-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4be7b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4be7b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4be7b-116">Not supported.</span></span>                           |
| <span data-ttu-id="4be7b-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4be7b-117">Application</span></span>                            | <span data-ttu-id="4be7b-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4be7b-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="4be7b-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4be7b-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageAccountCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="4be7b-120">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="4be7b-120">Function parameters</span></span>

<span data-ttu-id="4be7b-121">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="4be7b-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="4be7b-122">Parameter</span><span class="sxs-lookup"><span data-stu-id="4be7b-122">Parameter</span></span> | <span data-ttu-id="4be7b-123">Typ</span><span class="sxs-lookup"><span data-stu-id="4be7b-123">Type</span></span>   | <span data-ttu-id="4be7b-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4be7b-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="4be7b-125">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="4be7b-125">period</span></span>    | <span data-ttu-id="4be7b-126">string</span><span class="sxs-lookup"><span data-stu-id="4be7b-126">string</span></span> | <span data-ttu-id="4be7b-127">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="4be7b-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="4be7b-128">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="4be7b-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="4be7b-129">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="4be7b-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="4be7b-130">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="4be7b-130">Required.</span></span> |

<span data-ttu-id="4be7b-131">Diese Methode unterstützt die `$format` [OData-Abfragezeichenfolgen-Parameter](/graph/query-parameters) zum Anpassen der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4be7b-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="4be7b-132">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="4be7b-132">The default output type is text/csv.</span></span> <span data-ttu-id="4be7b-133">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="4be7b-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4be7b-134">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4be7b-134">Request headers</span></span>

| <span data-ttu-id="4be7b-135">Name</span><span class="sxs-lookup"><span data-stu-id="4be7b-135">Name</span></span>          | <span data-ttu-id="4be7b-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4be7b-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="4be7b-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="4be7b-137">Authorization</span></span> | <span data-ttu-id="4be7b-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4be7b-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="4be7b-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="4be7b-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="4be7b-141">CSV</span><span class="sxs-lookup"><span data-stu-id="4be7b-141">CSV</span></span>

<span data-ttu-id="4be7b-142">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="4be7b-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="4be7b-143">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4be7b-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="4be7b-144">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="4be7b-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="4be7b-145">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="4be7b-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="4be7b-146">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="4be7b-146">Report Refresh Date</span></span>
- <span data-ttu-id="4be7b-147">Websitetyp</span><span class="sxs-lookup"><span data-stu-id="4be7b-147">Site Type</span></span>
- <span data-ttu-id="4be7b-148">Gesamt</span><span class="sxs-lookup"><span data-stu-id="4be7b-148">Total</span></span>
- <span data-ttu-id="4be7b-149">Aktiv</span><span class="sxs-lookup"><span data-stu-id="4be7b-149">Active</span></span>
- <span data-ttu-id="4be7b-150">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="4be7b-150">Report Date</span></span>
- <span data-ttu-id="4be7b-151">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="4be7b-151">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="4be7b-152">JSON</span><span class="sxs-lookup"><span data-stu-id="4be7b-152">JSON</span></span>

<span data-ttu-id="4be7b-153">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines **[OneDriveUsageAccountCounts](../resources/onedriveusageaccountcounts.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="4be7b-153">If successful, this method returns a `200 OK` response code and a **[oneDriveUsageAccountCounts](../resources/onedriveusageaccountcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4be7b-154">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4be7b-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="4be7b-155">CSV</span><span class="sxs-lookup"><span data-stu-id="4be7b-155">CSV</span></span>

<span data-ttu-id="4be7b-156">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="4be7b-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="4be7b-157">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4be7b-157">Request</span></span>

<span data-ttu-id="4be7b-158">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4be7b-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountcounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="4be7b-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="4be7b-159">Response</span></span>

<span data-ttu-id="4be7b-160">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4be7b-160">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="4be7b-161">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="4be7b-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Total,Active,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="4be7b-162">JSON</span><span class="sxs-lookup"><span data-stu-id="4be7b-162">JSON</span></span>

<span data-ttu-id="4be7b-163">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4be7b-163">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="4be7b-164">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4be7b-164">Request</span></span>

<span data-ttu-id="4be7b-165">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4be7b-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountcounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="4be7b-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="4be7b-166">Response</span></span>

<span data-ttu-id="4be7b-167">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4be7b-167">The following is an example of the response.</span></span>

> <span data-ttu-id="4be7b-p108">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="4be7b-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oneDriveUsageAccountCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 249

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.oneDriveUsageAccountCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteType": "All", 
      "total": 207, 
      "active": 89, 
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
    "Error: /api-reference/beta/api/reportroot-getonedriveusageaccountcounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
