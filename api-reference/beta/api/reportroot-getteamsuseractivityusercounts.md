---
title: 'reportRoot: getTeamsUserActivityUserCounts'
description: Diese Methode ruft die Anzahl von Microsoft Teams-Benutzern nach Aktivitätstyp ab. Die Aktivitätstypen geben die Anzahl von Chatnachrichten, privaten Chatnachrichten, Anrufen oder Besprechungen der Teams an.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: f8ef35813b523a28c5f6a7b455b729c144b0f072
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577172"
---
# <a name="reportroot-getteamsuseractivityusercounts"></a><span data-ttu-id="f867c-104">reportRoot: getTeamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="f867c-104">reportRoot: getTeamsUserActivityUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f867c-105">Diese Methode ruft die Anzahl von Microsoft Teams-Benutzern nach Aktivitätstyp ab.</span><span class="sxs-lookup"><span data-stu-id="f867c-105">Get the number of Microsoft Teams users by activity type.</span></span> <span data-ttu-id="f867c-106">Die Aktivitätstypen geben die Anzahl von Chatnachrichten, privaten Chatnachrichten, Anrufen oder Besprechungen der Teams an.</span><span class="sxs-lookup"><span data-stu-id="f867c-106">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="f867c-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f867c-107">Permissions</span></span>

<span data-ttu-id="f867c-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f867c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f867c-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f867c-110">Permission type</span></span>                        | <span data-ttu-id="f867c-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f867c-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="f867c-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f867c-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="f867c-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f867c-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="f867c-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f867c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f867c-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f867c-115">Not supported.</span></span>                           |
| <span data-ttu-id="f867c-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f867c-116">Application</span></span>                            | <span data-ttu-id="f867c-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f867c-117">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="f867c-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f867c-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="f867c-119">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="f867c-119">Function parameters</span></span>

<span data-ttu-id="f867c-120">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="f867c-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="f867c-121">Parameter</span><span class="sxs-lookup"><span data-stu-id="f867c-121">Parameter</span></span> | <span data-ttu-id="f867c-122">Typ</span><span class="sxs-lookup"><span data-stu-id="f867c-122">Type</span></span>   | <span data-ttu-id="f867c-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f867c-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="f867c-124">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="f867c-124">period</span></span>    | <span data-ttu-id="f867c-125">string</span><span class="sxs-lookup"><span data-stu-id="f867c-125">string</span></span> | <span data-ttu-id="f867c-126">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="f867c-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="f867c-127">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="f867c-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="f867c-128">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="f867c-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="f867c-129">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="f867c-129">Required.</span></span> |

<span data-ttu-id="f867c-130">Diese Methode unterstützt die `$format` [OData-Abfragezeichenfolgen-Parameter](/graph/query-parameters) zum Anpassen der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f867c-130">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="f867c-131">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="f867c-131">The default output type is text/csv.</span></span> <span data-ttu-id="f867c-132">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="f867c-132">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f867c-133">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f867c-133">Request headers</span></span>

| <span data-ttu-id="f867c-134">Name</span><span class="sxs-lookup"><span data-stu-id="f867c-134">Name</span></span>          | <span data-ttu-id="f867c-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f867c-135">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="f867c-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="f867c-136">Authorization</span></span> | <span data-ttu-id="f867c-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f867c-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="f867c-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="f867c-139">Response</span></span>

### <a name="csv"></a><span data-ttu-id="f867c-140">CSV</span><span class="sxs-lookup"><span data-stu-id="f867c-140">CSV</span></span>

<span data-ttu-id="f867c-141">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="f867c-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="f867c-142">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f867c-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="f867c-143">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="f867c-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="f867c-144">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="f867c-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="f867c-145">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="f867c-145">Report Refresh Date</span></span>
- <span data-ttu-id="f867c-146">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="f867c-146">Report Date</span></span>
- <span data-ttu-id="f867c-147">Team-Chatnachrichten</span><span class="sxs-lookup"><span data-stu-id="f867c-147">Team Chat Messages</span></span>
- <span data-ttu-id="f867c-148">Private Chatnachrichten</span><span class="sxs-lookup"><span data-stu-id="f867c-148">Private Chat Messages</span></span>
- <span data-ttu-id="f867c-149">Anrufe</span><span class="sxs-lookup"><span data-stu-id="f867c-149">Calls</span></span>
- <span data-ttu-id="f867c-150">Besprechungen</span><span class="sxs-lookup"><span data-stu-id="f867c-150">Meetings</span></span>
- <span data-ttu-id="f867c-151">Sonstige Aktionen</span><span class="sxs-lookup"><span data-stu-id="f867c-151">Other Actions</span></span>
- <span data-ttu-id="f867c-152">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="f867c-152">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="f867c-153">JSON</span><span class="sxs-lookup"><span data-stu-id="f867c-153">JSON</span></span>

<span data-ttu-id="f867c-154">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines **[TeamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="f867c-154">If successful, this method returns a `200 OK` response code and a **[teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f867c-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f867c-155">Example</span></span>

### <a name="csv"></a><span data-ttu-id="f867c-156">CSV</span><span class="sxs-lookup"><span data-stu-id="f867c-156">CSV</span></span>

<span data-ttu-id="f867c-157">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="f867c-157">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="f867c-158">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f867c-158">Request</span></span>

<span data-ttu-id="f867c-159">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f867c-159">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="f867c-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="f867c-160">Response</span></span>

<span data-ttu-id="f867c-161">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f867c-161">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="f867c-162">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="f867c-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Team Chat Messages,Private Chat Messages,Calls,Meetings,Other Actions,Report Period
```

### <a name="json"></a><span data-ttu-id="f867c-163">JSON</span><span class="sxs-lookup"><span data-stu-id="f867c-163">JSON</span></span>

<span data-ttu-id="f867c-164">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f867c-164">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="f867c-165">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f867c-165">Request</span></span>

<span data-ttu-id="f867c-166">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f867c-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="f867c-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="f867c-167">Response</span></span>

<span data-ttu-id="f867c-168">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f867c-168">The following is an example of the response.</span></span>

> <span data-ttu-id="f867c-p108">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="f867c-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsUserActivityUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 291

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsUserActivityUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "reportDate": "2017-09-01", 
      "teamChatMessages": 30, 
      "privateChatMessages": 21, 
      "calls": 6, 
      "meetings": 2, 
      "otherActions": 17, 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getteamsuseractivityusercounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
