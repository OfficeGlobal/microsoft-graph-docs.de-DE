---
title: 'reportRoot: getSkypeForBusinessActivityUserDetail'
description: Rufen Sie Details der Skype for Business-Aktivität nach Benutzer ab.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 45b6eec0ac5d9d8523999fae763acb653bfd3a56
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575454"
---
# <a name="reportroot-getskypeforbusinessactivityuserdetail"></a><span data-ttu-id="70c44-103">reportRoot: getSkypeForBusinessActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="70c44-103">reportRoot: getSkypeForBusinessActivityUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70c44-104">Rufen Sie Details der Skype for Business-Aktivität nach Benutzer ab.</span><span class="sxs-lookup"><span data-stu-id="70c44-104">Get details about Skype for Business activity by user.</span></span>

> <span data-ttu-id="70c44-105">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Skype for Business-Aktivität](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span><span class="sxs-lookup"><span data-stu-id="70c44-105">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="permissions"></a><span data-ttu-id="70c44-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="70c44-106">Permissions</span></span>

<span data-ttu-id="70c44-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70c44-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="70c44-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="70c44-109">Permission type</span></span>                        | <span data-ttu-id="70c44-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="70c44-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="70c44-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="70c44-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="70c44-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="70c44-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="70c44-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="70c44-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70c44-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="70c44-114">Not supported.</span></span>                           |
| <span data-ttu-id="70c44-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="70c44-115">Application</span></span>                            | <span data-ttu-id="70c44-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="70c44-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="70c44-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="70c44-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessActivityUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="70c44-118">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="70c44-118">Function parameters</span></span>

<span data-ttu-id="70c44-119">Geben Sie in der Anforderungs-URL einen der folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="70c44-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="70c44-120">Parameter</span><span class="sxs-lookup"><span data-stu-id="70c44-120">Parameter</span></span> | <span data-ttu-id="70c44-121">Typ</span><span class="sxs-lookup"><span data-stu-id="70c44-121">Type</span></span>   | <span data-ttu-id="70c44-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="70c44-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="70c44-123">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="70c44-123">period</span></span>    | <span data-ttu-id="70c44-124">string</span><span class="sxs-lookup"><span data-stu-id="70c44-124">string</span></span> | <span data-ttu-id="70c44-125">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="70c44-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="70c44-126">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="70c44-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="70c44-127">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="70c44-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="70c44-128">date</span><span class="sxs-lookup"><span data-stu-id="70c44-128">date</span></span>      | <span data-ttu-id="70c44-129">Datum</span><span class="sxs-lookup"><span data-stu-id="70c44-129">Date</span></span>   | <span data-ttu-id="70c44-130">Gibt das Datum an, für das die Benutzer angezeigt werden sollen, die Aktivitäten durchgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="70c44-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="70c44-131">{date_value} muss im Format JJJJ-MM-TT vorliegen.</span><span class="sxs-lookup"><span data-stu-id="70c44-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="70c44-132">Da dieser Bericht nur für die letzten 30 Tage verfügbar ist, sollte {date_value} ein Datum aus diesem Zeitraum sein.</span><span class="sxs-lookup"><span data-stu-id="70c44-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="70c44-133">**Hinweis:** Sie müssen in der URL entweder einen Zeitraum oder ein Datum festlegen.</span><span class="sxs-lookup"><span data-stu-id="70c44-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="70c44-134">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) von  `$format`, `$top` und `$skipToken` zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="70c44-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="70c44-135">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="70c44-135">The default output type is text/csv.</span></span> <span data-ttu-id="70c44-136">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="70c44-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="70c44-137">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="70c44-137">Request headers</span></span>

| <span data-ttu-id="70c44-138">Name</span><span class="sxs-lookup"><span data-stu-id="70c44-138">Name</span></span>          | <span data-ttu-id="70c44-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="70c44-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="70c44-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="70c44-140">Authorization</span></span> | <span data-ttu-id="70c44-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="70c44-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="70c44-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="70c44-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="70c44-144">CSV</span><span class="sxs-lookup"><span data-stu-id="70c44-144">CSV</span></span>

