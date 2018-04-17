# <a name="reportroot-getoffice365activeuserdetail"></a><span data-ttu-id="8371a-101">reportRoot: getOffice365ActiveUserDetail</span><span class="sxs-lookup"><span data-stu-id="8371a-101">reportRoot: getOffice365ActiveUserDetail</span></span>

<span data-ttu-id="8371a-102">Rufen Sie Details zu aktiven Office 365-Benutzern ab.</span><span class="sxs-lookup"><span data-stu-id="8371a-102">Get details about Office 365 active users.</span></span>

> <span data-ttu-id="8371a-103">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Aktive Benutzer](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="8371a-103">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="8371a-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8371a-104">Permissions</span></span>

<span data-ttu-id="8371a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8371a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="8371a-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8371a-107">Permission type</span></span>                        | <span data-ttu-id="8371a-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8371a-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="8371a-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8371a-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="8371a-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8371a-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="8371a-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8371a-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8371a-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8371a-112">Not supported.</span></span>                           |
| <span data-ttu-id="8371a-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8371a-113">Application</span></span>                            | <span data-ttu-id="8371a-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8371a-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="8371a-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8371a-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserDetail(period='{period_value}')
GET /reports/getOffice365ActiveUserDetail(date={date_value})
```

## <a name="request-parameters"></a><span data-ttu-id="8371a-116">Anforderungsparameter</span><span class="sxs-lookup"><span data-stu-id="8371a-116">Request parameters</span></span>

<span data-ttu-id="8371a-117">Geben Sie in der Anforderungs-URL einen der folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="8371a-117">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="8371a-118">Parameter</span><span class="sxs-lookup"><span data-stu-id="8371a-118">Parameter</span></span> | <span data-ttu-id="8371a-119">Typ</span><span class="sxs-lookup"><span data-stu-id="8371a-119">Type</span></span>   | <span data-ttu-id="8371a-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8371a-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="8371a-121">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="8371a-121">period</span></span>    | <span data-ttu-id="8371a-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8371a-122">string</span></span> | <span data-ttu-id="8371a-123">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="8371a-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="8371a-124">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="8371a-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="8371a-125">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="8371a-125">These values follow the format D   where    represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="8371a-126">date</span><span class="sxs-lookup"><span data-stu-id="8371a-126">date</span></span>      | <span data-ttu-id="8371a-127">Datum</span><span class="sxs-lookup"><span data-stu-id="8371a-127">Date</span></span>   | <span data-ttu-id="8371a-128">Gibt das Datum an, für das die Benutzer angezeigt werden sollen, die Aktivitäten durchgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="8371a-128">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="8371a-129">{date_value} muss im Format JJJJ-MM-TT vorliegen.</span><span class="sxs-lookup"><span data-stu-id="8371a-129">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="8371a-130">Da dieser Bericht nur für die letzten 30 Tage verfügbar ist, sollte {date_value} ein Datum aus diesem Zeitraum sein.</span><span class="sxs-lookup"><span data-stu-id="8371a-130">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="8371a-131">**Hinweis:** Sie müssen in der URL entweder einen Zeitraum oder ein Datum festlegen.</span><span class="sxs-lookup"><span data-stu-id="8371a-131">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8371a-132">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8371a-132">Request headers</span></span>

| <span data-ttu-id="8371a-133">Name</span><span class="sxs-lookup"><span data-stu-id="8371a-133">Name</span></span>          | <span data-ttu-id="8371a-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8371a-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="8371a-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="8371a-135">Authorization</span></span> | <span data-ttu-id="8371a-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8371a-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="8371a-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="8371a-138">If-None-Match</span></span> | <span data-ttu-id="8371a-139">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8371a-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="8371a-140">Optional.</span><span class="sxs-lookup"><span data-stu-id="8371a-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="8371a-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="8371a-141">Response</span></span>

<span data-ttu-id="8371a-142">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="8371a-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="8371a-143">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8371a-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="8371a-144">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="8371a-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="8371a-145">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="8371a-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="8371a-146">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="8371a-146">Report Refresh Date</span></span>
- <span data-ttu-id="8371a-147">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="8371a-147">User Principal Name</span></span>
- <span data-ttu-id="8371a-148">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="8371a-148">Display Name</span></span>
- <span data-ttu-id="8371a-149">Ist gelöscht</span><span class="sxs-lookup"><span data-stu-id="8371a-149">Is Deleted</span></span>
- <span data-ttu-id="8371a-150">Gelöscht am</span><span class="sxs-lookup"><span data-stu-id="8371a-150">Deleted Date</span></span>
- <span data-ttu-id="8371a-151">Besitzt Exchange-Lizenz</span><span class="sxs-lookup"><span data-stu-id="8371a-151">Has Exchange License</span></span>
- <span data-ttu-id="8371a-152">Besitzt OneDrive-Lizenz</span><span class="sxs-lookup"><span data-stu-id="8371a-152">Has OneDrive License</span></span>
- <span data-ttu-id="8371a-153">Besitzt SharePoint-Lizenz</span><span class="sxs-lookup"><span data-stu-id="8371a-153">Has SharePoint License</span></span>
- <span data-ttu-id="8371a-154">Besitzt Skype For Business-Lizenz</span><span class="sxs-lookup"><span data-stu-id="8371a-154">Has Skype For Business License</span></span>
- <span data-ttu-id="8371a-155">Besitzt Yammer-Lizenz</span><span class="sxs-lookup"><span data-stu-id="8371a-155">Has Yammer License</span></span>
- <span data-ttu-id="8371a-156">Besitzt Teams-Lizenz</span><span class="sxs-lookup"><span data-stu-id="8371a-156">Has Teams License</span></span>
- <span data-ttu-id="8371a-157">Datum der letzten Exchange-Aktivität</span><span class="sxs-lookup"><span data-stu-id="8371a-157">Exchange Last Activity Date</span></span>
- <span data-ttu-id="8371a-158">Datum der letzten OneDrive-Aktivität</span><span class="sxs-lookup"><span data-stu-id="8371a-158">OneDrive Last Activity Date</span></span>
- <span data-ttu-id="8371a-159">Datum der letzten SharePoint-Aktivität</span><span class="sxs-lookup"><span data-stu-id="8371a-159">SharePoint Last Activity Date</span></span>
- <span data-ttu-id="8371a-160">Datum der letzten Skype for Business-Aktivität</span><span class="sxs-lookup"><span data-stu-id="8371a-160">Skype For Business Last Activity Date</span></span>
- <span data-ttu-id="8371a-161">Datum der letzten Yammer-Aktivität</span><span class="sxs-lookup"><span data-stu-id="8371a-161">Yammer Last Activity Date</span></span>
- <span data-ttu-id="8371a-162">Datum der letzten Teams-Aktivität</span><span class="sxs-lookup"><span data-stu-id="8371a-162">Teams Last Activity Date</span></span>
- <span data-ttu-id="8371a-163">Datum der Exchange-Lizenzzuweisung</span><span class="sxs-lookup"><span data-stu-id="8371a-163">Exchange License Assign Date</span></span>
- <span data-ttu-id="8371a-164">Datum der OneDrive-Lizenzzuweisung</span><span class="sxs-lookup"><span data-stu-id="8371a-164">OneDrive License Assign Date</span></span>
- <span data-ttu-id="8371a-165">Datum der SharePoint-Lizenzzuweisung</span><span class="sxs-lookup"><span data-stu-id="8371a-165">SharePoint License Assign Date</span></span>
- <span data-ttu-id="8371a-166">Datum der Skype For Business-Lizenzzuweisung</span><span class="sxs-lookup"><span data-stu-id="8371a-166">Skype For Business License Assign Date</span></span>
- <span data-ttu-id="8371a-167">Datum der Yammer-Lizenzzuweisung</span><span class="sxs-lookup"><span data-stu-id="8371a-167">Yammer License Assign Date</span></span>
- <span data-ttu-id="8371a-168">Datum der Teams-Lizenzzuweisung</span><span class="sxs-lookup"><span data-stu-id="8371a-168">Teams License Assign Date</span></span>
- <span data-ttu-id="8371a-169">Zugewiesene Produkte</span><span class="sxs-lookup"><span data-stu-id="8371a-169">Assigned Products</span></span>

## <a name="example"></a><span data-ttu-id="8371a-170">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8371a-170">Example</span></span>

#### <a name="request"></a><span data-ttu-id="8371a-171">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8371a-171">Request</span></span>

<span data-ttu-id="8371a-172">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8371a-172">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActiveUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="8371a-173">Antwort</span><span class="sxs-lookup"><span data-stu-id="8371a-173">Response</span></span>

<span data-ttu-id="8371a-174">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8371a-174">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="8371a-175">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="8371a-175">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Has Exchange License,Has OneDrive License,Has SharePoint License,Has Skype For Business License,Has Yammer License,Has Teams License,Exchange Last Activity Date,OneDrive Last Activity Date,SharePoint Last Activity Date,Skype For Business Last Activity Date,Yammer Last Activity Date,Teams Last Activity Date,Exchange License Assign Date,OneDrive License Assign Date,SharePoint License Assign Date,Skype For Business License Assign Date,Yammer License Assign Date,Teams License Assign Date,Assigned Products
```
