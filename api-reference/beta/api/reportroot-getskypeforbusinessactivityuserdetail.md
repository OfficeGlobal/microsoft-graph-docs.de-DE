---
title: 'reportRoot: getSkypeForBusinessActivityUserDetail'
description: Rufen Sie Details der Skype for Business-Aktivität nach Benutzer ab.
ms.openlocfilehash: 39113039226b48bcefc2121acda5ff5e554d5cd0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058786"
---
# <a name="reportroot-getskypeforbusinessactivityuserdetail"></a><span data-ttu-id="63cdf-103">reportRoot: getSkypeForBusinessActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="63cdf-103">reportRoot: getSkypeForBusinessActivityUserDetail</span></span>

> <span data-ttu-id="63cdf-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="63cdf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="63cdf-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="63cdf-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="63cdf-106">Rufen Sie Details der Skype for Business-Aktivität nach Benutzer ab.</span><span class="sxs-lookup"><span data-stu-id="63cdf-106">Get details about Skype for Business activity by user.</span></span>

> <span data-ttu-id="63cdf-107">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Skype for Business-Aktivität](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span><span class="sxs-lookup"><span data-stu-id="63cdf-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="permissions"></a><span data-ttu-id="63cdf-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="63cdf-108">Permissions</span></span>

<span data-ttu-id="63cdf-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63cdf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="63cdf-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="63cdf-111">Permission type</span></span>                        | <span data-ttu-id="63cdf-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="63cdf-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="63cdf-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="63cdf-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="63cdf-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="63cdf-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="63cdf-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="63cdf-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63cdf-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="63cdf-116">Not supported.</span></span>                           |
| <span data-ttu-id="63cdf-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="63cdf-117">Application</span></span>                            | <span data-ttu-id="63cdf-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="63cdf-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="63cdf-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="63cdf-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessActivityUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="63cdf-120">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="63cdf-120">Function parameters</span></span>

<span data-ttu-id="63cdf-121">Geben Sie in der Anforderungs-URL einen der folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="63cdf-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="63cdf-122">Parameter</span><span class="sxs-lookup"><span data-stu-id="63cdf-122">Parameter</span></span> | <span data-ttu-id="63cdf-123">Typ</span><span class="sxs-lookup"><span data-stu-id="63cdf-123">Type</span></span>   | <span data-ttu-id="63cdf-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="63cdf-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="63cdf-125">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="63cdf-125">period</span></span>    | <span data-ttu-id="63cdf-126">string</span><span class="sxs-lookup"><span data-stu-id="63cdf-126">string</span></span> | <span data-ttu-id="63cdf-127">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="63cdf-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="63cdf-128">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="63cdf-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="63cdf-129">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="63cdf-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="63cdf-130">date</span><span class="sxs-lookup"><span data-stu-id="63cdf-130">date</span></span>      | <span data-ttu-id="63cdf-131">Datum</span><span class="sxs-lookup"><span data-stu-id="63cdf-131">Date</span></span>   | <span data-ttu-id="63cdf-132">Gibt das Datum an, für das die Benutzer angezeigt werden sollen, die Aktivitäten durchgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="63cdf-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="63cdf-133">{date_value} muss im Format JJJJ-MM-TT vorliegen.</span><span class="sxs-lookup"><span data-stu-id="63cdf-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="63cdf-134">Da dieser Bericht nur für die letzten 30 Tage verfügbar ist, sollte {date_value} ein Datum aus diesem Zeitraum sein.</span><span class="sxs-lookup"><span data-stu-id="63cdf-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="63cdf-135">**Hinweis:** Sie müssen in der URL entweder einen Zeitraum oder ein Datum festlegen.</span><span class="sxs-lookup"><span data-stu-id="63cdf-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="63cdf-136">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) von  `$format`, `$top` und `$skipToken` zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="63cdf-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="63cdf-137">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="63cdf-137">The default output type is text/csv.</span></span> <span data-ttu-id="63cdf-138">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="63cdf-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="63cdf-139">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="63cdf-139">Request headers</span></span>

| <span data-ttu-id="63cdf-140">Name</span><span class="sxs-lookup"><span data-stu-id="63cdf-140">Name</span></span>          | <span data-ttu-id="63cdf-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="63cdf-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="63cdf-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="63cdf-142">Authorization</span></span> | <span data-ttu-id="63cdf-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="63cdf-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="63cdf-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="63cdf-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="63cdf-146">CSV</span><span class="sxs-lookup"><span data-stu-id="63cdf-146">CSV</span></span>

