# <a name="reportroot-getoffice365groupsactivitydetail"></a><span data-ttu-id="080d9-101">reportRoot: getOffice365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="080d9-101">reportRoot: getOffice365GroupsActivityDetail</span></span>

<span data-ttu-id="080d9-102">Rufen Sie Details zur Office 365-Gruppenaktivität nach Gruppe ab.</span><span class="sxs-lookup"><span data-stu-id="080d9-102">Get details about Office 365 Groups activity by group.</span></span>

> <span data-ttu-id="080d9-103">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Office 365-Gruppen](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="080d9-103">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="080d9-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="080d9-104">Permissions</span></span>

<span data-ttu-id="080d9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="080d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="080d9-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="080d9-107">Permission type</span></span>                        | <span data-ttu-id="080d9-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="080d9-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="080d9-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="080d9-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="080d9-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="080d9-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="080d9-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="080d9-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="080d9-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="080d9-112">Not supported.</span></span>                           |
| <span data-ttu-id="080d9-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="080d9-113">Application</span></span>                            | <span data-ttu-id="080d9-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="080d9-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="080d9-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="080d9-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityDetail(period='{period_value}')
GET /reports/getOffice365GroupsActivityDetail(date={date_value})
```

## <a name="request-parameters"></a><span data-ttu-id="080d9-116">Anforderungsparameter</span><span class="sxs-lookup"><span data-stu-id="080d9-116">Request parameters</span></span>

<span data-ttu-id="080d9-117">Geben Sie in der Anforderungs-URL einen der folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="080d9-117">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="080d9-118">Parameter</span><span class="sxs-lookup"><span data-stu-id="080d9-118">Parameter</span></span> | <span data-ttu-id="080d9-119">Typ</span><span class="sxs-lookup"><span data-stu-id="080d9-119">Type</span></span>   | <span data-ttu-id="080d9-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="080d9-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="080d9-121">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="080d9-121">period</span></span>    | <span data-ttu-id="080d9-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="080d9-122">string</span></span> | <span data-ttu-id="080d9-123">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="080d9-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="080d9-124">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="080d9-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="080d9-125">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="080d9-125">These values follow the format D   where    represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="080d9-126">date</span><span class="sxs-lookup"><span data-stu-id="080d9-126">date</span></span>      | <span data-ttu-id="080d9-127">Datum</span><span class="sxs-lookup"><span data-stu-id="080d9-127">Date</span></span>   | <span data-ttu-id="080d9-128">Gibt das Datum an, für das die Benutzer angezeigt werden sollen, die Aktivitäten durchgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="080d9-128">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="080d9-129">{date_value} muss im Format JJJJ-MM-TT vorliegen.</span><span class="sxs-lookup"><span data-stu-id="080d9-129">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="080d9-130">Da dieser Bericht nur für die letzten 30 Tage verfügbar ist, sollte {date_value} ein Datum aus diesem Zeitraum sein.</span><span class="sxs-lookup"><span data-stu-id="080d9-130">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="080d9-131">**Hinweis:** Sie müssen in der URL entweder einen Zeitraum oder ein Datum festlegen.</span><span class="sxs-lookup"><span data-stu-id="080d9-131">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="080d9-132">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="080d9-132">Request headers</span></span>

| <span data-ttu-id="080d9-133">Name</span><span class="sxs-lookup"><span data-stu-id="080d9-133">Name</span></span>          | <span data-ttu-id="080d9-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="080d9-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="080d9-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="080d9-135">Authorization</span></span> | <span data-ttu-id="080d9-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="080d9-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="080d9-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="080d9-138">If-None-Match</span></span> | <span data-ttu-id="080d9-139">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="080d9-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="080d9-140">Optional.</span><span class="sxs-lookup"><span data-stu-id="080d9-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="080d9-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="080d9-141">Response</span></span>

<span data-ttu-id="080d9-142">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="080d9-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="080d9-143">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="080d9-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="080d9-144">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="080d9-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="080d9-145">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="080d9-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="080d9-146">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="080d9-146">Report Refresh Date</span></span>
- <span data-ttu-id="080d9-147">Gruppenanzeigename</span><span class="sxs-lookup"><span data-stu-id="080d9-147">Group Display Name</span></span>
- <span data-ttu-id="080d9-148">Ist gelöscht</span><span class="sxs-lookup"><span data-stu-id="080d9-148">Is Deleted</span></span>
- <span data-ttu-id="080d9-149">Besitzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="080d9-149">Owner Principal Name</span></span>
- <span data-ttu-id="080d9-150">Datum der letzten Aktivität</span><span class="sxs-lookup"><span data-stu-id="080d9-150">Last Activity Date</span></span>
- <span data-ttu-id="080d9-151">Gruppentyp</span><span class="sxs-lookup"><span data-stu-id="080d9-151">Group Type</span></span>
- <span data-ttu-id="080d9-152">Mitgliederzahl</span><span class="sxs-lookup"><span data-stu-id="080d9-152">Member Count</span></span>
- <span data-ttu-id="080d9-153">Anzahl der externen Mitglieder</span><span class="sxs-lookup"><span data-stu-id="080d9-153">External Member Count</span></span>
- <span data-ttu-id="080d9-154">Anzahl der mit Exchange empfangenen E-Mail-Nachrichten</span><span class="sxs-lookup"><span data-stu-id="080d9-154">Exchange Received Email Count</span></span>
- <span data-ttu-id="080d9-155">Anzahl der aktiven SharePoint-Dateien</span><span class="sxs-lookup"><span data-stu-id="080d9-155">SharePoint Active File Count</span></span>
- <span data-ttu-id="080d9-156">Anzahl der veröffentlichten Yammer-Nachrichten</span><span class="sxs-lookup"><span data-stu-id="080d9-156">Yammer Posted Message Count</span></span>
- <span data-ttu-id="080d9-157">Anzahl der gelesenen Yammer-Nachricht</span><span class="sxs-lookup"><span data-stu-id="080d9-157">Yammer Read Message Count</span></span>
- <span data-ttu-id="080d9-158">Anzahl der gelikten Yammer-Nachrichten</span><span class="sxs-lookup"><span data-stu-id="080d9-158">Yammer Liked Message Count</span></span>
- <span data-ttu-id="080d9-159">Gesamtanzahl der Exchange-Postfachelemente</span><span class="sxs-lookup"><span data-stu-id="080d9-159">Exchange Mailbox Total Item Count</span></span>
- <span data-ttu-id="080d9-160">Verwendeter Exchange-Postfachspeicherplatz (Byte)</span><span class="sxs-lookup"><span data-stu-id="080d9-160">Exchange Mailbox Storage Used (Byte)</span></span>
- <span data-ttu-id="080d9-161">Gesamtzahl der SharePoint-Dateien</span><span class="sxs-lookup"><span data-stu-id="080d9-161">SharePoint Total File Count</span></span>
- <span data-ttu-id="080d9-162">Verwendeter SharePoint-Websitesspeicherplatz (Byte)</span><span class="sxs-lookup"><span data-stu-id="080d9-162">SharePoint Site Storage Used (Byte)</span></span>
- <span data-ttu-id="080d9-163">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="080d9-163">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="080d9-164">Beispiel</span><span class="sxs-lookup"><span data-stu-id="080d9-164">Example</span></span>

#### <a name="request"></a><span data-ttu-id="080d9-165">Anforderung</span><span class="sxs-lookup"><span data-stu-id="080d9-165">Request</span></span>

<span data-ttu-id="080d9-166">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="080d9-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365GroupsActivityDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="080d9-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="080d9-167">Response</span></span>

<span data-ttu-id="080d9-168">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="080d9-168">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="080d9-169">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="080d9-169">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Group Display Name,Is Deleted,Owner Principal Name,Last Activity Date,Group Type,Member Count,Guest Count,Exchange Received Email Count,SharePoint Active File Count,Yammer Posted Message Count,Yammer Read Message Count,Yammer Liked Message Count,Exchange Mailbox Total Item Count,Exchange Mailbox Storage Used (Byte),SharePoint Total File Count,SharePoint Site Storage Used (Byte),Report Period
```