<span data-ttu-id="70c44-145">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="70c44-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="70c44-146">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="70c44-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="70c44-147">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="70c44-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="70c44-148">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="70c44-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="70c44-149">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="70c44-149">Report Refresh Date</span></span>
- <span data-ttu-id="70c44-150">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="70c44-150">User Principal Name</span></span>
- <span data-ttu-id="70c44-151">Ist gelöscht</span><span class="sxs-lookup"><span data-stu-id="70c44-151">Is Deleted</span></span>
- <span data-ttu-id="70c44-152">Gelöscht am</span><span class="sxs-lookup"><span data-stu-id="70c44-152">Deleted Date</span></span>
- <span data-ttu-id="70c44-153">Datum der letzten Aktivität</span><span class="sxs-lookup"><span data-stu-id="70c44-153">Last Activity Date</span></span>
- <span data-ttu-id="70c44-154">Gesamtzahl Peer-to-Peer-Sitzung</span><span class="sxs-lookup"><span data-stu-id="70c44-154">Total Peer-to-peer Session Count</span></span>
- <span data-ttu-id="70c44-155">Gesamtzahl Organisierte Konferenz</span><span class="sxs-lookup"><span data-stu-id="70c44-155">Total Organized Conference Count</span></span>
- <span data-ttu-id="70c44-156">Gesamtzahl der teilgenommenen Konferenzen</span><span class="sxs-lookup"><span data-stu-id="70c44-156">Total Participated Conference Count</span></span>
- <span data-ttu-id="70c44-157">Datum der letzten Peer-to-Peer-Aktivität</span><span class="sxs-lookup"><span data-stu-id="70c44-157">Peer-to-peer Last Activity Date</span></span>
- <span data-ttu-id="70c44-158">Datum der letzten Aktivität der organisierten Konferenz</span><span class="sxs-lookup"><span data-stu-id="70c44-158">Organized Conference Last Activity Date</span></span>
- <span data-ttu-id="70c44-159">Datum der letzten Aktivität der teilgenommenen Konferenz</span><span class="sxs-lookup"><span data-stu-id="70c44-159">Participated Conference Last Activity Date</span></span>
- <span data-ttu-id="70c44-160">Anzahl Peer-to-Peer-Chat</span><span class="sxs-lookup"><span data-stu-id="70c44-160">Peer-to-peer IM Count</span></span>
- <span data-ttu-id="70c44-161">Anzahl Peer-to-Peer-Audio</span><span class="sxs-lookup"><span data-stu-id="70c44-161">Peer-to-peer Audio Count</span></span>
- <span data-ttu-id="70c44-162">Peer-to-Peer-Audiominuten</span><span class="sxs-lookup"><span data-stu-id="70c44-162">Peer-to-peer Audio Minutes</span></span>
- <span data-ttu-id="70c44-163">Anzahl Peer-to-Peer-Video</span><span class="sxs-lookup"><span data-stu-id="70c44-163">Peer-to-peer Video Count</span></span>
- <span data-ttu-id="70c44-164">Peer-to-Peer-Videominuten</span><span class="sxs-lookup"><span data-stu-id="70c44-164">Peer-to-peer Video Minutes</span></span>
- <span data-ttu-id="70c44-165">Anzahl Peer-to-Peer-App-Freigabe</span><span class="sxs-lookup"><span data-stu-id="70c44-165">Peer-to-peer App Sharing Count</span></span>
- <span data-ttu-id="70c44-166">Anzahl Peer-to-Peer-Dateiübertragung</span><span class="sxs-lookup"><span data-stu-id="70c44-166">Peer-to-peer File Transfer Count</span></span>
- <span data-ttu-id="70c44-167">Anzahl Organisierte Konferenz-Chat</span><span class="sxs-lookup"><span data-stu-id="70c44-167">Organized Conference IM Count</span></span>
- <span data-ttu-id="70c44-168">Anzahl Organisierte Konferenz-Audio/Video</span><span class="sxs-lookup"><span data-stu-id="70c44-168">Organized Conference Audio/Video Count</span></span>
- <span data-ttu-id="70c44-169">Anzahl Organisierte Konferenz-Audio-/Videominuten</span><span class="sxs-lookup"><span data-stu-id="70c44-169">Organized Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="70c44-170">Anzahl Organisierte Konferenz-App-Freigabe</span><span class="sxs-lookup"><span data-stu-id="70c44-170">Organized Conference App Sharing Count</span></span>
- <span data-ttu-id="70c44-171">Anzahl Organisierte Konferenz-Web</span><span class="sxs-lookup"><span data-stu-id="70c44-171">Organized Conference Web Count</span></span>
- <span data-ttu-id="70c44-172">Anzahl Organisierte Konferenz-Einwahl/Auswahl Drittanbieter</span><span class="sxs-lookup"><span data-stu-id="70c44-172">Organized Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="70c44-173">Anzahl Organisierte Konferenz-Einwahl/Auswahl Microsoft</span><span class="sxs-lookup"><span data-stu-id="70c44-173">Organized Conference Dial-in/out Microsoft Count</span></span>
- <span data-ttu-id="70c44-174">Organisierte Konferenz-Einwahlminuten Microsoft</span><span class="sxs-lookup"><span data-stu-id="70c44-174">Organized Conference Dial-in Microsoft Minutes</span></span>
- <span data-ttu-id="70c44-175">Organisierte Konferenz-Auswahlminuten Microsoft</span><span class="sxs-lookup"><span data-stu-id="70c44-175">Organized Conference Dial-out Microsoft Minutes</span></span>
- <span data-ttu-id="70c44-176">Anzahl der Konferenz teilgenommen Instant Messaging</span><span class="sxs-lookup"><span data-stu-id="70c44-176">Participated Conference IM Count</span></span>
- <span data-ttu-id="70c44-177">Anzahl Teilgenommene Konferenz-Audio/Video</span><span class="sxs-lookup"><span data-stu-id="70c44-177">Participated Conference Audio/Video Count</span></span>
- <span data-ttu-id="70c44-178">Teilgenommene Konferenz-Audio-/Videominuten</span><span class="sxs-lookup"><span data-stu-id="70c44-178">Participated Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="70c44-179">Anzahl Teilgenommene Konferenz-App-Freigabe</span><span class="sxs-lookup"><span data-stu-id="70c44-179">Participated Conference App Sharing Count</span></span>
- <span data-ttu-id="70c44-180">Anzahl Teilgenommene Konferenz-Web</span><span class="sxs-lookup"><span data-stu-id="70c44-180">Participated Conference Web Count</span></span>
- <span data-ttu-id="70c44-181">Anzahl Teilgenommene Konferenz-Einwahl/Auswahl Drittanbieter</span><span class="sxs-lookup"><span data-stu-id="70c44-181">Participated Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="70c44-182">Zugewiesene Produkte</span><span class="sxs-lookup"><span data-stu-id="70c44-182">Assigned Products</span></span>
- <span data-ttu-id="70c44-183">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="70c44-183">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="70c44-184">JSON</span><span class="sxs-lookup"><span data-stu-id="70c44-184">JSON</span></span>

