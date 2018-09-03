# <a name="reportroot-getyammeractivityuserdetail"></a><span data-ttu-id="7c488-101">reportRoot: getYammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="7c488-101">reportRoot: getYammerActivityUserDetail</span></span>

<span data-ttu-id="7c488-102">Rufen Sie Details zu Yammer-Aktivitäten nach Benutzer ab.</span><span class="sxs-lookup"><span data-stu-id="7c488-102">Get details about Yammer activity by user.</span></span>

> <span data-ttu-id="7c488-103">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Yammer-Aktivität](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span><span class="sxs-lookup"><span data-stu-id="7c488-103">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="permissions"></a><span data-ttu-id="7c488-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7c488-104">Permissions</span></span>

<span data-ttu-id="7c488-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7c488-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="7c488-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7c488-107">Permission type</span></span>                        | <span data-ttu-id="7c488-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7c488-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="7c488-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7c488-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="7c488-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c488-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="7c488-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7c488-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c488-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7c488-112">Not supported.</span></span>                           |
| <span data-ttu-id="7c488-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7c488-113">Application</span></span>                            | <span data-ttu-id="7c488-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c488-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="7c488-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7c488-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerActivityUserDetail(period='{period_value}')
GET /reports/getYammerActivityUserDetail(date={date_value})
```

## <a name="request-parameters"></a><span data-ttu-id="7c488-116">Anforderungsparameter</span><span class="sxs-lookup"><span data-stu-id="7c488-116">Request parameters</span></span>

<span data-ttu-id="7c488-117">Geben Sie in der Anforderungs-URL einen der folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="7c488-117">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="7c488-118">Parameter</span><span class="sxs-lookup"><span data-stu-id="7c488-118">Parameter</span></span> | <span data-ttu-id="7c488-119">Typ</span><span class="sxs-lookup"><span data-stu-id="7c488-119">Type</span></span>   | <span data-ttu-id="7c488-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7c488-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="7c488-121">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="7c488-121">period</span></span>    | <span data-ttu-id="7c488-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7c488-122">string</span></span> | <span data-ttu-id="7c488-123">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="7c488-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="7c488-124">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="7c488-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="7c488-125">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="7c488-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="7c488-126">date</span><span class="sxs-lookup"><span data-stu-id="7c488-126">date</span></span>      | <span data-ttu-id="7c488-127">Datum</span><span class="sxs-lookup"><span data-stu-id="7c488-127">Date</span></span>   | <span data-ttu-id="7c488-128">Gibt das Datum an, für das die Benutzer angezeigt werden sollen, die Aktivitäten durchgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="7c488-128">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="7c488-129">{date_value} muss im Format JJJJ-MM-TT vorliegen.</span><span class="sxs-lookup"><span data-stu-id="7c488-129">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="7c488-130">Da dieser Bericht nur für die letzten 30 Tage verfügbar ist, sollte {date_value} ein Datum aus diesem Zeitraum sein.</span><span class="sxs-lookup"><span data-stu-id="7c488-130">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="7c488-131">**Hinweis:** Sie müssen in der URL entweder einen Zeitraum oder ein Datum festlegen.</span><span class="sxs-lookup"><span data-stu-id="7c488-131">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7c488-132">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7c488-132">Request headers</span></span>

| <span data-ttu-id="7c488-133">Name</span><span class="sxs-lookup"><span data-stu-id="7c488-133">Name</span></span>          | <span data-ttu-id="7c488-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7c488-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="7c488-135">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="7c488-135">Authorization</span></span> | <span data-ttu-id="7c488-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7c488-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="7c488-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="7c488-138">If-None-Match</span></span> | <span data-ttu-id="7c488-139">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7c488-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="7c488-140">Optional.</span><span class="sxs-lookup"><span data-stu-id="7c488-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="7c488-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="7c488-141">Response</span></span>

<span data-ttu-id="7c488-142">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="7c488-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="7c488-143">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7c488-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="7c488-144">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="7c488-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="7c488-145">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="7c488-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="7c488-146">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="7c488-146">Report Refresh Date</span></span>
- <span data-ttu-id="7c488-147">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="7c488-147">User Principal Name</span></span>
- <span data-ttu-id="7c488-148">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="7c488-148">Display Name</span></span>
- <span data-ttu-id="7c488-149">Benutzerstatus</span><span class="sxs-lookup"><span data-stu-id="7c488-149">User State</span></span>
- <span data-ttu-id="7c488-150">Datum der Statusänderung</span><span class="sxs-lookup"><span data-stu-id="7c488-150">State Change Date</span></span>
- <span data-ttu-id="7c488-151">Datum der letzten Aktivität</span><span class="sxs-lookup"><span data-stu-id="7c488-151">Last Activity Date</span></span>
- <span data-ttu-id="7c488-152">Anzahl veröffentlicht</span><span class="sxs-lookup"><span data-stu-id="7c488-152">Posted Count</span></span>
- <span data-ttu-id="7c488-153">Anzahl gelesen</span><span class="sxs-lookup"><span data-stu-id="7c488-153">Read Count</span></span>
- <span data-ttu-id="7c488-154">Anzahl gelikt</span><span class="sxs-lookup"><span data-stu-id="7c488-154">Liked Count</span></span>
- <span data-ttu-id="7c488-155">Zugewiesene Produkte</span><span class="sxs-lookup"><span data-stu-id="7c488-155">Assigned Products</span></span>
- <span data-ttu-id="7c488-156">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="7c488-156">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="7c488-157">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7c488-157">Example</span></span>

#### <a name="request"></a><span data-ttu-id="7c488-158">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7c488-158">Request</span></span>

<span data-ttu-id="7c488-159">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7c488-159">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammeractivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerActivityUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="7c488-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="7c488-160">Response</span></span>

<span data-ttu-id="7c488-161">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7c488-161">The following is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.report" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

#### <a name="request"></a><span data-ttu-id="7c488-162">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7c488-162">Request</span></span>

<span data-ttu-id="7c488-163">Wenn der `date` Parameter angegeben ist, wird der Bericht auf Aktivitäten beschränkt, die an dem angegebenen Datum stattgefunden haben.</span><span class="sxs-lookup"><span data-stu-id="7c488-163">If the `date` parameter is specified, the report is scoped to activities that took place on the given date.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammeractivityuserdetail_date"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerActivityUserDetail(date='2018-03-05')
```

#### <a name="response"></a><span data-ttu-id="7c488-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="7c488-164">Response</span></span>

<span data-ttu-id="7c488-165">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7c488-165">The following is an example of the response.</span></span>

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


<span data-ttu-id="7c488-166">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="7c488-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,User State,State Change Date,Last Activity Date,Posted Count,Read Count,Liked Count,Assigned Products,Report Period
```
