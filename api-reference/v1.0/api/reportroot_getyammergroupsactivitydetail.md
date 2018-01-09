# <a name="reportroot-getyammergroupsactivitydetail"></a><span data-ttu-id="7ed8c-101">reportRoot: getYammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="7ed8c-101">reportRoot: getYammerGroupsActivityDetail</span></span>

<span data-ttu-id="7ed8c-102">Rufen Sie Details zur Yammer-Gruppenaktivität nach Gruppe ab.</span><span class="sxs-lookup"><span data-stu-id="7ed8c-102">Get details about Yammer groups activity by group.</span></span>

> <span data-ttu-id="7ed8c-103">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Yammer-Gruppenaktivität]((https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31)).</span><span class="sxs-lookup"><span data-stu-id="7ed8c-103">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity]((https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31)).</span></span>

## <a name="permissions"></a><span data-ttu-id="7ed8c-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7ed8c-104">Permissions</span></span>

<span data-ttu-id="7ed8c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7ed8c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="7ed8c-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7ed8c-107">Permission type</span></span>                        | <span data-ttu-id="7ed8c-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7ed8c-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="7ed8c-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7ed8c-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="7ed8c-110">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7ed8c-110">Not supported.</span></span>                           |
| <span data-ttu-id="7ed8c-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7ed8c-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ed8c-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7ed8c-112">Not supported.</span></span>                           |
| <span data-ttu-id="7ed8c-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7ed8c-113">Application</span></span>                            | <span data-ttu-id="7ed8c-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7ed8c-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="7ed8c-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7ed8c-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerGroupsActivityDetail(period='{period_value}')
GET /reports/getYammerGroupsActivityDetail(date={date_value})
```

## <a name="request-parameters"></a><span data-ttu-id="7ed8c-116">Anforderungsparameter</span><span class="sxs-lookup"><span data-stu-id="7ed8c-116">Request parameters</span></span>

<span data-ttu-id="7ed8c-117">Stellen Sie in der URL der Anforderung den gewählten Abfrageparameter mit einem gültigen Wert bereit.</span><span class="sxs-lookup"><span data-stu-id="7ed8c-117">In the request URL, provide the chosen query parameter with a valid value.</span></span>

| <span data-ttu-id="7ed8c-118">Parameter</span><span class="sxs-lookup"><span data-stu-id="7ed8c-118">Parameter</span></span> | <span data-ttu-id="7ed8c-119">Typ</span><span class="sxs-lookup"><span data-stu-id="7ed8c-119">Type</span></span>   | <span data-ttu-id="7ed8c-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7ed8c-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="7ed8c-121">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="7ed8c-121">Period</span></span>    | <span data-ttu-id="7ed8c-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7ed8c-122">string</span></span> | <span data-ttu-id="7ed8c-123">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="7ed8c-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="7ed8c-124">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="7ed8c-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="7ed8c-125">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="7ed8c-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="7ed8c-126">date</span><span class="sxs-lookup"><span data-stu-id="7ed8c-126">date</span></span>      | <span data-ttu-id="7ed8c-127">Datum</span><span class="sxs-lookup"><span data-stu-id="7ed8c-127">Date</span></span>   | <span data-ttu-id="7ed8c-128">Gibt das Datum an, für das die Benutzer angezeigt werden sollen, die Aktivitäten durchgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="7ed8c-128">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="7ed8c-129">{date_value} muss im Format JJJJ-MM-TT vorliegen.</span><span class="sxs-lookup"><span data-stu-id="7ed8c-129">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="7ed8c-130">Da dieser Bericht nur für die letzten 30 Tage verfügbar ist, sollte {date_value} ein Datum aus diesem Zeitraum sein.</span><span class="sxs-lookup"><span data-stu-id="7ed8c-130">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="7ed8c-131">**Hinweis:** Sie müssen in der URL entweder einen Zeitraum oder ein Datum festlegen.</span><span class="sxs-lookup"><span data-stu-id="7ed8c-131">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7ed8c-132">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7ed8c-132">Request headers</span></span>

| <span data-ttu-id="7ed8c-133">Name</span><span class="sxs-lookup"><span data-stu-id="7ed8c-133">Name</span></span>          | <span data-ttu-id="7ed8c-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7ed8c-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="7ed8c-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ed8c-135">Authorization</span></span> | <span data-ttu-id="7ed8c-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7ed8c-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7ed8c-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="7ed8c-138">if-none-match</span></span> | <span data-ttu-id="7ed8c-139">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7ed8c-139">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `304 Not Modified` response is returned.</span></span> <span data-ttu-id="7ed8c-140">Optional.</span><span class="sxs-lookup"><span data-stu-id="7ed8c-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="7ed8c-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="7ed8c-141">Response</span></span>

<span data-ttu-id="7ed8c-142">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="7ed8c-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="7ed8c-143">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7ed8c-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="7ed8c-144">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="7ed8c-144">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

<span data-ttu-id="7ed8c-145">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="7ed8c-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="7ed8c-146">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="7ed8c-146">Report Refresh Date</span></span>
- <span data-ttu-id="7ed8c-147">Gruppenanzeigename</span><span class="sxs-lookup"><span data-stu-id="7ed8c-147">Group Display Name</span></span>
- <span data-ttu-id="7ed8c-148">Ist gelöscht</span><span class="sxs-lookup"><span data-stu-id="7ed8c-148">Is Deleted</span></span>
- <span data-ttu-id="7ed8c-149">Besitzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="7ed8c-149">Owner Principal Name</span></span>
- <span data-ttu-id="7ed8c-150">Datum der letzten Aktivität</span><span class="sxs-lookup"><span data-stu-id="7ed8c-150">Last Activity Date</span></span>
- <span data-ttu-id="7ed8c-151">Gruppentyp</span><span class="sxs-lookup"><span data-stu-id="7ed8c-151">Group Type</span></span>
- <span data-ttu-id="7ed8c-152">Mit Office 365 verbunden</span><span class="sxs-lookup"><span data-stu-id="7ed8c-152">Office 365 Connected</span></span>
- <span data-ttu-id="7ed8c-153">Mitgliederzahl</span><span class="sxs-lookup"><span data-stu-id="7ed8c-153">Member Count</span></span>
- <span data-ttu-id="7ed8c-154">Anzahl veröffentlicht</span><span class="sxs-lookup"><span data-stu-id="7ed8c-154">Posted Count</span></span>
- <span data-ttu-id="7ed8c-155">Anzahl gelesen</span><span class="sxs-lookup"><span data-stu-id="7ed8c-155">Read Count</span></span>
- <span data-ttu-id="7ed8c-156">Anzahl gelikt</span><span class="sxs-lookup"><span data-stu-id="7ed8c-156">Liked Count</span></span>
- <span data-ttu-id="7ed8c-157">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="7ed8c-157">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="7ed8c-158">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7ed8c-158">Example</span></span>

#### <a name="request"></a><span data-ttu-id="7ed8c-159">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7ed8c-159">Request</span></span>

<span data-ttu-id="7ed8c-160">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7ed8c-160">The following is an example of making the request in ASP.NET that uses the TokenHelper file:</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerGroupsActivityDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="7ed8c-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="7ed8c-161">Response</span></span>

<span data-ttu-id="7ed8c-162">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7ed8c-162">Here is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="7ed8c-163">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="7ed8c-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Group Display Name,Is Deleted,Owner Principal Name,Last Activity Date,Group Type,Office 365 Connected,Member Count,Posted Count,Read Count,Liked Count,Report Period
```
