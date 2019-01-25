---
title: 'reportRoot: getSharePointActivityUserCounts'
description: Rufen Sie die Anzahl der aktiven Benutzer ab. Ein Benutzer wird als aktiv betrachtet, wenn er innerhalb des angegebenen Zeitraums eine Dateiaktivität ausgeführt (speichern, synchronisieren, ändern oder freigeben) oder eine Seite besucht hat.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: e3c806c991375d140a07c1fa09e19493f9b41f5b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513438"
---
# <a name="reportroot-getsharepointactivityusercounts"></a><span data-ttu-id="94ff2-104">reportRoot: getSharePointActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="94ff2-104">reportRoot: getSharePointActivityUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94ff2-105">Rufen Sie die Anzahl der aktiven Benutzer ab.</span><span class="sxs-lookup"><span data-stu-id="94ff2-105">Get the trend in the number of active users.</span></span> <span data-ttu-id="94ff2-106">Ein Benutzer wird als aktiv betrachtet, wenn er innerhalb des angegebenen Zeitraums eine Dateiaktivität ausgeführt (speichern, synchronisieren, ändern oder freigeben) oder eine Seite besucht hat.</span><span class="sxs-lookup"><span data-stu-id="94ff2-106">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span>

> <span data-ttu-id="94ff2-107">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – SharePoint-Aktivität](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="94ff2-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="94ff2-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="94ff2-108">Permissions</span></span>

<span data-ttu-id="94ff2-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94ff2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="94ff2-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="94ff2-111">Permission type</span></span>                        | <span data-ttu-id="94ff2-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="94ff2-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="94ff2-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="94ff2-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="94ff2-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="94ff2-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="94ff2-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="94ff2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94ff2-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="94ff2-116">Not supported.</span></span>                           |
| <span data-ttu-id="94ff2-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="94ff2-117">Application</span></span>                            | <span data-ttu-id="94ff2-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="94ff2-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="94ff2-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="94ff2-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="94ff2-120">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="94ff2-120">Function parameters</span></span>

<span data-ttu-id="94ff2-121">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="94ff2-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="94ff2-122">Parameter</span><span class="sxs-lookup"><span data-stu-id="94ff2-122">Parameter</span></span> | <span data-ttu-id="94ff2-123">Typ</span><span class="sxs-lookup"><span data-stu-id="94ff2-123">Type</span></span>   | <span data-ttu-id="94ff2-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="94ff2-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="94ff2-125">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="94ff2-125">period</span></span>    | <span data-ttu-id="94ff2-126">string</span><span class="sxs-lookup"><span data-stu-id="94ff2-126">string</span></span> | <span data-ttu-id="94ff2-127">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="94ff2-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="94ff2-128">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="94ff2-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="94ff2-129">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="94ff2-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="94ff2-130">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="94ff2-130">Required.</span></span> |

<span data-ttu-id="94ff2-131">Diese Methode unterstützt die `$format` [OData-Abfragezeichenfolgen-Parameter](/graph/query-parameters) zum Anpassen der Antwort.</span><span class="sxs-lookup"><span data-stu-id="94ff2-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="94ff2-132">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="94ff2-132">The default output type is text/csv.</span></span> <span data-ttu-id="94ff2-133">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="94ff2-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="94ff2-134">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="94ff2-134">Request headers</span></span>

| <span data-ttu-id="94ff2-135">Name</span><span class="sxs-lookup"><span data-stu-id="94ff2-135">Name</span></span>          | <span data-ttu-id="94ff2-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="94ff2-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="94ff2-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="94ff2-137">Authorization</span></span> | <span data-ttu-id="94ff2-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="94ff2-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="94ff2-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="94ff2-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="94ff2-141">CSV</span><span class="sxs-lookup"><span data-stu-id="94ff2-141">CSV</span></span>

<span data-ttu-id="94ff2-142">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="94ff2-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="94ff2-143">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="94ff2-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="94ff2-144">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="94ff2-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="94ff2-145">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="94ff2-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="94ff2-146">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="94ff2-146">Report Refresh Date</span></span>
- <span data-ttu-id="94ff2-147">Besuchte Seite</span><span class="sxs-lookup"><span data-stu-id="94ff2-147">Visited Page</span></span>
- <span data-ttu-id="94ff2-148">Angezeigt oder Bearbeitet</span><span class="sxs-lookup"><span data-stu-id="94ff2-148">Viewed Or Edited</span></span>
- <span data-ttu-id="94ff2-149">Synchronisiert</span><span class="sxs-lookup"><span data-stu-id="94ff2-149">Synced</span></span>
- <span data-ttu-id="94ff2-150">Intern freigegeben</span><span class="sxs-lookup"><span data-stu-id="94ff2-150">Shared Internally</span></span>
- <span data-ttu-id="94ff2-151">Extern freigegeben</span><span class="sxs-lookup"><span data-stu-id="94ff2-151">Shared Externally</span></span>
- <span data-ttu-id="94ff2-152">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="94ff2-152">Report Date</span></span>
- <span data-ttu-id="94ff2-153">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="94ff2-153">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="94ff2-154">JSON</span><span class="sxs-lookup"><span data-stu-id="94ff2-154">JSON</span></span>

<span data-ttu-id="94ff2-155">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines **[SharePointActivityUserCounts](../resources/sharepointactivityusercounts.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="94ff2-155">If successful, this method returns a `200 OK` response code and a **[sharePointActivityUserCounts](../resources/sharepointactivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94ff2-156">Beispiel</span><span class="sxs-lookup"><span data-stu-id="94ff2-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="94ff2-157">CSV</span><span class="sxs-lookup"><span data-stu-id="94ff2-157">CSV</span></span>

<span data-ttu-id="94ff2-158">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="94ff2-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="94ff2-159">Anforderung</span><span class="sxs-lookup"><span data-stu-id="94ff2-159">Request</span></span>

<span data-ttu-id="94ff2-160">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="94ff2-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="94ff2-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="94ff2-161">Response</span></span>

<span data-ttu-id="94ff2-162">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="94ff2-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="94ff2-163">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="94ff2-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Visited Page,Viewed Or Edited,Synced,Shared Internally,Shared Externally,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="94ff2-164">JSON</span><span class="sxs-lookup"><span data-stu-id="94ff2-164">JSON</span></span>

<span data-ttu-id="94ff2-165">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="94ff2-165">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="94ff2-166">Anforderung</span><span class="sxs-lookup"><span data-stu-id="94ff2-166">Request</span></span>

<span data-ttu-id="94ff2-167">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="94ff2-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="94ff2-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="94ff2-168">Response</span></span>

<span data-ttu-id="94ff2-169">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="94ff2-169">The following is an example of the response.</span></span>

> <span data-ttu-id="94ff2-p108">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="94ff2-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharePointActivityUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 302

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.sharePointActivityUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "visitedPage": 56, 
      "viewedOrEdited": 163, 
      "synced": 7, 
      "sharedInternally": 10, 
      "sharedExternally": 1, 
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
    "Error: /api-reference/beta/api/reportroot-getsharepointactivityusercounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
