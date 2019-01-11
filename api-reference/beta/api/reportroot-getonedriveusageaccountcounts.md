---
title: 'reportRoot: getOneDriveUsageAccountCounts'
description: Rufen Sie die Anzahl der aktiven OneDrive for Business-Benutzer ab. Jede Website, über die Benutzer Dateien angezeigt, geändert, hochgeladen, heruntergeladen, freigegeben oder synchronisiert haben, wird als aktive Website betrachtet.
localization_priority: Normal
ms.openlocfilehash: 2db065d71e741abe9a3a9fe20e3de62b78115cbb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806216"
---
# <a name="reportroot-getonedriveusageaccountcounts"></a><span data-ttu-id="02690-104">reportRoot: getOneDriveUsageAccountCounts</span><span class="sxs-lookup"><span data-stu-id="02690-104">reportRoot: getOneDriveUsageAccountCounts</span></span>

> <span data-ttu-id="02690-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="02690-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="02690-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="02690-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="02690-107">Rufen Sie die Anzahl der aktiven OneDrive for Business-Benutzer ab.</span><span class="sxs-lookup"><span data-stu-id="02690-107">Get the trend in the number of active OneDrive for Business sites.</span></span> <span data-ttu-id="02690-108">Jede Website, über die Benutzer Dateien angezeigt, geändert, hochgeladen, heruntergeladen, freigegeben oder synchronisiert haben, wird als aktive Website betrachtet.</span><span class="sxs-lookup"><span data-stu-id="02690-108">Any site on which users viewed, modified, uploaded, downloaded, shared, or synced files is considered an active site.</span></span>

> <span data-ttu-id="02690-109">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – OneDrive for Business-Nutzung](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span><span class="sxs-lookup"><span data-stu-id="02690-109">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="02690-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="02690-110">Permissions</span></span>

<span data-ttu-id="02690-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02690-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="02690-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="02690-113">Permission type</span></span>                        | <span data-ttu-id="02690-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="02690-114">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="02690-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="02690-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="02690-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="02690-116">Reports.Read.All</span></span>                         |
| <span data-ttu-id="02690-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="02690-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02690-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="02690-118">Not supported.</span></span>                           |
| <span data-ttu-id="02690-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="02690-119">Application</span></span>                            | <span data-ttu-id="02690-120">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="02690-120">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="02690-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="02690-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageAccountCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="02690-122">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="02690-122">Function parameters</span></span>

<span data-ttu-id="02690-123">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="02690-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="02690-124">Parameter</span><span class="sxs-lookup"><span data-stu-id="02690-124">Parameter</span></span> | <span data-ttu-id="02690-125">Typ</span><span class="sxs-lookup"><span data-stu-id="02690-125">Type</span></span>   | <span data-ttu-id="02690-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="02690-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="02690-127">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="02690-127">period</span></span>    | <span data-ttu-id="02690-128">string</span><span class="sxs-lookup"><span data-stu-id="02690-128">string</span></span> | <span data-ttu-id="02690-129">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="02690-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="02690-130">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="02690-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="02690-131">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="02690-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="02690-132">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="02690-132">Required.</span></span> |

<span data-ttu-id="02690-133">Diese Methode unterstützt die `$format` [OData-Abfragezeichenfolgen-Parameter](/graph/query-parameters) zum Anpassen der Antwort.</span><span class="sxs-lookup"><span data-stu-id="02690-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="02690-134">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="02690-134">The default output type is text/csv.</span></span> <span data-ttu-id="02690-135">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="02690-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="02690-136">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="02690-136">Request headers</span></span>

| <span data-ttu-id="02690-137">Name</span><span class="sxs-lookup"><span data-stu-id="02690-137">Name</span></span>          | <span data-ttu-id="02690-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="02690-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="02690-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="02690-139">Authorization</span></span> | <span data-ttu-id="02690-p107">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="02690-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="02690-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="02690-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="02690-143">CSV</span><span class="sxs-lookup"><span data-stu-id="02690-143">CSV</span></span>

<span data-ttu-id="02690-144">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="02690-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="02690-145">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="02690-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="02690-146">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="02690-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="02690-147">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="02690-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="02690-148">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="02690-148">Report Refresh Date</span></span>
- <span data-ttu-id="02690-149">Websitetyp</span><span class="sxs-lookup"><span data-stu-id="02690-149">Site Type</span></span>
- <span data-ttu-id="02690-150">Gesamt</span><span class="sxs-lookup"><span data-stu-id="02690-150">Total</span></span>
- <span data-ttu-id="02690-151">Aktiv</span><span class="sxs-lookup"><span data-stu-id="02690-151">Active</span></span>
- <span data-ttu-id="02690-152">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="02690-152">Report Date</span></span>
- <span data-ttu-id="02690-153">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="02690-153">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="02690-154">JSON</span><span class="sxs-lookup"><span data-stu-id="02690-154">JSON</span></span>

<span data-ttu-id="02690-155">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines **[OneDriveUsageAccountCounts](../resources/onedriveusageaccountcounts.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="02690-155">If successful, this method returns a `200 OK` response code and a **[oneDriveUsageAccountCounts](../resources/onedriveusageaccountcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02690-156">Beispiel</span><span class="sxs-lookup"><span data-stu-id="02690-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="02690-157">CSV</span><span class="sxs-lookup"><span data-stu-id="02690-157">CSV</span></span>

<span data-ttu-id="02690-158">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="02690-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="02690-159">Anforderung</span><span class="sxs-lookup"><span data-stu-id="02690-159">Request</span></span>

<span data-ttu-id="02690-160">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="02690-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountcounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="02690-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="02690-161">Response</span></span>

<span data-ttu-id="02690-162">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="02690-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="02690-163">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="02690-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="02690-164">JSON</span><span class="sxs-lookup"><span data-stu-id="02690-164">JSON</span></span>

<span data-ttu-id="02690-165">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="02690-165">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="02690-166">Anforderung</span><span class="sxs-lookup"><span data-stu-id="02690-166">Request</span></span>

<span data-ttu-id="02690-167">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="02690-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountcounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="02690-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="02690-168">Response</span></span>

<span data-ttu-id="02690-169">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="02690-169">The following is an example of the response.</span></span>

> <span data-ttu-id="02690-p109">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="02690-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
