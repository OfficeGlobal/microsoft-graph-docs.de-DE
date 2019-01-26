---
title: 'reportRoot: getTeamsUserActivityCounts'
description: Diese Methode ruft die Anzahl von Microsoft Teams-Aktivitäten nach Aktivitätstyp ab. Die Aktivitätstypen sind Chatnachricht, private Chatnachricht, Anruf und Besprechung.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: eadd1904aa198e14a796e3d0af79f68f1a2355af
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577403"
---
# <a name="reportroot-getteamsuseractivitycounts"></a><span data-ttu-id="efef5-104">reportRoot: getTeamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="efef5-104">reportRoot: getTeamsUserActivityCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="efef5-105">Diese Methode ruft die Anzahl von Microsoft Teams-Aktivitäten nach Aktivitätstyp ab.</span><span class="sxs-lookup"><span data-stu-id="efef5-105">Get the number of Microsoft Teams activities by activity type.</span></span> <span data-ttu-id="efef5-106">Die Aktivitätstypen sind Chatnachricht, private Chatnachricht, Anruf und Besprechung.</span><span class="sxs-lookup"><span data-stu-id="efef5-106">The activity types are team chat messages, private chat messages, calls, and meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="efef5-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="efef5-107">Permissions</span></span>

<span data-ttu-id="efef5-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="efef5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="efef5-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="efef5-110">Permission type</span></span>                        | <span data-ttu-id="efef5-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="efef5-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="efef5-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="efef5-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="efef5-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="efef5-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="efef5-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="efef5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="efef5-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="efef5-115">Not supported.</span></span>                           |
| <span data-ttu-id="efef5-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="efef5-116">Application</span></span>                            | <span data-ttu-id="efef5-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="efef5-117">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="efef5-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="efef5-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="efef5-119">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="efef5-119">Function parameters</span></span>

<span data-ttu-id="efef5-120">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="efef5-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="efef5-121">Parameter</span><span class="sxs-lookup"><span data-stu-id="efef5-121">Parameter</span></span> | <span data-ttu-id="efef5-122">Typ</span><span class="sxs-lookup"><span data-stu-id="efef5-122">Type</span></span>   | <span data-ttu-id="efef5-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="efef5-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="efef5-124">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="efef5-124">period</span></span>    | <span data-ttu-id="efef5-125">string</span><span class="sxs-lookup"><span data-stu-id="efef5-125">string</span></span> | <span data-ttu-id="efef5-126">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="efef5-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="efef5-127">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="efef5-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="efef5-128">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="efef5-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="efef5-129">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="efef5-129">Required.</span></span> |

<span data-ttu-id="efef5-130">Diese Methode unterstützt die `$format` [OData-Abfragezeichenfolgen-Parameter](/graph/query-parameters) zum Anpassen der Antwort.</span><span class="sxs-lookup"><span data-stu-id="efef5-130">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="efef5-131">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="efef5-131">The default output type is text/csv.</span></span> <span data-ttu-id="efef5-132">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="efef5-132">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="efef5-133">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="efef5-133">Request headers</span></span>

| <span data-ttu-id="efef5-134">Name</span><span class="sxs-lookup"><span data-stu-id="efef5-134">Name</span></span>          | <span data-ttu-id="efef5-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="efef5-135">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="efef5-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="efef5-136">Authorization</span></span> | <span data-ttu-id="efef5-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="efef5-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="efef5-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="efef5-139">Response</span></span>

### <a name="csv"></a><span data-ttu-id="efef5-140">CSV</span><span class="sxs-lookup"><span data-stu-id="efef5-140">CSV</span></span>

<span data-ttu-id="efef5-141">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="efef5-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="efef5-142">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="efef5-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="efef5-143">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="efef5-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="efef5-144">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="efef5-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="efef5-145">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="efef5-145">Report Refresh Date</span></span>
- <span data-ttu-id="efef5-146">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="efef5-146">Report Date</span></span>
- <span data-ttu-id="efef5-147">Team-Chatnachrichten</span><span class="sxs-lookup"><span data-stu-id="efef5-147">Team Chat Messages</span></span>
- <span data-ttu-id="efef5-148">Private Chatnachrichten</span><span class="sxs-lookup"><span data-stu-id="efef5-148">Private Chat Messages</span></span>
- <span data-ttu-id="efef5-149">Anrufe</span><span class="sxs-lookup"><span data-stu-id="efef5-149">Calls</span></span>
- <span data-ttu-id="efef5-150">Meetings</span><span class="sxs-lookup"><span data-stu-id="efef5-150">Meetings</span></span>
- <span data-ttu-id="efef5-151">Report Period</span><span class="sxs-lookup"><span data-stu-id="efef5-151">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="efef5-152">JSON</span><span class="sxs-lookup"><span data-stu-id="efef5-152">JSON</span></span>

<span data-ttu-id="efef5-153">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines **[TeamsUserActivityCounts](../resources/teamsuseractivitycounts.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="efef5-153">If successful, this method returns a `200 OK` response code and a **[teamsUserActivityCounts](../resources/teamsuseractivitycounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="efef5-154">Beispiel</span><span class="sxs-lookup"><span data-stu-id="efef5-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="efef5-155">CSV</span><span class="sxs-lookup"><span data-stu-id="efef5-155">CSV</span></span>

<span data-ttu-id="efef5-156">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="efef5-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="efef5-157">Anforderung</span><span class="sxs-lookup"><span data-stu-id="efef5-157">Request</span></span>

<span data-ttu-id="efef5-158">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="efef5-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="efef5-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="efef5-159">Response</span></span>

<span data-ttu-id="efef5-160">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="efef5-160">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
<span data-ttu-id="efef5-161">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="efef5-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Team Chat Messages,Private Chat Messages,Calls,Meetings,Report Period
```

### <a name="json"></a><span data-ttu-id="efef5-162">JSON</span><span class="sxs-lookup"><span data-stu-id="efef5-162">JSON</span></span>

<span data-ttu-id="efef5-163">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="efef5-163">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="efef5-164">Anforderung</span><span class="sxs-lookup"><span data-stu-id="efef5-164">Request</span></span>

<span data-ttu-id="efef5-165">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="efef5-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="efef5-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="efef5-166">Response</span></span>

<span data-ttu-id="efef5-167">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="efef5-167">The following is an example of the response.</span></span>

> <span data-ttu-id="efef5-p108">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="efef5-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsUserActivityCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 277

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsUserActivityCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "reportDate": "2017-09-01", 
      "teamChatMessages": 26, 
      "privateChatMessages": 17, 
      "calls": 4, 
      "meetings": 0, 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getteamsuseractivitycounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
