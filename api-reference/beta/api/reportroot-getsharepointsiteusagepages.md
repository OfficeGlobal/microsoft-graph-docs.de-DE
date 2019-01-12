---
title: 'reportRoot: getSharePointSiteUsagePages'
description: Rufen Sie die Anzahl der angezeigten Seiten aller Websites ab.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 621e94340f4011780c81340c8f26864ce276607b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914920"
---
# <a name="reportroot-getsharepointsiteusagepages"></a><span data-ttu-id="0aefe-103">reportRoot: getSharePointSiteUsagePages</span><span class="sxs-lookup"><span data-stu-id="0aefe-103">reportRoot: getSharePointSiteUsagePages</span></span>

> <span data-ttu-id="0aefe-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0aefe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0aefe-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0aefe-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0aefe-106">Rufen Sie die Anzahl der angezeigten Seiten aller Websites ab.</span><span class="sxs-lookup"><span data-stu-id="0aefe-106">Get the number of pages viewed across all sites.</span></span>

> <span data-ttu-id="0aefe-107">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – SharePoint-Websiteverwendung](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span><span class="sxs-lookup"><span data-stu-id="0aefe-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="0aefe-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0aefe-108">Permissions</span></span>

<span data-ttu-id="0aefe-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0aefe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0aefe-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0aefe-111">Permission type</span></span>                        | <span data-ttu-id="0aefe-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0aefe-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="0aefe-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0aefe-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="0aefe-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0aefe-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="0aefe-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0aefe-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0aefe-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0aefe-116">Not supported.</span></span>                           |
| <span data-ttu-id="0aefe-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0aefe-117">Application</span></span>                            | <span data-ttu-id="0aefe-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0aefe-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="0aefe-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0aefe-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsagePages(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="0aefe-120">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="0aefe-120">Function parameters</span></span>

<span data-ttu-id="0aefe-121">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="0aefe-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="0aefe-122">Parameter</span><span class="sxs-lookup"><span data-stu-id="0aefe-122">Parameter</span></span> | <span data-ttu-id="0aefe-123">Typ</span><span class="sxs-lookup"><span data-stu-id="0aefe-123">Type</span></span>   | <span data-ttu-id="0aefe-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0aefe-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="0aefe-125">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="0aefe-125">period</span></span>    | <span data-ttu-id="0aefe-126">string</span><span class="sxs-lookup"><span data-stu-id="0aefe-126">string</span></span> | <span data-ttu-id="0aefe-127">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="0aefe-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="0aefe-128">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="0aefe-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="0aefe-129">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="0aefe-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="0aefe-130">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="0aefe-130">Required.</span></span> |

<span data-ttu-id="0aefe-131">Diese Methode unterstützt die `$format` [OData-Abfragezeichenfolgen-Parameter](/graph/query-parameters) zum Anpassen der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0aefe-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="0aefe-132">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="0aefe-132">The default output type is text/csv.</span></span> <span data-ttu-id="0aefe-133">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="0aefe-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0aefe-134">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0aefe-134">Request headers</span></span>

| <span data-ttu-id="0aefe-135">Name</span><span class="sxs-lookup"><span data-stu-id="0aefe-135">Name</span></span>          | <span data-ttu-id="0aefe-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0aefe-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="0aefe-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="0aefe-137">Authorization</span></span> | <span data-ttu-id="0aefe-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0aefe-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="0aefe-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="0aefe-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="0aefe-141">CSV</span><span class="sxs-lookup"><span data-stu-id="0aefe-141">CSV</span></span>

<span data-ttu-id="0aefe-142">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="0aefe-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="0aefe-143">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0aefe-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="0aefe-144">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="0aefe-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="0aefe-145">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="0aefe-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="0aefe-146">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="0aefe-146">Report Refresh Date</span></span>
- <span data-ttu-id="0aefe-147">Websitetyp</span><span class="sxs-lookup"><span data-stu-id="0aefe-147">Site Type</span></span>
- <span data-ttu-id="0aefe-148">Anzahl der angezeigten Seiten</span><span class="sxs-lookup"><span data-stu-id="0aefe-148">Page View Count</span></span>
- <span data-ttu-id="0aefe-149">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="0aefe-149">Report Date</span></span>
- <span data-ttu-id="0aefe-150">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="0aefe-150">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="0aefe-151">JSON</span><span class="sxs-lookup"><span data-stu-id="0aefe-151">JSON</span></span>

<span data-ttu-id="0aefe-152">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines **[SharePointSiteUsagePages](../resources/sharepointsiteusagepages.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="0aefe-152">If successful, this method returns a `200 OK` response code and a **[sharePointSiteUsagePages](../resources/sharepointsiteusagepages.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0aefe-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0aefe-153">Example</span></span>

### <a name="csv"></a><span data-ttu-id="0aefe-154">CSV</span><span class="sxs-lookup"><span data-stu-id="0aefe-154">CSV</span></span>

<span data-ttu-id="0aefe-155">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="0aefe-155">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="0aefe-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0aefe-156">Request</span></span>

<span data-ttu-id="0aefe-157">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0aefe-157">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagepages_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsagePages(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="0aefe-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="0aefe-158">Response</span></span>

<span data-ttu-id="0aefe-159">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0aefe-159">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="0aefe-160">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="0aefe-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Page View Count,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="0aefe-161">JSON</span><span class="sxs-lookup"><span data-stu-id="0aefe-161">JSON</span></span>

<span data-ttu-id="0aefe-162">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0aefe-162">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="0aefe-163">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0aefe-163">Request</span></span>

<span data-ttu-id="0aefe-164">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0aefe-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagepages_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsagePages(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="0aefe-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="0aefe-165">Response</span></span>

<span data-ttu-id="0aefe-166">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0aefe-166">The following is an example of the response.</span></span>

> <span data-ttu-id="0aefe-p107">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="0aefe-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharePointSiteUsagePages"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 243

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.sharePointSiteUsagePages)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteType": "All", 
      "pageViewCount": 183, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
