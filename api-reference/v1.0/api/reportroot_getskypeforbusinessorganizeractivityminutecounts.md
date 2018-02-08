# <a name="reportroot-getskypeforbusinessorganizeractivityminutecounts"></a><span data-ttu-id="7f546-101">reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="7f546-101">reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts</span></span>

<span data-ttu-id="7f546-102">Erhalten Sie Informationen über die Dauer (in Minuten) und die Art der von Benutzern aus Ihrem Unternehmen gehaltenen und organisierten Konferenzsitzungen.</span><span class="sxs-lookup"><span data-stu-id="7f546-102">Get usage trends on the length in minutes and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="7f546-103">Arten von Konferenzsitzungen sind Audio/Video und Einwahl/Auswahl - Microsoft.</span><span class="sxs-lookup"><span data-stu-id="7f546-103">Types of conference sessions include audio/video, and dial-in and dial-out - Microsoft.</span></span>

> <span data-ttu-id="7f546-104">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Skype for Business-Konferenzorganisationsaktivität](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span><span class="sxs-lookup"><span data-stu-id="7f546-104">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span></span>

## <a name="permissions"></a><span data-ttu-id="7f546-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7f546-105">Permissions</span></span>

<span data-ttu-id="7f546-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7f546-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="7f546-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7f546-108">Permission type</span></span>                        | <span data-ttu-id="7f546-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7f546-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="7f546-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7f546-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="7f546-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7f546-111">Not supported.</span></span>                           |
| <span data-ttu-id="7f546-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7f546-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f546-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7f546-113">Not supported.</span></span>                           |
| <span data-ttu-id="7f546-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7f546-114">Application</span></span>                            | <span data-ttu-id="7f546-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f546-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="7f546-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7f546-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessOrganizerActivityMinuteCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="7f546-117">Anforderungsparameter</span><span class="sxs-lookup"><span data-stu-id="7f546-117">Request parameters</span></span>

<span data-ttu-id="7f546-118">Stellen Sie in der URL der Anforderung den folgenden Parameter mit einem gültigen Wert bereit.</span><span class="sxs-lookup"><span data-stu-id="7f546-118">In the request URL, provide the following query parameter with a valid value.</span></span>

| <span data-ttu-id="7f546-119">Parameter</span><span class="sxs-lookup"><span data-stu-id="7f546-119">Parameter</span></span> | <span data-ttu-id="7f546-120">Typ</span><span class="sxs-lookup"><span data-stu-id="7f546-120">Type</span></span>   | <span data-ttu-id="7f546-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7f546-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="7f546-122">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="7f546-122">period</span></span>    | <span data-ttu-id="7f546-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7f546-123">string</span></span> | <span data-ttu-id="7f546-124">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="7f546-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="7f546-125">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="7f546-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="7f546-126">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="7f546-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="7f546-127">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7f546-127">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="7f546-128">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7f546-128">Request headers</span></span>

| <span data-ttu-id="7f546-129">Name</span><span class="sxs-lookup"><span data-stu-id="7f546-129">Name</span></span>          | <span data-ttu-id="7f546-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7f546-130">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="7f546-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f546-131">Authorization</span></span> | <span data-ttu-id="7f546-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7f546-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7f546-134">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="7f546-134">If-None-Match</span></span> | <span data-ttu-id="7f546-135">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7f546-135">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="7f546-136">Optional.</span><span class="sxs-lookup"><span data-stu-id="7f546-136">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="7f546-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="7f546-137">Response</span></span>

<span data-ttu-id="7f546-138">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="7f546-138">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="7f546-139">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7f546-139">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="7f546-140">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="7f546-140">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="7f546-141">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="7f546-141">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="7f546-142">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="7f546-142">Report Refresh Date</span></span>
- <span data-ttu-id="7f546-143">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="7f546-143">Report Date</span></span>
- <span data-ttu-id="7f546-144">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="7f546-144">Report Period</span></span>
- <span data-ttu-id="7f546-145">Audio/Video</span><span class="sxs-lookup"><span data-stu-id="7f546-145">Audio/Video</span></span>
- <span data-ttu-id="7f546-146">Einwahl von Microsoft</span><span class="sxs-lookup"><span data-stu-id="7f546-146">Dial-in Microsoft</span></span>
- <span data-ttu-id="7f546-147">Auswahl von Microsoft</span><span class="sxs-lookup"><span data-stu-id="7f546-147">Dial-out Microsoft</span></span>

## <a name="example"></a><span data-ttu-id="7f546-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7f546-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="7f546-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7f546-149">Request</span></span>

<span data-ttu-id="7f546-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7f546-150">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessorganizeractivityminutecounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessOrganizerActivityMinuteCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="7f546-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="7f546-151">Response</span></span>

<span data-ttu-id="7f546-152">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7f546-152">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="7f546-153">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="7f546-153">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Audio/Video,Dial-in Microsoft,Dial-out Microsoft
```
