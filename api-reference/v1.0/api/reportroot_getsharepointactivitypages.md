# <a name="reportroot-getsharepointactivitypages"></a><span data-ttu-id="a34b2-101">reportRoot: getSharePointActivityPages</span><span class="sxs-lookup"><span data-stu-id="a34b2-101">reportRoot: getSharePointActivityPages</span></span>

<span data-ttu-id="a34b2-102">Rufen Sie die Anzahl der von Benutzern besuchten eindeutigen Seiten ab.</span><span class="sxs-lookup"><span data-stu-id="a34b2-102">Get the number of unique pages visited by users.</span></span>

> <span data-ttu-id="a34b2-103">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – SharePoint-Aktivität]((https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)).</span><span class="sxs-lookup"><span data-stu-id="a34b2-103">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity]((https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)).</span></span>

## <a name="permissions"></a><span data-ttu-id="a34b2-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a34b2-104">Permissions</span></span>

<span data-ttu-id="a34b2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a34b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="a34b2-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a34b2-107">Permission type</span></span>                        | <span data-ttu-id="a34b2-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a34b2-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="a34b2-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a34b2-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="a34b2-110">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a34b2-110">Not supported.</span></span>                           |
| <span data-ttu-id="a34b2-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a34b2-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a34b2-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a34b2-112">Not supported.</span></span>                           |
| <span data-ttu-id="a34b2-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a34b2-113">Application</span></span>                            | <span data-ttu-id="a34b2-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a34b2-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="a34b2-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a34b2-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityPages(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="a34b2-116">Anforderungsparameter</span><span class="sxs-lookup"><span data-stu-id="a34b2-116">Request parameters</span></span>

<span data-ttu-id="a34b2-117">Stellen Sie in der URL der Anforderung die folgenden Abfrageparameter mit einem gültigen Wert bereit.</span><span class="sxs-lookup"><span data-stu-id="a34b2-117">In the request URL, provide the following query parameter with a valid value.</span></span>

| <span data-ttu-id="a34b2-118">Parameter</span><span class="sxs-lookup"><span data-stu-id="a34b2-118">Parameter</span></span> | <span data-ttu-id="a34b2-119">Typ</span><span class="sxs-lookup"><span data-stu-id="a34b2-119">Type</span></span>   | <span data-ttu-id="a34b2-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a34b2-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="a34b2-121">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="a34b2-121">Period</span></span>    | <span data-ttu-id="a34b2-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a34b2-122">string</span></span> | <span data-ttu-id="a34b2-123">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="a34b2-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="a34b2-124">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="a34b2-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="a34b2-125">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="a34b2-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="a34b2-126">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a34b2-126">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="a34b2-127">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a34b2-127">Request headers</span></span>

| <span data-ttu-id="a34b2-128">Name</span><span class="sxs-lookup"><span data-stu-id="a34b2-128">Name</span></span>          | <span data-ttu-id="a34b2-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a34b2-129">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="a34b2-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="a34b2-130">Authorization</span></span> | <span data-ttu-id="a34b2-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a34b2-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a34b2-133">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="a34b2-133">if-none-match</span></span> | <span data-ttu-id="a34b2-134">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a34b2-134">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `304 Not Modified` response is returned.</span></span> <span data-ttu-id="a34b2-135">Optional.</span><span class="sxs-lookup"><span data-stu-id="a34b2-135">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="a34b2-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="a34b2-136">Response</span></span>

<span data-ttu-id="a34b2-137">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="a34b2-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="a34b2-138">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a34b2-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="a34b2-139">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="a34b2-139">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

<span data-ttu-id="a34b2-140">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="a34b2-140">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="a34b2-141">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="a34b2-141">Report Refresh Date</span></span>
- <span data-ttu-id="a34b2-142">Anzahl der besuchten Seite</span><span class="sxs-lookup"><span data-stu-id="a34b2-142">Visited Page Count</span></span>
- <span data-ttu-id="a34b2-143">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="a34b2-143">Report Date</span></span>
- <span data-ttu-id="a34b2-144">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="a34b2-144">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="a34b2-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a34b2-145">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a34b2-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a34b2-146">Request</span></span>

<span data-ttu-id="a34b2-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a34b2-147">The following is an example of making the request in ASP.NET that uses the TokenHelper file:</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivitypages"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointActivityPages(period='D7')
```

#### <a name="response"></a><span data-ttu-id="a34b2-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="a34b2-148">Response</span></span>

<span data-ttu-id="a34b2-149">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a34b2-149">Here is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="a34b2-150">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="a34b2-150">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Visited Page Count,Report Date,Report Period
```
