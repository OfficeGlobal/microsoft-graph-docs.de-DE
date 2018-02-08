# <a name="reportroot-getyammerdeviceusageuserdetail-function"></a><span data-ttu-id="593ae-101">reportRoot: getYammerDeviceUsageUserDetail function</span><span class="sxs-lookup"><span data-stu-id="593ae-101">reportRoot: getYammerDeviceUsageUserDetail function</span></span>

<span data-ttu-id="593ae-102">Rufen Sie Details zur Yammer-Gerätenutzung nach Benutzer ab.</span><span class="sxs-lookup"><span data-stu-id="593ae-102">Get details about Yammer device usage by user.</span></span>

> <span data-ttu-id="593ae-103">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Yammer-Gerätenutzung](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="593ae-103">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="593ae-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="593ae-104">Permissions</span></span>

<span data-ttu-id="593ae-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="593ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="593ae-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="593ae-107">Permission type</span></span>                        | <span data-ttu-id="593ae-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="593ae-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="593ae-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="593ae-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="593ae-110">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="593ae-110">Not supported.</span></span>                           |
| <span data-ttu-id="593ae-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="593ae-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="593ae-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="593ae-112">Not supported.</span></span>                           |
| <span data-ttu-id="593ae-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="593ae-113">Application</span></span>                            | <span data-ttu-id="593ae-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="593ae-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="593ae-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="593ae-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageUserDetail(period='{period_value}')
GET /reports/getYammerDeviceUsageUserDetail(date={date_value})
```

## <a name="request-parameters"></a><span data-ttu-id="593ae-116">Anforderungsparameter</span><span class="sxs-lookup"><span data-stu-id="593ae-116">Request parameters</span></span>

<span data-ttu-id="593ae-117">Stellen Sie in der URL der Anforderung den Parameter mit einem gültigen Wert bereit.</span><span class="sxs-lookup"><span data-stu-id="593ae-117">In the request URL, provide the chosen query parameter with a valid value.</span></span>

| <span data-ttu-id="593ae-118">Parameter</span><span class="sxs-lookup"><span data-stu-id="593ae-118">Parameter</span></span> | <span data-ttu-id="593ae-119">Typ</span><span class="sxs-lookup"><span data-stu-id="593ae-119">Type</span></span>   | <span data-ttu-id="593ae-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="593ae-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="593ae-121">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="593ae-121">period</span></span>    | <span data-ttu-id="593ae-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="593ae-122">string</span></span> | <span data-ttu-id="593ae-123">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="593ae-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="593ae-124">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="593ae-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="593ae-125">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="593ae-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="593ae-126">date</span><span class="sxs-lookup"><span data-stu-id="593ae-126">date</span></span>      | <span data-ttu-id="593ae-127">Datum</span><span class="sxs-lookup"><span data-stu-id="593ae-127">Date</span></span>   | <span data-ttu-id="593ae-128">Gibt das Datum an, für das die Benutzer angezeigt werden sollen, die Aktivitäten durchgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="593ae-128">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="593ae-129">{date_value} muss im Format JJJJ-MM-TT vorliegen.</span><span class="sxs-lookup"><span data-stu-id="593ae-129">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="593ae-130">Da dieser Bericht nur für die letzten 30 Tage verfügbar ist, sollte {date_value} ein Datum aus diesem Zeitraum sein.</span><span class="sxs-lookup"><span data-stu-id="593ae-130">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="593ae-131">**Hinweis:** Sie müssen in der URL entweder einen Zeitraum oder ein Datum festlegen.</span><span class="sxs-lookup"><span data-stu-id="593ae-131">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="593ae-132">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="593ae-132">Request headers</span></span>

| <span data-ttu-id="593ae-133">Name</span><span class="sxs-lookup"><span data-stu-id="593ae-133">Name</span></span>          | <span data-ttu-id="593ae-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="593ae-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="593ae-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="593ae-135">Authorization</span></span> | <span data-ttu-id="593ae-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="593ae-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="593ae-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="593ae-138">If-None-Match</span></span> | <span data-ttu-id="593ae-139">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="593ae-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="593ae-140">Optional.</span><span class="sxs-lookup"><span data-stu-id="593ae-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="593ae-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="593ae-141">Response</span></span>

<span data-ttu-id="593ae-142">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="593ae-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="593ae-143">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="593ae-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="593ae-144">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="593ae-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="593ae-145">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="593ae-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="593ae-146">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="593ae-146">Report Refresh Date</span></span>
- <span data-ttu-id="593ae-147">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="593ae-147">User Principal Name</span></span>
- <span data-ttu-id="593ae-148">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="593ae-148">Display Name</span></span>
- <span data-ttu-id="593ae-149">Benutzerstatus</span><span class="sxs-lookup"><span data-stu-id="593ae-149">User State</span></span>
- <span data-ttu-id="593ae-150">Datum der Statusänderung</span><span class="sxs-lookup"><span data-stu-id="593ae-150">State Change Date</span></span>
- <span data-ttu-id="593ae-151">Datum der letzten Aktivität</span><span class="sxs-lookup"><span data-stu-id="593ae-151">Last Activity Date</span></span>
- <span data-ttu-id="593ae-152">Verwendetes Web</span><span class="sxs-lookup"><span data-stu-id="593ae-152">Used Web</span></span>
- <span data-ttu-id="593ae-153">Verwendetes Windows Phone</span><span class="sxs-lookup"><span data-stu-id="593ae-153">Used Windows Phone</span></span>
- <span data-ttu-id="593ae-154">Verwendetes Android Phone</span><span class="sxs-lookup"><span data-stu-id="593ae-154">Used Android Phone</span></span>
- <span data-ttu-id="593ae-155">Verwendetes iPhone</span><span class="sxs-lookup"><span data-stu-id="593ae-155">Used iPhone</span></span>
- <span data-ttu-id="593ae-156">Verwendetes iPad</span><span class="sxs-lookup"><span data-stu-id="593ae-156">Used iPad</span></span>
- <span data-ttu-id="593ae-157">Andere verwendet</span><span class="sxs-lookup"><span data-stu-id="593ae-157">Used Others</span></span>
- <span data-ttu-id="593ae-158">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="593ae-158">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="593ae-159">Beispiel</span><span class="sxs-lookup"><span data-stu-id="593ae-159">Example</span></span>

#### <a name="request"></a><span data-ttu-id="593ae-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="593ae-160">Request</span></span>

<span data-ttu-id="593ae-161">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="593ae-161">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerDeviceUsageUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="593ae-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="593ae-162">Response</span></span>

<span data-ttu-id="593ae-163">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="593ae-163">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="593ae-164">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="593ae-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,User State,State Change Date,Last Activity Date,Used Web,Used Windows Phone,Used Android Phone,Used iPhone,Used iPad,Used Others,Report Period
```