<span data-ttu-id="63cdf-147">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="63cdf-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="63cdf-148">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="63cdf-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="63cdf-149">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="63cdf-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="63cdf-150">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="63cdf-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="63cdf-151">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="63cdf-151">Report Refresh Date</span></span>
- <span data-ttu-id="63cdf-152">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="63cdf-152">User Principal Name</span></span>
- <span data-ttu-id="63cdf-153">Ist gelöscht</span><span class="sxs-lookup"><span data-stu-id="63cdf-153">Is Deleted</span></span>
- <span data-ttu-id="63cdf-154">Gelöscht am</span><span class="sxs-lookup"><span data-stu-id="63cdf-154">Deleted Date</span></span>
- <span data-ttu-id="63cdf-155">Datum der letzten Aktivität</span><span class="sxs-lookup"><span data-stu-id="63cdf-155">Last Activity Date</span></span>
- <span data-ttu-id="63cdf-156">Gesamtzahl Peer-to-Peer-Sitzung</span><span class="sxs-lookup"><span data-stu-id="63cdf-156">Total Peer-to-peer Session Count</span></span>
- <span data-ttu-id="63cdf-157">Gesamtzahl Organisierte Konferenz</span><span class="sxs-lookup"><span data-stu-id="63cdf-157">Total Organized Conference Count</span></span>
- <span data-ttu-id="63cdf-158">Gesamtzahl der teilgenommenen Konferenzen</span><span class="sxs-lookup"><span data-stu-id="63cdf-158">Total Participated Conference Count</span></span>
- <span data-ttu-id="63cdf-159">Datum der letzten Peer-to-Peer-Aktivität</span><span class="sxs-lookup"><span data-stu-id="63cdf-159">Peer-to-peer Last Activity Date</span></span>
- <span data-ttu-id="63cdf-160">Datum der letzten Aktivität der organisierten Konferenz</span><span class="sxs-lookup"><span data-stu-id="63cdf-160">Organized Conference Last Activity Date</span></span>
- <span data-ttu-id="63cdf-161">Datum der letzten Aktivität der teilgenommenen Konferenz</span><span class="sxs-lookup"><span data-stu-id="63cdf-161">Participated Conference Last Activity Date</span></span>
- <span data-ttu-id="63cdf-162">Anzahl Peer-to-Peer-Chat</span><span class="sxs-lookup"><span data-stu-id="63cdf-162">Peer-to-peer IM Count</span></span>
- <span data-ttu-id="63cdf-163">Anzahl Peer-to-Peer-Audio</span><span class="sxs-lookup"><span data-stu-id="63cdf-163">Peer-to-peer Audio Count</span></span>
- <span data-ttu-id="63cdf-164">Peer-to-Peer-Audiominuten</span><span class="sxs-lookup"><span data-stu-id="63cdf-164">Peer-to-peer Audio Minutes</span></span>
- <span data-ttu-id="63cdf-165">Anzahl Peer-to-Peer-Video</span><span class="sxs-lookup"><span data-stu-id="63cdf-165">Peer-to-peer Video Count</span></span>
- <span data-ttu-id="63cdf-166">Peer-to-Peer-Videominuten</span><span class="sxs-lookup"><span data-stu-id="63cdf-166">Peer-to-peer Video Minutes</span></span>
- <span data-ttu-id="63cdf-167">Anzahl Peer-to-Peer-App-Freigabe</span><span class="sxs-lookup"><span data-stu-id="63cdf-167">Peer-to-peer App Sharing Count</span></span>
- <span data-ttu-id="63cdf-168">Anzahl Peer-to-Peer-Dateiübertragung</span><span class="sxs-lookup"><span data-stu-id="63cdf-168">Peer-to-peer File Transfer Count</span></span>
- <span data-ttu-id="63cdf-169">Anzahl Organisierte Konferenz-Chat</span><span class="sxs-lookup"><span data-stu-id="63cdf-169">Organized Conference IM Count</span></span>
- <span data-ttu-id="63cdf-170">Anzahl Organisierte Konferenz-Audio/Video</span><span class="sxs-lookup"><span data-stu-id="63cdf-170">Organized Conference Audio/Video Count</span></span>
- <span data-ttu-id="63cdf-171">Anzahl Organisierte Konferenz-Audio-/Videominuten</span><span class="sxs-lookup"><span data-stu-id="63cdf-171">Organized Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="63cdf-172">Anzahl Organisierte Konferenz-App-Freigabe</span><span class="sxs-lookup"><span data-stu-id="63cdf-172">Organized Conference App Sharing Count</span></span>
- <span data-ttu-id="63cdf-173">Anzahl Organisierte Konferenz-Web</span><span class="sxs-lookup"><span data-stu-id="63cdf-173">Organized Conference Web Count</span></span>
- <span data-ttu-id="63cdf-174">Anzahl Organisierte Konferenz-Einwahl/Auswahl Drittanbieter</span><span class="sxs-lookup"><span data-stu-id="63cdf-174">Organized Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="63cdf-175">Anzahl Organisierte Konferenz-Einwahl/Auswahl Microsoft</span><span class="sxs-lookup"><span data-stu-id="63cdf-175">Organized Conference Dial-in/out Microsoft Count</span></span>
- <span data-ttu-id="63cdf-176">Organisierte Konferenz-Einwahlminuten Microsoft</span><span class="sxs-lookup"><span data-stu-id="63cdf-176">Organized Conference Dial-in Microsoft Minutes</span></span>
- <span data-ttu-id="63cdf-177">Organisierte Konferenz-Auswahlminuten Microsoft</span><span class="sxs-lookup"><span data-stu-id="63cdf-177">Organized Conference Dial-out Microsoft Minutes</span></span>
- <span data-ttu-id="63cdf-178">Anzahl der Konferenz teilgenommen Instant Messaging</span><span class="sxs-lookup"><span data-stu-id="63cdf-178">Participated Conference IM Count</span></span>
- <span data-ttu-id="63cdf-179">Anzahl Teilgenommene Konferenz-Audio/Video</span><span class="sxs-lookup"><span data-stu-id="63cdf-179">Participated Conference Audio/Video Count</span></span>
- <span data-ttu-id="63cdf-180">Teilgenommene Konferenz-Audio-/Videominuten</span><span class="sxs-lookup"><span data-stu-id="63cdf-180">Participated Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="63cdf-181">Anzahl Teilgenommene Konferenz-App-Freigabe</span><span class="sxs-lookup"><span data-stu-id="63cdf-181">Participated Conference App Sharing Count</span></span>
- <span data-ttu-id="63cdf-182">Anzahl Teilgenommene Konferenz-Web</span><span class="sxs-lookup"><span data-stu-id="63cdf-182">Participated Conference Web Count</span></span>
- <span data-ttu-id="63cdf-183">Anzahl Teilgenommene Konferenz-Einwahl/Auswahl Drittanbieter</span><span class="sxs-lookup"><span data-stu-id="63cdf-183">Participated Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="63cdf-184">Zugewiesene Produkte</span><span class="sxs-lookup"><span data-stu-id="63cdf-184">Assigned Products</span></span>
- <span data-ttu-id="63cdf-185">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="63cdf-185">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="63cdf-186">JSON</span><span class="sxs-lookup"><span data-stu-id="63cdf-186">JSON</span></span>