<span data-ttu-id="70c44-185">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines **[SkypeForBusinessActivityUserDetail](../resources/skypeforbusinessactivityuserdetail.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="70c44-185">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessActivityUserDetail](../resources/skypeforbusinessactivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="70c44-186">Die Seite Standardgröße für diese Anforderung ist 200 Elemente.</span><span class="sxs-lookup"><span data-stu-id="70c44-186">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="70c44-187">Beispiel</span><span class="sxs-lookup"><span data-stu-id="70c44-187">Example</span></span>

### <a name="csv"></a><span data-ttu-id="70c44-188">CSV</span><span class="sxs-lookup"><span data-stu-id="70c44-188">CSV</span></span>

<span data-ttu-id="70c44-189">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="70c44-189">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="70c44-190">Anforderung</span><span class="sxs-lookup"><span data-stu-id="70c44-190">Request</span></span>

<span data-ttu-id="70c44-191">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="70c44-191">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessactivityuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="70c44-192">Antwort</span><span class="sxs-lookup"><span data-stu-id="70c44-192">Response</span></span>

<span data-ttu-id="70c44-193">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="70c44-193">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="70c44-194">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="70c44-194">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Is Deleted,Deleted Date,Last Activity Date,Total Peer-to-peer Session Count,Total Organized Conference Count,Total Participated Conference Count,Peer-to-peer Last Activity Date,Organized Conference Last Activity Date,Participated Conference Last Activity Date,Peer-to-peer IM Count,Peer-to-peer Audio Count,Peer-to-peer Audio Minutes,Peer-to-peer Video Count,Peer-to-peer Video Minutes,Peer-to-peer App Sharing Count,Peer-to-peer File Transfer Count,Organized Conference IM Count,Organized Conference Audio/Video Count,Organized Conference Audio/Video Minutes,Organized Conference App Sharing Count,Organized Conference Web Count,Organized Conference Dial-in/out 3rd Party Count,Organized Conference Dial-in/out Microsoft Count,Organized Conference Dial-in Microsoft Minutes,Organized Conference Dial-out Microsoft Minutes,Participated Conference IM Count,Participated Conference Audio/Video Count,Participated Conference Audio/Video Minutes,Participated Conference App Sharing Count,Participated Conference Web Count,Participated Conference Dial-in/out 3rd Party Count,Assigned Products,Report Period
```

### <a name="json"></a><span data-ttu-id="70c44-195">JSON</span><span class="sxs-lookup"><span data-stu-id="70c44-195">JSON</span></span>

<span data-ttu-id="70c44-196">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="70c44-196">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="70c44-197">Anforderung</span><span class="sxs-lookup"><span data-stu-id="70c44-197">Request</span></span>

<span data-ttu-id="70c44-198">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="70c44-198">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessactivityuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="70c44-199">Antwort</span><span class="sxs-lookup"><span data-stu-id="70c44-199">Response</span></span>

<span data-ttu-id="70c44-200">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="70c44-200">The following is an example of the response.</span></span>

> <span data-ttu-id="70c44-p107">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="70c44-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessActivityUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1419

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessActivityUserDetail)", 
  "value": [
    {
      "totalPeerToPeerSessionCount": 12, 
      "totalOrganizedConferenceCount": 0, 
      "totalParticipatedConferenceCount": 1, 
      "peerToPeerLastActivityDate": "2017-09-01", 
      "organizedConferenceLastActivityDate": null, 
      "participatedConferenceLastActivityDate": "2017-08-31", 
      "peerToPeerIMCount": 12, 
      "peerToPeerAudioCount": 0, 
      "peerToPeerAudioMinutes": 0, 
      "peerToPeerVideoCount": 0, 
      "peerToPeerVideoMinutes": 0, 
      "peerToPeerAppSharingCount": 0, 
      "peerToPeerFileTransferCount": 0, 
      "organizedConferenceIMCount": 0, 
      "organizedConferenceAudioVideoCount": 0, 
      "organizedConferenceAudioVideoMinutes": 0, 
      "organizedConferenceAppSharingCount": 0, 
      "organizedConferenceWebCount": 0, 
      "organizedConferenceDialInOut3rdPartyCount": 0, 
      "organizedConferenceCloudDialInOutMicrosoftCount": 0, 
      "organizedConferenceCloudDialInMicrosoftMinutes": 0, 
      "organizedConferenceCloudDialOutMicrosoftMinutes": 0, 
      "participatedConferenceIMCount": 0, 
      "participatedConferenceAudioVideoCount": 1, 
      "participatedConferenceAudioVideoMinutes": 69, 
      "participatedConferenceAppSharingCount": 0, 
      "participatedConferenceWebCount": 0, 
      "participatedConferenceDialInOut3rdPartyCount": 0, 
      "reportRefreshDate": "2017-09-06", 
      "userPrincipalName": "userPrincipalName-value", 
      "isDeleted": false, 
      "deletedDate": null, 
      "lastActivityDate": "2017-09-01", 
      "assignedProducts": [
        "OFFICE 365 ENTERPRISE E5", 
      ], 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessactivityuserdetail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
