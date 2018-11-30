---
title: 'reportRoot: getSharePointSiteUsagePages'
description: Rufen Sie die Anzahl der angezeigten Seiten aller Websites ab.
ms.openlocfilehash: 7e6d620179e5b6d41b5076ae6e79917fd27ef4bb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065463"
---
# <a name="reportroot-getsharepointsiteusagepages"></a><span data-ttu-id="f9001-103">reportRoot: getSharePointSiteUsagePages</span><span class="sxs-lookup"><span data-stu-id="f9001-103">reportRoot: getSharePointSiteUsagePages</span></span>

> <span data-ttu-id="f9001-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f9001-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f9001-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f9001-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f9001-106">Rufen Sie die Anzahl der angezeigten Seiten aller Websites ab.</span><span class="sxs-lookup"><span data-stu-id="f9001-106">Get the number of pages viewed across all sites.</span></span>

> <span data-ttu-id="f9001-107">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – SharePoint-Websiteverwendung](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span><span class="sxs-lookup"><span data-stu-id="f9001-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="f9001-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f9001-108">Permissions</span></span>

<span data-ttu-id="f9001-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9001-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f9001-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f9001-111">Permission type</span></span>                        | <span data-ttu-id="f9001-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f9001-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="f9001-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f9001-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="f9001-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f9001-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="f9001-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f9001-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9001-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f9001-116">Not supported.</span></span>                           |
| <span data-ttu-id="f9001-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f9001-117">Application</span></span>                            | <span data-ttu-id="f9001-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f9001-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="f9001-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f9001-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsagePages(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="f9001-120">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="f9001-120">Function parameters</span></span>

<span data-ttu-id="f9001-121">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="f9001-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="f9001-122">Parameter</span><span class="sxs-lookup"><span data-stu-id="f9001-122">Parameter</span></span> | <span data-ttu-id="f9001-123">Typ</span><span class="sxs-lookup"><span data-stu-id="f9001-123">Type</span></span>   | <span data-ttu-id="f9001-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f9001-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="f9001-125">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="f9001-125">period</span></span>    | <span data-ttu-id="f9001-126">string</span><span class="sxs-lookup"><span data-stu-id="f9001-126">string</span></span> | <span data-ttu-id="f9001-127">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="f9001-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="f9001-128">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="f9001-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="f9001-129">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="f9001-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="f9001-130">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="f9001-130">Required.</span></span> |

<span data-ttu-id="f9001-131">Diese Methode unterstützt die `$format` [OData-Abfragezeichenfolgen-Parameter](/graph/query-parameters) zum Anpassen der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f9001-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="f9001-132">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="f9001-132">The default output type is text/csv.</span></span> <span data-ttu-id="f9001-133">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="f9001-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f9001-134">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f9001-134">Request headers</span></span>

| <span data-ttu-id="f9001-135">Name</span><span class="sxs-lookup"><span data-stu-id="f9001-135">Name</span></span>          | <span data-ttu-id="f9001-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f9001-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="f9001-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9001-137">Authorization</span></span> | <span data-ttu-id="f9001-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f9001-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="f9001-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="f9001-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="f9001-141">CSV</span><span class="sxs-lookup"><span data-stu-id="f9001-141">CSV</span></span>

<span data-ttu-id="f9001-142">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="f9001-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="f9001-143">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f9001-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="f9001-144">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="f9001-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="f9001-145">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="f9001-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="f9001-146">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="f9001-146">Report Refresh Date</span></span>
- <span data-ttu-id="f9001-147">Websitetyp</span><span class="sxs-lookup"><span data-stu-id="f9001-147">Site Type</span></span>
- <span data-ttu-id="f9001-148">Anzahl der angezeigten Seiten</span><span class="sxs-lookup"><span data-stu-id="f9001-148">Page View Count</span></span>
- <span data-ttu-id="f9001-149">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="f9001-149">Report Date</span></span>
- <span data-ttu-id="f9001-150">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="f9001-150">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="f9001-151">JSON</span><span class="sxs-lookup"><span data-stu-id="f9001-151">JSON</span></span>

<span data-ttu-id="f9001-152">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines **[SharePointSiteUsagePages](../resources/sharepointsiteusagepages.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="f9001-152">If successful, this method returns a `200 OK` response code and a **[sharePointSiteUsagePages](../resources/sharepointsiteusagepages.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9001-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f9001-153">Example</span></span>

### <a name="csv"></a><span data-ttu-id="f9001-154">CSV</span><span class="sxs-lookup"><span data-stu-id="f9001-154">CSV</span></span>

<span data-ttu-id="f9001-155">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="f9001-155">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="f9001-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f9001-156">Request</span></span>

<span data-ttu-id="f9001-157">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f9001-157">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagepages_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsagePages(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="f9001-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="f9001-158">Response</span></span>

<span data-ttu-id="f9001-159">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f9001-159">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="f9001-160">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="f9001-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="f9001-161">JSON</span><span class="sxs-lookup"><span data-stu-id="f9001-161">JSON</span></span>

<span data-ttu-id="f9001-162">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f9001-162">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="f9001-163">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f9001-163">Request</span></span>

<span data-ttu-id="f9001-164">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f9001-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagepages_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsagePages(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="f9001-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="f9001-165">Response</span></span>

<span data-ttu-id="f9001-166">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f9001-166">The following is an example of the response.</span></span>

> <span data-ttu-id="f9001-p107">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="f9001-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
