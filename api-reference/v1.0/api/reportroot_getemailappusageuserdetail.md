# <a name="reportroot-getemailappusageuserdetail"></a><span data-ttu-id="cdb11-101">reportRoot: getEmailAppUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="cdb11-101">reportRoot: getEmailAppUsageUserDetail</span></span>

<span data-ttu-id="cdb11-102">Erhalten Sie detaillierte Informationen darüber, welche Aktivitäten Benutzer mit den verschiedenen E-Mail-Apps ausgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="cdb11-102">Get details about which activities users performed on the various email apps.</span></span>

> <span data-ttu-id="cdb11-103">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Nutzung von E-Mail-Apps](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span><span class="sxs-lookup"><span data-stu-id="cdb11-103">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="cdb11-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="cdb11-104">Permissions</span></span>

<span data-ttu-id="cdb11-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="cdb11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="cdb11-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cdb11-107">Permission type</span></span>                        | <span data-ttu-id="cdb11-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cdb11-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="cdb11-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cdb11-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="cdb11-110">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cdb11-110">Not supported.</span></span>                           |
| <span data-ttu-id="cdb11-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cdb11-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cdb11-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cdb11-112">Not supported.</span></span>                           |
| <span data-ttu-id="cdb11-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cdb11-113">Application</span></span>                            | <span data-ttu-id="cdb11-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="cdb11-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="cdb11-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cdb11-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageUserDetail(period='{period_value}')
GET /reports/getEmailAppUsageUserDetail(date={date_value})
```

## <a name="request-parameters"></a><span data-ttu-id="cdb11-116">Anforderungsparameter</span><span class="sxs-lookup"><span data-stu-id="cdb11-116">Request parameters</span></span>

<span data-ttu-id="cdb11-117">Stellen Sie in der URL der Anforderung die folgenden Parameter mit einem gültigen Wert bereit.</span><span class="sxs-lookup"><span data-stu-id="cdb11-117">In the request URL, provide the following query parameter with a valid value.</span></span>

| <span data-ttu-id="cdb11-118">Parameter</span><span class="sxs-lookup"><span data-stu-id="cdb11-118">Parameter</span></span> | <span data-ttu-id="cdb11-119">Typ</span><span class="sxs-lookup"><span data-stu-id="cdb11-119">Type</span></span>   | <span data-ttu-id="cdb11-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cdb11-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="cdb11-121">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="cdb11-121">period</span></span>    | <span data-ttu-id="cdb11-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cdb11-122">string</span></span> | <span data-ttu-id="cdb11-123">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="cdb11-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="cdb11-124">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="cdb11-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="cdb11-125">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="cdb11-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="cdb11-126">date</span><span class="sxs-lookup"><span data-stu-id="cdb11-126">date</span></span>      | <span data-ttu-id="cdb11-127">Datum</span><span class="sxs-lookup"><span data-stu-id="cdb11-127">Date</span></span>   | <span data-ttu-id="cdb11-128">Gibt das Datum an, für das die Benutzer angezeigt werden sollen, die Aktivitäten durchgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="cdb11-128">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="cdb11-129">{date_value} muss im Format JJJJ-MM-TT vorliegen.</span><span class="sxs-lookup"><span data-stu-id="cdb11-129">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="cdb11-130">Da dieser Bericht nur für die letzten 30 Tage verfügbar ist, sollte {date_value} ein Datum aus diesem Zeitraum sein.</span><span class="sxs-lookup"><span data-stu-id="cdb11-130">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="cdb11-131">**Hinweis:** Sie müssen in der URL entweder einen Zeitraum oder ein Datum festlegen.</span><span class="sxs-lookup"><span data-stu-id="cdb11-131">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cdb11-132">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cdb11-132">Request headers</span></span>

| <span data-ttu-id="cdb11-133">Name</span><span class="sxs-lookup"><span data-stu-id="cdb11-133">Name</span></span>          | <span data-ttu-id="cdb11-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cdb11-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="cdb11-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="cdb11-135">Authorization</span></span> | <span data-ttu-id="cdb11-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cdb11-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="cdb11-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="cdb11-138">If-None-Match</span></span> | <span data-ttu-id="cdb11-139">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cdb11-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="cdb11-140">Optional.</span><span class="sxs-lookup"><span data-stu-id="cdb11-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="cdb11-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="cdb11-141">Response</span></span>

<span data-ttu-id="cdb11-142">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="cdb11-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="cdb11-143">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="cdb11-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="cdb11-144">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="cdb11-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="cdb11-145">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="cdb11-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="cdb11-146">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="cdb11-146">Report Refresh Date</span></span>
- <span data-ttu-id="cdb11-147">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="cdb11-147">User Principal Name</span></span>
- <span data-ttu-id="cdb11-148">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="cdb11-148">Display Name</span></span>
- <span data-ttu-id="cdb11-149">Ist gelöscht</span><span class="sxs-lookup"><span data-stu-id="cdb11-149">Is Deleted</span></span>
- <span data-ttu-id="cdb11-150">Gelöscht am</span><span class="sxs-lookup"><span data-stu-id="cdb11-150">Deleted Date</span></span>
- <span data-ttu-id="cdb11-151">Datum der letzten Aktivität</span><span class="sxs-lookup"><span data-stu-id="cdb11-151">Last Activity Date</span></span>
- <span data-ttu-id="cdb11-152">E-Mail für Mac</span><span class="sxs-lookup"><span data-stu-id="cdb11-152">Mail For Mac</span></span>
- <span data-ttu-id="cdb11-153">Outlook für Mac</span><span class="sxs-lookup"><span data-stu-id="cdb11-153">Outlook For Mac</span></span>
- <span data-ttu-id="cdb11-154">Outlook für Windows</span><span class="sxs-lookup"><span data-stu-id="cdb11-154">Outlook For Windows</span></span>
- <span data-ttu-id="cdb11-155">Outlook für mobile Geräte</span><span class="sxs-lookup"><span data-stu-id="cdb11-155">Outlook For Mobile</span></span>
- <span data-ttu-id="cdb11-156">Weiteres für mobile Geräte</span><span class="sxs-lookup"><span data-stu-id="cdb11-156">Other For Mobile</span></span>
- <span data-ttu-id="cdb11-157">Outlook für Web</span><span class="sxs-lookup"><span data-stu-id="cdb11-157">Outlook For Web</span></span>
- <span data-ttu-id="cdb11-158">POP3-App</span><span class="sxs-lookup"><span data-stu-id="cdb11-158">POP3 App</span></span>
- <span data-ttu-id="cdb11-159">IMAP4-App</span><span class="sxs-lookup"><span data-stu-id="cdb11-159">IMAP4 App</span></span>
- <span data-ttu-id="cdb11-160">SMTP-App</span><span class="sxs-lookup"><span data-stu-id="cdb11-160">SMTP App</span></span>
- <span data-ttu-id="cdb11-161">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="cdb11-161">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="cdb11-162">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cdb11-162">Example</span></span>

#### <a name="request"></a><span data-ttu-id="cdb11-163">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cdb11-163">Request</span></span>

<span data-ttu-id="cdb11-164">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cdb11-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getEmailAppUsageUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="cdb11-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="cdb11-165">Response</span></span>

<span data-ttu-id="cdb11-166">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="cdb11-166">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="cdb11-167">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="cdb11-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Last Activity Date,Mail For Mac,Outlook For Mac,Outlook For Windows,Outlook For Mobile,Other For Mobile,Outlook For Web,POP3 App,IMAP4 App,SMTP App,Report Period
```
