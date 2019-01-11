---
title: 'reportRoot: getTeamsUserActivityCounts'
description: Diese Methode ruft die Anzahl von Microsoft Teams-Aktivitäten nach Aktivitätstyp ab. Die Aktivitätstypen sind Chatnachricht, private Chatnachricht, Anruf und Besprechung.
localization_priority: Normal
ms.openlocfilehash: 34c059a262ba01b66b9e7ecc3489e4cfd5da0b5f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27857603"
---
# <a name="reportroot-getteamsuseractivitycounts"></a><span data-ttu-id="c5673-104">reportRoot: getTeamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="c5673-104">reportRoot: getTeamsUserActivityCounts</span></span>

> <span data-ttu-id="c5673-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c5673-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c5673-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c5673-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c5673-107">Diese Methode ruft die Anzahl von Microsoft Teams-Aktivitäten nach Aktivitätstyp ab.</span><span class="sxs-lookup"><span data-stu-id="c5673-107">Get the number of Microsoft Teams activities by activity type.</span></span> <span data-ttu-id="c5673-108">Die Aktivitätstypen sind Chatnachricht, private Chatnachricht, Anruf und Besprechung.</span><span class="sxs-lookup"><span data-stu-id="c5673-108">The activity types are team chat messages, private chat messages, calls, and meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="c5673-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c5673-109">Permissions</span></span>

<span data-ttu-id="c5673-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5673-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c5673-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c5673-112">Permission type</span></span>                        | <span data-ttu-id="c5673-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c5673-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="c5673-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c5673-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="c5673-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c5673-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="c5673-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c5673-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5673-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c5673-117">Not supported.</span></span>                           |
| <span data-ttu-id="c5673-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c5673-118">Application</span></span>                            | <span data-ttu-id="c5673-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c5673-119">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="c5673-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c5673-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="c5673-121">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="c5673-121">Function parameters</span></span>

<span data-ttu-id="c5673-122">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="c5673-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="c5673-123">Parameter</span><span class="sxs-lookup"><span data-stu-id="c5673-123">Parameter</span></span> | <span data-ttu-id="c5673-124">Typ</span><span class="sxs-lookup"><span data-stu-id="c5673-124">Type</span></span>   | <span data-ttu-id="c5673-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c5673-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="c5673-126">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="c5673-126">period</span></span>    | <span data-ttu-id="c5673-127">string</span><span class="sxs-lookup"><span data-stu-id="c5673-127">string</span></span> | <span data-ttu-id="c5673-128">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="c5673-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="c5673-129">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="c5673-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="c5673-130">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="c5673-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="c5673-131">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="c5673-131">Required.</span></span> |

<span data-ttu-id="c5673-132">Diese Methode unterstützt die `$format` [OData-Abfragezeichenfolgen-Parameter](/graph/query-parameters) zum Anpassen der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c5673-132">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="c5673-133">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="c5673-133">The default output type is text/csv.</span></span> <span data-ttu-id="c5673-134">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="c5673-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c5673-135">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c5673-135">Request headers</span></span>

| <span data-ttu-id="c5673-136">Name</span><span class="sxs-lookup"><span data-stu-id="c5673-136">Name</span></span>          | <span data-ttu-id="c5673-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c5673-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="c5673-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5673-138">Authorization</span></span> | <span data-ttu-id="c5673-p107">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c5673-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="c5673-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="c5673-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="c5673-142">CSV</span><span class="sxs-lookup"><span data-stu-id="c5673-142">CSV</span></span>

<span data-ttu-id="c5673-143">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="c5673-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="c5673-144">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c5673-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="c5673-145">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="c5673-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="c5673-146">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="c5673-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="c5673-147">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="c5673-147">Report Refresh Date</span></span>
- <span data-ttu-id="c5673-148">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="c5673-148">Report Date</span></span>
- <span data-ttu-id="c5673-149">Team-Chatnachrichten</span><span class="sxs-lookup"><span data-stu-id="c5673-149">Team Chat Messages</span></span>
- <span data-ttu-id="c5673-150">Private Chatnachrichten</span><span class="sxs-lookup"><span data-stu-id="c5673-150">Private Chat Messages</span></span>
- <span data-ttu-id="c5673-151">Anrufe</span><span class="sxs-lookup"><span data-stu-id="c5673-151">Calls</span></span>
- <span data-ttu-id="c5673-152">Meetings</span><span class="sxs-lookup"><span data-stu-id="c5673-152">Meetings</span></span>
- <span data-ttu-id="c5673-153">Report Period</span><span class="sxs-lookup"><span data-stu-id="c5673-153">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="c5673-154">JSON</span><span class="sxs-lookup"><span data-stu-id="c5673-154">JSON</span></span>

<span data-ttu-id="c5673-155">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines **[TeamsUserActivityCounts](../resources/teamsuseractivitycounts.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="c5673-155">If successful, this method returns a `200 OK` response code and a **[teamsUserActivityCounts](../resources/teamsuseractivitycounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5673-156">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c5673-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="c5673-157">CSV</span><span class="sxs-lookup"><span data-stu-id="c5673-157">CSV</span></span>

<span data-ttu-id="c5673-158">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="c5673-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="c5673-159">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c5673-159">Request</span></span>

<span data-ttu-id="c5673-160">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c5673-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="c5673-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="c5673-161">Response</span></span>

<span data-ttu-id="c5673-162">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c5673-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
<span data-ttu-id="c5673-163">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="c5673-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="c5673-164">JSON</span><span class="sxs-lookup"><span data-stu-id="c5673-164">JSON</span></span>

<span data-ttu-id="c5673-165">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c5673-165">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="c5673-166">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c5673-166">Request</span></span>

<span data-ttu-id="c5673-167">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c5673-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="c5673-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="c5673-168">Response</span></span>

<span data-ttu-id="c5673-169">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c5673-169">The following is an example of the response.</span></span>

> <span data-ttu-id="c5673-p109">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="c5673-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
