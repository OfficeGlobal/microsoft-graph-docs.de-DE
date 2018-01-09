# <a name="reportroot-getoffice365groupsactivitycounts"></a><span data-ttu-id="24746-101">reportRoot: getOffice365GroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="24746-101">reportRoot: getOffice365GroupsActivityCounts</span></span>

<span data-ttu-id="24746-102">Rufen Sie die Anzahl der Gruppenaktivitäten für Gruppenarbeitslasten ab.</span><span class="sxs-lookup"><span data-stu-id="24746-102">Get the number of group activities across group workloads.</span></span>

> <span data-ttu-id="24746-103">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Office 365-Gruppen]((https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)).</span><span class="sxs-lookup"><span data-stu-id="24746-103">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups]((https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)).</span></span>

## <a name="permissions"></a><span data-ttu-id="24746-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="24746-104">Permissions</span></span>

<span data-ttu-id="24746-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="24746-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="24746-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="24746-107">Permission type</span></span>                        | <span data-ttu-id="24746-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="24746-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="24746-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="24746-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="24746-110">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="24746-110">Not supported.</span></span>                           |
| <span data-ttu-id="24746-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="24746-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24746-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="24746-112">Not supported.</span></span>                           |
| <span data-ttu-id="24746-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="24746-113">Application</span></span>                            | <span data-ttu-id="24746-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="24746-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="24746-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="24746-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="24746-116">Anforderungsparameter</span><span class="sxs-lookup"><span data-stu-id="24746-116">Request parameters</span></span>

<span data-ttu-id="24746-117">Stellen Sie in der URL der Anforderung die folgenden Abfrageparameter mit einem gültigen Wert bereit.</span><span class="sxs-lookup"><span data-stu-id="24746-117">In the request URL, provide the following query parameter with a valid value.</span></span>

| <span data-ttu-id="24746-118">Parameter</span><span class="sxs-lookup"><span data-stu-id="24746-118">Parameter</span></span> | <span data-ttu-id="24746-119">Typ</span><span class="sxs-lookup"><span data-stu-id="24746-119">Type</span></span>   | <span data-ttu-id="24746-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="24746-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="24746-121">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="24746-121">Period</span></span>    | <span data-ttu-id="24746-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="24746-122">string</span></span> | <span data-ttu-id="24746-123">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="24746-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="24746-124">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="24746-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="24746-125">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="24746-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="24746-126">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="24746-126">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="24746-127">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="24746-127">Request headers</span></span>

| <span data-ttu-id="24746-128">Name</span><span class="sxs-lookup"><span data-stu-id="24746-128">Name</span></span>          | <span data-ttu-id="24746-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="24746-129">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="24746-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="24746-130">Authorization</span></span> | <span data-ttu-id="24746-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="24746-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="24746-133">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="24746-133">if-none-match</span></span> | <span data-ttu-id="24746-134">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="24746-134">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `304 Not Modified` response is returned.</span></span> <span data-ttu-id="24746-135">Optional.</span><span class="sxs-lookup"><span data-stu-id="24746-135">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="24746-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="24746-136">Response</span></span>

<span data-ttu-id="24746-137">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="24746-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="24746-138">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="24746-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="24746-139">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="24746-139">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

<span data-ttu-id="24746-140">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="24746-140">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="24746-141">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="24746-141">Report Refresh Date</span></span>
- <span data-ttu-id="24746-142">Empfangene Exchange-E-Mails</span><span class="sxs-lookup"><span data-stu-id="24746-142">Exchange Emails Received</span></span>
- <span data-ttu-id="24746-143">Veröffentlichte Yammer-Nachrichten</span><span class="sxs-lookup"><span data-stu-id="24746-143">Yammer Messages Posted</span></span>
- <span data-ttu-id="24746-144">Gelesene Yammer-Nachrichten</span><span class="sxs-lookup"><span data-stu-id="24746-144">Yammer Messages Read</span></span>
- <span data-ttu-id="24746-145">Gelikte Yammer-Nachrichten</span><span class="sxs-lookup"><span data-stu-id="24746-145">Yammer Messages Liked</span></span>
- <span data-ttu-id="24746-146">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="24746-146">Report Date</span></span>
- <span data-ttu-id="24746-147">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="24746-147">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="24746-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="24746-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="24746-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="24746-149">Request</span></span>

<span data-ttu-id="24746-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="24746-150">The following is an example of making the request in ASP.NET that uses the TokenHelper file:</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitycounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365GroupsActivityCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="24746-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="24746-151">Response</span></span>

<span data-ttu-id="24746-152">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="24746-152">Here is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="24746-153">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="24746-153">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Exchange Emails Received,Yammer Messages Posted,Yammer Messages Read,Yammer Messages Liked,Report Date,Report Period
```
