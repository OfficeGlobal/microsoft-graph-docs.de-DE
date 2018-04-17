# <a name="reportroot-getskypeforbusinessactivityuserdetail"></a><span data-ttu-id="578e6-101">reportRoot: getSkypeForBusinessActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="578e6-101">reportRoot: getSkypeForBusinessActivityUserDetail</span></span>

<span data-ttu-id="578e6-102">Rufen Sie Details der Skype for Business-Aktivität nach Benutzer ab.</span><span class="sxs-lookup"><span data-stu-id="578e6-102">Get details about Skype for Business activity by user.</span></span>

> <span data-ttu-id="578e6-103">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Skype for Business-Aktivität](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span><span class="sxs-lookup"><span data-stu-id="578e6-103">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="permissions"></a><span data-ttu-id="578e6-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="578e6-104">Permissions</span></span>

<span data-ttu-id="578e6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="578e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="578e6-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="578e6-107">Permission type</span></span>                        | <span data-ttu-id="578e6-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="578e6-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="578e6-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="578e6-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="578e6-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="578e6-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="578e6-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="578e6-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="578e6-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="578e6-112">Not supported.</span></span>                           |
| <span data-ttu-id="578e6-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="578e6-113">Application</span></span>                            | <span data-ttu-id="578e6-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="578e6-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="578e6-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="578e6-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessActivityUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessActivityUserDetail(date={date_value})
```

## <a name="request-parameters"></a><span data-ttu-id="578e6-116">Anforderungsparameter</span><span class="sxs-lookup"><span data-stu-id="578e6-116">Request parameters</span></span>

<span data-ttu-id="578e6-117">Geben Sie in der Anforderungs-URL einen der folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="578e6-117">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="578e6-118">Parameter</span><span class="sxs-lookup"><span data-stu-id="578e6-118">Parameter</span></span> | <span data-ttu-id="578e6-119">Typ</span><span class="sxs-lookup"><span data-stu-id="578e6-119">Type</span></span>   | <span data-ttu-id="578e6-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="578e6-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="578e6-121">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="578e6-121">period</span></span>    | <span data-ttu-id="578e6-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="578e6-122">string</span></span> | <span data-ttu-id="578e6-123">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="578e6-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="578e6-124">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="578e6-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="578e6-125">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="578e6-125">These values follow the format D   where    represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="578e6-126">date</span><span class="sxs-lookup"><span data-stu-id="578e6-126">date</span></span>      | <span data-ttu-id="578e6-127">Datum</span><span class="sxs-lookup"><span data-stu-id="578e6-127">Date</span></span>   | <span data-ttu-id="578e6-128">Gibt das Datum an, für das die Benutzer angezeigt werden sollen, die Aktivitäten durchgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="578e6-128">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="578e6-129">{date_value} muss im Format JJJJ-MM-TT vorliegen.</span><span class="sxs-lookup"><span data-stu-id="578e6-129">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="578e6-130">Da dieser Bericht nur für die letzten 30 Tage verfügbar ist, sollte {date_value} ein Datum aus diesem Zeitraum sein.</span><span class="sxs-lookup"><span data-stu-id="578e6-130">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="578e6-131">**Hinweis:** Sie müssen in der URL entweder einen Zeitraum oder ein Datum festlegen.</span><span class="sxs-lookup"><span data-stu-id="578e6-131">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="578e6-132">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="578e6-132">Request headers</span></span>

| <span data-ttu-id="578e6-133">Name</span><span class="sxs-lookup"><span data-stu-id="578e6-133">Name</span></span>          | <span data-ttu-id="578e6-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="578e6-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="578e6-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="578e6-135">Authorization</span></span> | <span data-ttu-id="578e6-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="578e6-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="578e6-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="578e6-138">If-None-Match</span></span> | <span data-ttu-id="578e6-139">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="578e6-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="578e6-140">Optional.</span><span class="sxs-lookup"><span data-stu-id="578e6-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="578e6-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="578e6-141">Response</span></span>

<span data-ttu-id="578e6-142">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="578e6-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="578e6-143">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="578e6-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="578e6-144">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="578e6-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="578e6-145">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="578e6-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="578e6-146">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="578e6-146">Report Refresh Date</span></span>
- <span data-ttu-id="578e6-147">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="578e6-147">User Principal Name</span></span>
- <span data-ttu-id="578e6-148">Ist gelöscht</span><span class="sxs-lookup"><span data-stu-id="578e6-148">Is Deleted</span></span>
- <span data-ttu-id="578e6-149">Gelöscht am</span><span class="sxs-lookup"><span data-stu-id="578e6-149">Deleted Date</span></span>
- <span data-ttu-id="578e6-150">Datum der letzten Aktivität</span><span class="sxs-lookup"><span data-stu-id="578e6-150">Last Activity Date</span></span>
- <span data-ttu-id="578e6-151">Gesamtzahl Peer-to-Peer-Sitzung</span><span class="sxs-lookup"><span data-stu-id="578e6-151">Total Peer-to-peer Session Count</span></span>
- <span data-ttu-id="578e6-152">Gesamtzahl Organisierte Konferenz</span><span class="sxs-lookup"><span data-stu-id="578e6-152">Total Organized Conference Count</span></span>
- <span data-ttu-id="578e6-153">Gesamtzahl der teilgenommenen Konferenzen</span><span class="sxs-lookup"><span data-stu-id="578e6-153">Total Participated Conference Count</span></span>
- <span data-ttu-id="578e6-154">Datum der letzten Peer-to-Peer-Aktivität</span><span class="sxs-lookup"><span data-stu-id="578e6-154">Peer-to-peer Last Activity Date</span></span>
- <span data-ttu-id="578e6-155">Datum der letzten Aktivität der organisierten Konferenz</span><span class="sxs-lookup"><span data-stu-id="578e6-155">Organized Conference Last Activity Date</span></span>
- <span data-ttu-id="578e6-156">Datum der letzten Aktivität der teilgenommenen Konferenz</span><span class="sxs-lookup"><span data-stu-id="578e6-156">Participated Conference Last Activity Date</span></span>
- <span data-ttu-id="578e6-157">Anzahl Peer-to-Peer-Chat</span><span class="sxs-lookup"><span data-stu-id="578e6-157">Peer-to-peer IM Count</span></span>
- <span data-ttu-id="578e6-158">Anzahl Peer-to-Peer-Audio</span><span class="sxs-lookup"><span data-stu-id="578e6-158">Peer-to-peer Audio Count</span></span>
- <span data-ttu-id="578e6-159">Peer-to-Peer-Audiominuten</span><span class="sxs-lookup"><span data-stu-id="578e6-159">Peer-to-peer Audio Minutes</span></span>
- <span data-ttu-id="578e6-160">Anzahl Peer-to-Peer-Video</span><span class="sxs-lookup"><span data-stu-id="578e6-160">Peer-to-peer Video Count</span></span>
- <span data-ttu-id="578e6-161">Peer-to-Peer-Videominuten</span><span class="sxs-lookup"><span data-stu-id="578e6-161">Peer-to-peer Video Minutes</span></span>
- <span data-ttu-id="578e6-162">Anzahl Peer-to-Peer-App-Freigabe</span><span class="sxs-lookup"><span data-stu-id="578e6-162">Peer-to-peer App Sharing Count</span></span>
- <span data-ttu-id="578e6-163">Anzahl Peer-to-Peer-Dateiübertragung</span><span class="sxs-lookup"><span data-stu-id="578e6-163">Peer-to-peer File Transfer Count</span></span>
- <span data-ttu-id="578e6-164">Anzahl Organisierte Konferenz-Chat</span><span class="sxs-lookup"><span data-stu-id="578e6-164">Organized Conference IM Count</span></span>
- <span data-ttu-id="578e6-165">Anzahl Organisierte Konferenz-Audio/Video</span><span class="sxs-lookup"><span data-stu-id="578e6-165">Organized Conference Audio/Video Count</span></span>
- <span data-ttu-id="578e6-166">Anzahl Organisierte Konferenz-Audio-/Videominuten</span><span class="sxs-lookup"><span data-stu-id="578e6-166">Organized Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="578e6-167">Anzahl Organisierte Konferenz-App-Freigabe</span><span class="sxs-lookup"><span data-stu-id="578e6-167">Organized Conference App Sharing Count</span></span>
- <span data-ttu-id="578e6-168">Anzahl Organisierte Konferenz-Web</span><span class="sxs-lookup"><span data-stu-id="578e6-168">Organized Conference Web Count</span></span>
- <span data-ttu-id="578e6-169">Anzahl Organisierte Konferenz-Einwahl/Auswahl Drittanbieter</span><span class="sxs-lookup"><span data-stu-id="578e6-169">Organized Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="578e6-170">Anzahl Organisierte Konferenz-Einwahl/Auswahl Microsoft</span><span class="sxs-lookup"><span data-stu-id="578e6-170">Organized Conference Dial-in/out Microsoft Count</span></span>
- <span data-ttu-id="578e6-171">Organisierte Konferenz-Einwahlminuten Microsoft</span><span class="sxs-lookup"><span data-stu-id="578e6-171">Organized Conference Dial-in Microsoft Minutes</span></span>
- <span data-ttu-id="578e6-172">Organisierte Konferenz-Auswahlminuten Microsoft</span><span class="sxs-lookup"><span data-stu-id="578e6-172">Organized Conference Dial-out Microsoft Minutes</span></span>
- <span data-ttu-id="578e6-173">Anzahl Teilgenommene Konferenz-Chat</span><span class="sxs-lookup"><span data-stu-id="578e6-173">Paricipated Conference IM Count</span></span>
- <span data-ttu-id="578e6-174">Anzahl Teilgenommene Konferenz-Audio/Video</span><span class="sxs-lookup"><span data-stu-id="578e6-174">Participated Conference Audio/Video Count</span></span>
- <span data-ttu-id="578e6-175">Teilgenommene Konferenz-Audio-/Videominuten</span><span class="sxs-lookup"><span data-stu-id="578e6-175">Participated Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="578e6-176">Anzahl Teilgenommene Konferenz-App-Freigabe</span><span class="sxs-lookup"><span data-stu-id="578e6-176">Participated Conference App Sharing Count</span></span>
- <span data-ttu-id="578e6-177">Anzahl Teilgenommene Konferenz-Web</span><span class="sxs-lookup"><span data-stu-id="578e6-177">Participated Conference Web Count</span></span>
- <span data-ttu-id="578e6-178">Anzahl Teilgenommene Konferenz-Einwahl/Auswahl Drittanbieter</span><span class="sxs-lookup"><span data-stu-id="578e6-178">Participated Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="578e6-179">Zugewiesene Produkte</span><span class="sxs-lookup"><span data-stu-id="578e6-179">Assigned Products</span></span>
- <span data-ttu-id="578e6-180">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="578e6-180">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="578e6-181">Beispiel</span><span class="sxs-lookup"><span data-stu-id="578e6-181">Example</span></span>

#### <a name="request"></a><span data-ttu-id="578e6-182">Anforderung</span><span class="sxs-lookup"><span data-stu-id="578e6-182">Request</span></span>

<span data-ttu-id="578e6-183">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="578e6-183">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessActivityUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="578e6-184">Antwort</span><span class="sxs-lookup"><span data-stu-id="578e6-184">Response</span></span>

<span data-ttu-id="578e6-185">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="578e6-185">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="578e6-186">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="578e6-186">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Is Deleted,Deleted Date,Last Activity Date,Total Peer-to-peer Session Count,Total Organized Conference Count,Total Participated Conference Count,Peer-to-peer Last Activity Date,Organized Conference Last Activity Date,Participated Conference Last Activity Date,Peer-to-peer IM Count,Peer-to-peer Audio Count,Peer-to-peer Audio Minutes,Peer-to-peer Video Count,Peer-to-peer Video Minutes,Peer-to-peer App Sharing Count,Peer-to-peer File Transfer Count,Organized Conference IM Count,Organized Conference Audio/Video Count,Organized Conference Audio/Video Minutes,Organized Conference App Sharing Count,Organized Conference Web Count,Organized Conference Dial-in/out 3rd Party Count,Organized Conference Dial-in/out Microsoft Count,Organized Conference Dial-in Microsoft Minutes,Organized Conference Dial-out Microsoft Minutes,Paricipated Conference IM Count,Participated Conference Audio/Video Count,Participated Conference Audio/Video Minutes,Participated Conference App Sharing Count,Participated Conference Web Count,Participated Conference Dial-in/out 3rd Party Count,Assigned Products,Report Period
```
