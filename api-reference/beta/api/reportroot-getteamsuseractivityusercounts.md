---
title: 'reportRoot: getTeamsUserActivityUserCounts'
description: Diese Methode ruft die Anzahl von Microsoft Teams-Benutzern nach Aktivitätstyp ab. Die Aktivitätstypen geben die Anzahl von Chatnachrichten, privaten Chatnachrichten, Anrufen oder Besprechungen der Teams an.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 1cc651d1237ca9455ff6f6ab402ba3c6332f9873
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27975862"
---
# <a name="reportroot-getteamsuseractivityusercounts"></a><span data-ttu-id="7c3e7-104">reportRoot: getTeamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="7c3e7-104">reportRoot: getTeamsUserActivityUserCounts</span></span>

> <span data-ttu-id="7c3e7-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7c3e7-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7c3e7-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7c3e7-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7c3e7-107">Diese Methode ruft die Anzahl von Microsoft Teams-Benutzern nach Aktivitätstyp ab.</span><span class="sxs-lookup"><span data-stu-id="7c3e7-107">Get the number of Microsoft Teams users by activity type.</span></span> <span data-ttu-id="7c3e7-108">Die Aktivitätstypen geben die Anzahl von Chatnachrichten, privaten Chatnachrichten, Anrufen oder Besprechungen der Teams an.</span><span class="sxs-lookup"><span data-stu-id="7c3e7-108">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="7c3e7-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7c3e7-109">Permissions</span></span>

<span data-ttu-id="7c3e7-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c3e7-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7c3e7-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7c3e7-112">Permission type</span></span>                        | <span data-ttu-id="7c3e7-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7c3e7-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="7c3e7-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7c3e7-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="7c3e7-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c3e7-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="7c3e7-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7c3e7-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c3e7-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7c3e7-117">Not supported.</span></span>                           |
| <span data-ttu-id="7c3e7-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7c3e7-118">Application</span></span>                            | <span data-ttu-id="7c3e7-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c3e7-119">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="7c3e7-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7c3e7-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="7c3e7-121">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="7c3e7-121">Function parameters</span></span>

<span data-ttu-id="7c3e7-122">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="7c3e7-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="7c3e7-123">Parameter</span><span class="sxs-lookup"><span data-stu-id="7c3e7-123">Parameter</span></span> | <span data-ttu-id="7c3e7-124">Typ</span><span class="sxs-lookup"><span data-stu-id="7c3e7-124">Type</span></span>   | <span data-ttu-id="7c3e7-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7c3e7-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="7c3e7-126">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="7c3e7-126">period</span></span>    | <span data-ttu-id="7c3e7-127">string</span><span class="sxs-lookup"><span data-stu-id="7c3e7-127">string</span></span> | <span data-ttu-id="7c3e7-128">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="7c3e7-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="7c3e7-129">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="7c3e7-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="7c3e7-130">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="7c3e7-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="7c3e7-131">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="7c3e7-131">Required.</span></span> |

<span data-ttu-id="7c3e7-132">Diese Methode unterstützt die `$format` [OData-Abfragezeichenfolgen-Parameter](/graph/query-parameters) zum Anpassen der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7c3e7-132">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="7c3e7-133">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="7c3e7-133">The default output type is text/csv.</span></span> <span data-ttu-id="7c3e7-134">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="7c3e7-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7c3e7-135">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7c3e7-135">Request headers</span></span>

| <span data-ttu-id="7c3e7-136">Name</span><span class="sxs-lookup"><span data-stu-id="7c3e7-136">Name</span></span>          | <span data-ttu-id="7c3e7-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7c3e7-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="7c3e7-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c3e7-138">Authorization</span></span> | <span data-ttu-id="7c3e7-p107">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7c3e7-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="7c3e7-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="7c3e7-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="7c3e7-142">CSV</span><span class="sxs-lookup"><span data-stu-id="7c3e7-142">CSV</span></span>

<span data-ttu-id="7c3e7-143">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="7c3e7-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="7c3e7-144">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7c3e7-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="7c3e7-145">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="7c3e7-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="7c3e7-146">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="7c3e7-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="7c3e7-147">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="7c3e7-147">Report Refresh Date</span></span>
- <span data-ttu-id="7c3e7-148">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="7c3e7-148">Report Date</span></span>
- <span data-ttu-id="7c3e7-149">Team-Chatnachrichten</span><span class="sxs-lookup"><span data-stu-id="7c3e7-149">Team Chat Messages</span></span>
- <span data-ttu-id="7c3e7-150">Private Chatnachrichten</span><span class="sxs-lookup"><span data-stu-id="7c3e7-150">Private Chat Messages</span></span>
- <span data-ttu-id="7c3e7-151">Anrufe</span><span class="sxs-lookup"><span data-stu-id="7c3e7-151">Calls</span></span>
- <span data-ttu-id="7c3e7-152">Besprechungen</span><span class="sxs-lookup"><span data-stu-id="7c3e7-152">Meetings</span></span>
- <span data-ttu-id="7c3e7-153">Sonstige Aktionen</span><span class="sxs-lookup"><span data-stu-id="7c3e7-153">Other Actions</span></span>
- <span data-ttu-id="7c3e7-154">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="7c3e7-154">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="7c3e7-155">JSON</span><span class="sxs-lookup"><span data-stu-id="7c3e7-155">JSON</span></span>

<span data-ttu-id="7c3e7-156">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines **[TeamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="7c3e7-156">If successful, this method returns a `200 OK` response code and a **[teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c3e7-157">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7c3e7-157">Example</span></span>

### <a name="csv"></a><span data-ttu-id="7c3e7-158">CSV</span><span class="sxs-lookup"><span data-stu-id="7c3e7-158">CSV</span></span>

<span data-ttu-id="7c3e7-159">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="7c3e7-159">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="7c3e7-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7c3e7-160">Request</span></span>

<span data-ttu-id="7c3e7-161">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7c3e7-161">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="7c3e7-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="7c3e7-162">Response</span></span>

<span data-ttu-id="7c3e7-163">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7c3e7-163">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="7c3e7-164">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="7c3e7-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="7c3e7-165">JSON</span><span class="sxs-lookup"><span data-stu-id="7c3e7-165">JSON</span></span>

<span data-ttu-id="7c3e7-166">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7c3e7-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="7c3e7-167">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7c3e7-167">Request</span></span>

<span data-ttu-id="7c3e7-168">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7c3e7-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="7c3e7-169">Antwort</span><span class="sxs-lookup"><span data-stu-id="7c3e7-169">Response</span></span>

<span data-ttu-id="7c3e7-170">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7c3e7-170">The following is an example of the response.</span></span>

> <span data-ttu-id="7c3e7-p109">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="7c3e7-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
