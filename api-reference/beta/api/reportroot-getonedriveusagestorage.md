---
title: 'reportRoot: getOneDriveUsageStorage'
description: Verschaffen Sie sich einen Überblick über die Menge an Speicherplatz, die Sie in OneDrive for Business verwenden.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 4274740947e9160817cf874f9d2105b24d71de86
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510015"
---
# <a name="reportroot-getonedriveusagestorage"></a><span data-ttu-id="59de6-103">reportRoot: getOneDriveUsageStorage</span><span class="sxs-lookup"><span data-stu-id="59de6-103">reportRoot: getOneDriveUsageStorage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59de6-104">Verschaffen Sie sich einen Überblick über die Menge an Speicherplatz, die Sie in OneDrive for Business verwenden.</span><span class="sxs-lookup"><span data-stu-id="59de6-104">Get the trend on the amount of storage you are using in OneDrive for Business.</span></span>

> <span data-ttu-id="59de6-105">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – OneDrive for Business-Nutzung](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span><span class="sxs-lookup"><span data-stu-id="59de6-105">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="59de6-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="59de6-106">Permissions</span></span>

<span data-ttu-id="59de6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59de6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="59de6-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="59de6-109">Permission type</span></span>                        | <span data-ttu-id="59de6-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="59de6-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="59de6-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="59de6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="59de6-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="59de6-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="59de6-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="59de6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59de6-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="59de6-114">Not supported.</span></span>                           |
| <span data-ttu-id="59de6-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="59de6-115">Application</span></span>                            | <span data-ttu-id="59de6-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="59de6-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="59de6-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="59de6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageStorage(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="59de6-118">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="59de6-118">Function parameters</span></span>

<span data-ttu-id="59de6-119">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="59de6-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="59de6-120">Parameter</span><span class="sxs-lookup"><span data-stu-id="59de6-120">Parameter</span></span> | <span data-ttu-id="59de6-121">Typ</span><span class="sxs-lookup"><span data-stu-id="59de6-121">Type</span></span>   | <span data-ttu-id="59de6-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="59de6-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="59de6-123">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="59de6-123">period</span></span>    | <span data-ttu-id="59de6-124">string</span><span class="sxs-lookup"><span data-stu-id="59de6-124">string</span></span> | <span data-ttu-id="59de6-125">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="59de6-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="59de6-126">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="59de6-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="59de6-127">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="59de6-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="59de6-128">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="59de6-128">Required.</span></span> |

<span data-ttu-id="59de6-129">Diese Methode unterstützt die `$format` [OData-Abfragezeichenfolgen-Parameter](/graph/query-parameters) zum Anpassen der Antwort.</span><span class="sxs-lookup"><span data-stu-id="59de6-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="59de6-130">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="59de6-130">The default output type is text/csv.</span></span> <span data-ttu-id="59de6-131">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="59de6-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="59de6-132">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="59de6-132">Request headers</span></span>

| <span data-ttu-id="59de6-133">Name</span><span class="sxs-lookup"><span data-stu-id="59de6-133">Name</span></span>          | <span data-ttu-id="59de6-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="59de6-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="59de6-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="59de6-135">Authorization</span></span> | <span data-ttu-id="59de6-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="59de6-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="59de6-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="59de6-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="59de6-139">CSV</span><span class="sxs-lookup"><span data-stu-id="59de6-139">CSV</span></span>

<span data-ttu-id="59de6-140">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="59de6-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="59de6-141">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="59de6-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="59de6-142">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="59de6-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="59de6-143">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="59de6-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="59de6-144">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="59de6-144">Report Refresh Date</span></span>
- <span data-ttu-id="59de6-145">Websitetyp</span><span class="sxs-lookup"><span data-stu-id="59de6-145">Site Type</span></span>
- <span data-ttu-id="59de6-146">Verwendeter Speicherplatz (Byte)</span><span class="sxs-lookup"><span data-stu-id="59de6-146">Storage Used (Byte)</span></span>
- <span data-ttu-id="59de6-147">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="59de6-147">Report Date</span></span>
- <span data-ttu-id="59de6-148">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="59de6-148">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="59de6-149">JSON</span><span class="sxs-lookup"><span data-stu-id="59de6-149">JSON</span></span>

<span data-ttu-id="59de6-150">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines **[SiteUsageStorage](../resources/siteusagestorage.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="59de6-150">If successful, this method returns a `200 OK` response code and a **[siteUsageStorage](../resources/siteusagestorage.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59de6-151">Beispiel</span><span class="sxs-lookup"><span data-stu-id="59de6-151">Example</span></span>

### <a name="csv"></a><span data-ttu-id="59de6-152">CSV</span><span class="sxs-lookup"><span data-stu-id="59de6-152">CSV</span></span>

<span data-ttu-id="59de6-153">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="59de6-153">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="59de6-154">Anforderung</span><span class="sxs-lookup"><span data-stu-id="59de6-154">Request</span></span>

<span data-ttu-id="59de6-155">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="59de6-155">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusagestorage_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageStorage(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="59de6-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="59de6-156">Response</span></span>

<span data-ttu-id="59de6-157">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="59de6-157">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="59de6-158">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="59de6-158">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Storage Used (Byte),Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="59de6-159">JSON</span><span class="sxs-lookup"><span data-stu-id="59de6-159">JSON</span></span>

<span data-ttu-id="59de6-160">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="59de6-160">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="59de6-161">Anforderung</span><span class="sxs-lookup"><span data-stu-id="59de6-161">Request</span></span>

<span data-ttu-id="59de6-162">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="59de6-162">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusagestorage_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageStorage(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="59de6-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="59de6-163">Response</span></span>

<span data-ttu-id="59de6-164">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="59de6-164">The following is an example of the response.</span></span>

> <span data-ttu-id="59de6-p106">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="59de6-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.siteUsageStorage"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 248

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.siteUsageStorage)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteType": "All", 
      "storageUsedInBytes": 132654293197, 
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
    "Error: /api-reference/beta/api/reportroot-getonedriveusagestorage.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
