# <a name="reportroot-getsharepointactivityuserdetail"></a><span data-ttu-id="48b2d-101">reportRoot: getSharePointActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="48b2d-101">reportRoot: getSharePointActivityUserDetail</span></span>

<span data-ttu-id="48b2d-102">Rufen Sie Details zu SharePoint-Aktivitäten nach Benutzer ab.</span><span class="sxs-lookup"><span data-stu-id="48b2d-102">Get details about SharePoint activity by user.</span></span>

> <span data-ttu-id="48b2d-103">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – SharePoint-Aktivität](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="48b2d-103">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="48b2d-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="48b2d-104">Permissions</span></span>

<span data-ttu-id="48b2d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="48b2d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="48b2d-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="48b2d-107">Permission type</span></span>                        | <span data-ttu-id="48b2d-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="48b2d-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="48b2d-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="48b2d-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="48b2d-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="48b2d-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="48b2d-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="48b2d-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48b2d-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="48b2d-112">Not supported.</span></span>                           |
| <span data-ttu-id="48b2d-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="48b2d-113">Application</span></span>                            | <span data-ttu-id="48b2d-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="48b2d-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="48b2d-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="48b2d-115">HTTP request</span></span>

<!-- { "blockType": "samples" } --> 

```http
GET /reports/getSharePointActivityUserDetail(period='{period_value}')
GET /reports/getSharePointActivityUserDetail(date={date_value})
```

## <a name="request-parameters"></a><span data-ttu-id="48b2d-116">Anforderungsparameter</span><span class="sxs-lookup"><span data-stu-id="48b2d-116">Request parameters</span></span>

<span data-ttu-id="48b2d-117">Geben Sie in der Anforderungs-URL einen der folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="48b2d-117">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="48b2d-118">Parameter</span><span class="sxs-lookup"><span data-stu-id="48b2d-118">Parameter</span></span> | <span data-ttu-id="48b2d-119">Typ</span><span class="sxs-lookup"><span data-stu-id="48b2d-119">Type</span></span>   | <span data-ttu-id="48b2d-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="48b2d-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="48b2d-121">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="48b2d-121">period</span></span>    | <span data-ttu-id="48b2d-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="48b2d-122">string</span></span> | <span data-ttu-id="48b2d-123">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="48b2d-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="48b2d-124">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="48b2d-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="48b2d-125">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="48b2d-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="48b2d-126">Datum</span><span class="sxs-lookup"><span data-stu-id="48b2d-126">date</span></span>      | <span data-ttu-id="48b2d-127">Datum</span><span class="sxs-lookup"><span data-stu-id="48b2d-127">Date</span></span>   | <span data-ttu-id="48b2d-128">Gibt das Datum an, für das die Benutzer angezeigt werden sollen, die Aktivitäten durchgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="48b2d-128">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="48b2d-129">{date_value} muss im Format JJJJ-MM-TT vorliegen.</span><span class="sxs-lookup"><span data-stu-id="48b2d-129">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="48b2d-130">Da dieser Bericht nur für die letzten 30 Tage verfügbar ist, sollte {date_value} ein Datum aus diesem Zeitraum sein.</span><span class="sxs-lookup"><span data-stu-id="48b2d-130">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="48b2d-131">**Hinweis:** Sie müssen in der URL entweder einen Zeitraum oder ein Datum festlegen.</span><span class="sxs-lookup"><span data-stu-id="48b2d-131">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="48b2d-132">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="48b2d-132">Request headers</span></span>

| <span data-ttu-id="48b2d-133">Name</span><span class="sxs-lookup"><span data-stu-id="48b2d-133">Name</span></span>          | <span data-ttu-id="48b2d-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="48b2d-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="48b2d-135">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="48b2d-135">Authorization</span></span> | <span data-ttu-id="48b2d-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="48b2d-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="48b2d-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="48b2d-138">If-None-Match</span></span> | <span data-ttu-id="48b2d-139">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="48b2d-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="48b2d-140">Optional.</span><span class="sxs-lookup"><span data-stu-id="48b2d-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="48b2d-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="48b2d-141">Response</span></span>

<span data-ttu-id="48b2d-142">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="48b2d-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="48b2d-143">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="48b2d-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="48b2d-144">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="48b2d-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="48b2d-145">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="48b2d-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="48b2d-146">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="48b2d-146">Report Refresh Date</span></span>
- <span data-ttu-id="48b2d-147">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="48b2d-147">User Principal Name</span></span>
- <span data-ttu-id="48b2d-148">Ist gelöscht</span><span class="sxs-lookup"><span data-stu-id="48b2d-148">Is Deleted</span></span>
- <span data-ttu-id="48b2d-149">Gelöscht am</span><span class="sxs-lookup"><span data-stu-id="48b2d-149">Deleted Date</span></span>
- <span data-ttu-id="48b2d-150">Datum der letzten Aktivität</span><span class="sxs-lookup"><span data-stu-id="48b2d-150">Last Activity Date</span></span>
- <span data-ttu-id="48b2d-151">Anzahl der angezeigten oder bearbeiteten Dateien</span><span class="sxs-lookup"><span data-stu-id="48b2d-151">Viewed Or Edited File Count</span></span>
- <span data-ttu-id="48b2d-152">Anzahl der synchronisierten Dateien</span><span class="sxs-lookup"><span data-stu-id="48b2d-152">Synced File Count</span></span>
- <span data-ttu-id="48b2d-153">Anzahl der intern freigegebenen Dateien</span><span class="sxs-lookup"><span data-stu-id="48b2d-153">Shared Internally File Count</span></span>
- <span data-ttu-id="48b2d-154">Anzahl der extern freigegebenen Dateien</span><span class="sxs-lookup"><span data-stu-id="48b2d-154">Shared Externally File Count</span></span>
- <span data-ttu-id="48b2d-155">Anzahl der besuchten Seiten</span><span class="sxs-lookup"><span data-stu-id="48b2d-155">Visited Page Count</span></span>
- <span data-ttu-id="48b2d-156">Zugewiesene Produkte</span><span class="sxs-lookup"><span data-stu-id="48b2d-156">Assigned Products</span></span>
- <span data-ttu-id="48b2d-157">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="48b2d-157">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="48b2d-158">Beispiel</span><span class="sxs-lookup"><span data-stu-id="48b2d-158">Example</span></span>

#### <a name="request"></a><span data-ttu-id="48b2d-159">Anforderung</span><span class="sxs-lookup"><span data-stu-id="48b2d-159">Request</span></span>

<span data-ttu-id="48b2d-160">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="48b2d-160">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getsharepointactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointActivityUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="48b2d-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="48b2d-161">Response</span></span>

<span data-ttu-id="48b2d-162">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="48b2d-162">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.report"
} -->

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="48b2d-163">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="48b2d-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Is Deleted,Deleted Date,Last Activity Date,Viewed Or Edited File Count,Synced File Count,Shared Internally File Count,Shared Externally File Count,Visited Page Count,Assigned Products,Report Period
```