<span data-ttu-id="63cdf-187">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines **[SkypeForBusinessActivityUserDetail](../resources/skypeforbusinessactivityuserdetail.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="63cdf-187">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessActivityUserDetail](../resources/skypeforbusinessactivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="63cdf-188">Die Seite Standardgröße für diese Anforderung ist 200 Elemente.</span><span class="sxs-lookup"><span data-stu-id="63cdf-188">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="63cdf-189">Beispiel</span><span class="sxs-lookup"><span data-stu-id="63cdf-189">Example</span></span>

### <a name="csv"></a><span data-ttu-id="63cdf-190">CSV</span><span class="sxs-lookup"><span data-stu-id="63cdf-190">CSV</span></span>

<span data-ttu-id="63cdf-191">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="63cdf-191">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="63cdf-192">Anforderung</span><span class="sxs-lookup"><span data-stu-id="63cdf-192">Request</span></span>

<span data-ttu-id="63cdf-193">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="63cdf-193">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessactivityuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="63cdf-194">Antwort</span><span class="sxs-lookup"><span data-stu-id="63cdf-194">Response</span></span>

<span data-ttu-id="63cdf-195">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="63cdf-195">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="63cdf-196">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="63cdf-196">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="63cdf-197">JSON</span><span class="sxs-lookup"><span data-stu-id="63cdf-197">JSON</span></span>

<span data-ttu-id="63cdf-198">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="63cdf-198">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="63cdf-199">Anforderung</span><span class="sxs-lookup"><span data-stu-id="63cdf-199">Request</span></span>

<span data-ttu-id="63cdf-200">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="63cdf-200">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessactivityuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="63cdf-201">Antwort</span><span class="sxs-lookup"><span data-stu-id="63cdf-201">Response</span></span>

<span data-ttu-id="63cdf-202">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="63cdf-202">The following is an example of the response.</span></span>

> <span data-ttu-id="63cdf-p108">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="63cdf-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
