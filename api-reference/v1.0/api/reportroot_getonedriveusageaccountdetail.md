# <a name="reportroot-getonedriveusageaccountdetail"></a><span data-ttu-id="b01a0-101">reportRoot: getOneDriveUsageAccountDetail</span><span class="sxs-lookup"><span data-stu-id="b01a0-101">reportRoot: getOneDriveUsageAccountDetail</span></span>

<span data-ttu-id="b01a0-102">Rufen Sie Details zur OneDrive-Nutzung nach Konto ab.</span><span class="sxs-lookup"><span data-stu-id="b01a0-102">Get details about OneDrive usage by account.</span></span>

> <span data-ttu-id="b01a0-103">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – OneDrive for Business-Nutzung](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span><span class="sxs-lookup"><span data-stu-id="b01a0-103">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="b01a0-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b01a0-104">Permissions</span></span>

<span data-ttu-id="b01a0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b01a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="b01a0-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b01a0-107">Permission type</span></span>                        | <span data-ttu-id="b01a0-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b01a0-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b01a0-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b01a0-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="b01a0-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b01a0-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b01a0-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b01a0-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b01a0-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b01a0-112">Not supported.</span></span>                           |
| <span data-ttu-id="b01a0-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b01a0-113">Application</span></span>                            | <span data-ttu-id="b01a0-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b01a0-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="b01a0-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b01a0-115">HTTP request</span></span>

<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOneDriveUsageAccountDetail(period='{period_value}')
GET /reports/getOneDriveUsageAccountDetail(date={date_value})
```

## <a name="request-parameters"></a><span data-ttu-id="b01a0-116">Anforderungsparameter</span><span class="sxs-lookup"><span data-stu-id="b01a0-116">Request parameters</span></span>

<span data-ttu-id="b01a0-117">Geben Sie in der Anforderungs-URL einen der folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="b01a0-117">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="b01a0-118">Parameter</span><span class="sxs-lookup"><span data-stu-id="b01a0-118">Parameter</span></span> | <span data-ttu-id="b01a0-119">Typ</span><span class="sxs-lookup"><span data-stu-id="b01a0-119">Type</span></span>   | <span data-ttu-id="b01a0-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b01a0-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="b01a0-121">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="b01a0-121">period</span></span>    | <span data-ttu-id="b01a0-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b01a0-122">string</span></span> | <span data-ttu-id="b01a0-123">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="b01a0-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="b01a0-124">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="b01a0-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="b01a0-125">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="b01a0-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="b01a0-126">date</span><span class="sxs-lookup"><span data-stu-id="b01a0-126">date</span></span>      | <span data-ttu-id="b01a0-127">Datum</span><span class="sxs-lookup"><span data-stu-id="b01a0-127">Date</span></span>   | <span data-ttu-id="b01a0-128">Gibt das Datum an, für das die Benutzer angezeigt werden sollen, die Aktivitäten durchgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="b01a0-128">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="b01a0-129">{date_value} muss im Format JJJJ-MM-TT vorliegen.</span><span class="sxs-lookup"><span data-stu-id="b01a0-129">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="b01a0-130">Da dieser Bericht nur für die letzten 30 Tage verfügbar ist, sollte {date_value} ein Datum aus diesem Zeitraum sein.</span><span class="sxs-lookup"><span data-stu-id="b01a0-130">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="b01a0-131">**Hinweis:** Sie müssen in der URL entweder einen Zeitraum oder ein Datum festlegen.</span><span class="sxs-lookup"><span data-stu-id="b01a0-131">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b01a0-132">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b01a0-132">Request headers</span></span>

| <span data-ttu-id="b01a0-133">Name</span><span class="sxs-lookup"><span data-stu-id="b01a0-133">Name</span></span>          | <span data-ttu-id="b01a0-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b01a0-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="b01a0-135">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="b01a0-135">Authorization</span></span> | <span data-ttu-id="b01a0-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b01a0-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="b01a0-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="b01a0-138">If-None-Match</span></span> | <span data-ttu-id="b01a0-139">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b01a0-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="b01a0-140">Optional.</span><span class="sxs-lookup"><span data-stu-id="b01a0-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="b01a0-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="b01a0-141">Response</span></span>

<span data-ttu-id="b01a0-142">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="b01a0-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b01a0-143">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b01a0-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b01a0-144">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="b01a0-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b01a0-145">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="b01a0-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="b01a0-146">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="b01a0-146">Report Refresh Date</span></span>
- <span data-ttu-id="b01a0-147">Website-URL</span><span class="sxs-lookup"><span data-stu-id="b01a0-147">Site URL</span></span>
- <span data-ttu-id="b01a0-148">Anzeigename des Besitzers</span><span class="sxs-lookup"><span data-stu-id="b01a0-148">Owner Display Name</span></span>
- <span data-ttu-id="b01a0-149">Ist gelöscht</span><span class="sxs-lookup"><span data-stu-id="b01a0-149">Is Deleted</span></span>
- <span data-ttu-id="b01a0-150">Datum der letzten Aktivität</span><span class="sxs-lookup"><span data-stu-id="b01a0-150">Last Activity Date</span></span>
- <span data-ttu-id="b01a0-151">Anzahl der Dateien</span><span class="sxs-lookup"><span data-stu-id="b01a0-151">File Count</span></span>
- <span data-ttu-id="b01a0-152">Anzahl der aktiven Datei</span><span class="sxs-lookup"><span data-stu-id="b01a0-152">Active File Count</span></span>
- <span data-ttu-id="b01a0-153">Verwendeter Speicherplatz (Byte)</span><span class="sxs-lookup"><span data-stu-id="b01a0-153">Storage Used (Byte)</span></span>
- <span data-ttu-id="b01a0-154">Zugewiesener Speicherplatz (Byte)</span><span class="sxs-lookup"><span data-stu-id="b01a0-154">Storage Allocated (Byte)</span></span>
- <span data-ttu-id="b01a0-155">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="b01a0-155">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="b01a0-156">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b01a0-156">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b01a0-157">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b01a0-157">Request</span></span>

<span data-ttu-id="b01a0-158">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b01a0-158">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getonedriveusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOneDriveUsageAccountDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="b01a0-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="b01a0-159">Response</span></span>

<span data-ttu-id="b01a0-160">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b01a0-160">The following is an example of the response.</span></span>

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

<span data-ttu-id="b01a0-161">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="b01a0-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site URL,Owner Display Name,Is Deleted,Last Activity Date,File Count,Active File Count,Storage Used (Byte),Storage Allocated (Byte),Report Period
```
