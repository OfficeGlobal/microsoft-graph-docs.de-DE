---
title: 'reportRoot: getSharePointActivityUserCounts'
description: Rufen Sie die Anzahl der aktiven Benutzer ab. Ein Benutzer wird als aktiv betrachtet, wenn er innerhalb des angegebenen Zeitraums eine Dateiaktivität ausgeführt (speichern, synchronisieren, ändern oder freigeben) oder eine Seite besucht hat.
localization_priority: Normal
ms.openlocfilehash: 356f079a1d0836b6cd824a30d6882ed12f0155fd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842203"
---
# <a name="reportroot-getsharepointactivityusercounts"></a><span data-ttu-id="a2cbe-104">reportRoot: getSharePointActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="a2cbe-104">reportRoot: getSharePointActivityUserCounts</span></span>

> <span data-ttu-id="a2cbe-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a2cbe-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a2cbe-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a2cbe-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a2cbe-107">Rufen Sie die Anzahl der aktiven Benutzer ab.</span><span class="sxs-lookup"><span data-stu-id="a2cbe-107">Get the trend in the number of active users.</span></span> <span data-ttu-id="a2cbe-108">Ein Benutzer wird als aktiv betrachtet, wenn er innerhalb des angegebenen Zeitraums eine Dateiaktivität ausgeführt (speichern, synchronisieren, ändern oder freigeben) oder eine Seite besucht hat.</span><span class="sxs-lookup"><span data-stu-id="a2cbe-108">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span>

> <span data-ttu-id="a2cbe-109">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – SharePoint-Aktivität](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="a2cbe-109">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="a2cbe-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a2cbe-110">Permissions</span></span>

<span data-ttu-id="a2cbe-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2cbe-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a2cbe-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a2cbe-113">Permission type</span></span>                        | <span data-ttu-id="a2cbe-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a2cbe-114">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="a2cbe-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a2cbe-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="a2cbe-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a2cbe-116">Reports.Read.All</span></span>                         |
| <span data-ttu-id="a2cbe-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a2cbe-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2cbe-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a2cbe-118">Not supported.</span></span>                           |
| <span data-ttu-id="a2cbe-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a2cbe-119">Application</span></span>                            | <span data-ttu-id="a2cbe-120">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a2cbe-120">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="a2cbe-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a2cbe-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="a2cbe-122">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="a2cbe-122">Function parameters</span></span>

<span data-ttu-id="a2cbe-123">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="a2cbe-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="a2cbe-124">Parameter</span><span class="sxs-lookup"><span data-stu-id="a2cbe-124">Parameter</span></span> | <span data-ttu-id="a2cbe-125">Typ</span><span class="sxs-lookup"><span data-stu-id="a2cbe-125">Type</span></span>   | <span data-ttu-id="a2cbe-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a2cbe-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="a2cbe-127">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="a2cbe-127">period</span></span>    | <span data-ttu-id="a2cbe-128">string</span><span class="sxs-lookup"><span data-stu-id="a2cbe-128">string</span></span> | <span data-ttu-id="a2cbe-129">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="a2cbe-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="a2cbe-130">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="a2cbe-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="a2cbe-131">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="a2cbe-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="a2cbe-132">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="a2cbe-132">Required.</span></span> |

<span data-ttu-id="a2cbe-133">Diese Methode unterstützt die `$format` [OData-Abfragezeichenfolgen-Parameter](/graph/query-parameters) zum Anpassen der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a2cbe-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="a2cbe-134">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="a2cbe-134">The default output type is text/csv.</span></span> <span data-ttu-id="a2cbe-135">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="a2cbe-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a2cbe-136">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a2cbe-136">Request headers</span></span>

| <span data-ttu-id="a2cbe-137">Name</span><span class="sxs-lookup"><span data-stu-id="a2cbe-137">Name</span></span>          | <span data-ttu-id="a2cbe-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a2cbe-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="a2cbe-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2cbe-139">Authorization</span></span> | <span data-ttu-id="a2cbe-p107">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a2cbe-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="a2cbe-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="a2cbe-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="a2cbe-143">CSV</span><span class="sxs-lookup"><span data-stu-id="a2cbe-143">CSV</span></span>

<span data-ttu-id="a2cbe-144">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="a2cbe-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="a2cbe-145">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a2cbe-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="a2cbe-146">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="a2cbe-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="a2cbe-147">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="a2cbe-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="a2cbe-148">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="a2cbe-148">Report Refresh Date</span></span>
- <span data-ttu-id="a2cbe-149">Besuchte Seite</span><span class="sxs-lookup"><span data-stu-id="a2cbe-149">Visited Page</span></span>
- <span data-ttu-id="a2cbe-150">Angezeigt oder Bearbeitet</span><span class="sxs-lookup"><span data-stu-id="a2cbe-150">Viewed Or Edited</span></span>
- <span data-ttu-id="a2cbe-151">Synchronisiert</span><span class="sxs-lookup"><span data-stu-id="a2cbe-151">Synced</span></span>
- <span data-ttu-id="a2cbe-152">Intern freigegeben</span><span class="sxs-lookup"><span data-stu-id="a2cbe-152">Shared Internally</span></span>
- <span data-ttu-id="a2cbe-153">Extern freigegeben</span><span class="sxs-lookup"><span data-stu-id="a2cbe-153">Shared Externally</span></span>
- <span data-ttu-id="a2cbe-154">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="a2cbe-154">Report Date</span></span>
- <span data-ttu-id="a2cbe-155">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="a2cbe-155">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="a2cbe-156">JSON</span><span class="sxs-lookup"><span data-stu-id="a2cbe-156">JSON</span></span>

<span data-ttu-id="a2cbe-157">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines **[SharePointActivityUserCounts](../resources/sharepointactivityusercounts.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="a2cbe-157">If successful, this method returns a `200 OK` response code and a **[sharePointActivityUserCounts](../resources/sharepointactivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2cbe-158">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a2cbe-158">Example</span></span>

### <a name="csv"></a><span data-ttu-id="a2cbe-159">CSV</span><span class="sxs-lookup"><span data-stu-id="a2cbe-159">CSV</span></span>

<span data-ttu-id="a2cbe-160">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="a2cbe-160">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="a2cbe-161">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a2cbe-161">Request</span></span>

<span data-ttu-id="a2cbe-162">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a2cbe-162">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="a2cbe-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="a2cbe-163">Response</span></span>

<span data-ttu-id="a2cbe-164">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a2cbe-164">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="a2cbe-165">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="a2cbe-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="a2cbe-166">JSON</span><span class="sxs-lookup"><span data-stu-id="a2cbe-166">JSON</span></span>

<span data-ttu-id="a2cbe-167">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a2cbe-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="a2cbe-168">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a2cbe-168">Request</span></span>

<span data-ttu-id="a2cbe-169">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a2cbe-169">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="a2cbe-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="a2cbe-170">Response</span></span>

<span data-ttu-id="a2cbe-171">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a2cbe-171">The following is an example of the response.</span></span>

> <span data-ttu-id="a2cbe-p109">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="a2cbe-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
