# <a name="reportroot-getyammeractivityusercounts"></a><span data-ttu-id="9ea99-101">reportRoot: getYammerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="9ea99-101">reportRoot: getYammerActivityUserCounts</span></span>

<span data-ttu-id="9ea99-102">Erfahren Sie, wie viele eindeutige Benutzer Yammer-Nachrichten veröffentlicht, gelesen und gelikt haben.</span><span class="sxs-lookup"><span data-stu-id="9ea99-102">Get the trends on the number of unique users who posted, read, and liked Yammer messages.</span></span>

> <span data-ttu-id="9ea99-103">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Yammer-Aktivität]((https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a)).</span><span class="sxs-lookup"><span data-stu-id="9ea99-103">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity]((https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a)).</span></span>

## <a name="permissions"></a><span data-ttu-id="9ea99-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9ea99-104">Permissions</span></span>

<span data-ttu-id="9ea99-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9ea99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="9ea99-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9ea99-107">Permission type</span></span>                        | <span data-ttu-id="9ea99-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9ea99-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="9ea99-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9ea99-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="9ea99-110">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9ea99-110">Not supported.</span></span>                           |
| <span data-ttu-id="9ea99-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9ea99-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ea99-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9ea99-112">Not supported.</span></span>                           |
| <span data-ttu-id="9ea99-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9ea99-113">Application</span></span>                            | <span data-ttu-id="9ea99-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9ea99-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="9ea99-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9ea99-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerActivityUserCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="9ea99-116">Anforderungsparameter</span><span class="sxs-lookup"><span data-stu-id="9ea99-116">Request parameters</span></span>

<span data-ttu-id="9ea99-117">Stellen Sie in der URL der Anforderung die folgenden Abfrageparameter mit einem gültigen Wert bereit.</span><span class="sxs-lookup"><span data-stu-id="9ea99-117">In the request URL, provide the following query parameter with a valid value.</span></span>

| <span data-ttu-id="9ea99-118">Parameter</span><span class="sxs-lookup"><span data-stu-id="9ea99-118">Parameter</span></span> | <span data-ttu-id="9ea99-119">Typ</span><span class="sxs-lookup"><span data-stu-id="9ea99-119">Type</span></span>   | <span data-ttu-id="9ea99-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9ea99-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="9ea99-121">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="9ea99-121">Period</span></span>    | <span data-ttu-id="9ea99-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9ea99-122">string</span></span> | <span data-ttu-id="9ea99-123">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="9ea99-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="9ea99-124">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="9ea99-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="9ea99-125">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="9ea99-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="9ea99-126">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9ea99-126">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="9ea99-127">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9ea99-127">Request headers</span></span>

| <span data-ttu-id="9ea99-128">Name</span><span class="sxs-lookup"><span data-stu-id="9ea99-128">Name</span></span>          | <span data-ttu-id="9ea99-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9ea99-129">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="9ea99-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ea99-130">Authorization</span></span> | <span data-ttu-id="9ea99-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9ea99-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9ea99-133">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="9ea99-133">if-none-match</span></span> | <span data-ttu-id="9ea99-134">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9ea99-134">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `304 Not Modified` response is returned.</span></span> <span data-ttu-id="9ea99-135">Optional.</span><span class="sxs-lookup"><span data-stu-id="9ea99-135">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="9ea99-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="9ea99-136">Response</span></span>

<span data-ttu-id="9ea99-137">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="9ea99-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="9ea99-138">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9ea99-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="9ea99-139">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="9ea99-139">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

<span data-ttu-id="9ea99-140">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="9ea99-140">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="9ea99-141">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="9ea99-141">Report Refresh Date</span></span>
- <span data-ttu-id="9ea99-142">Gelikt</span><span class="sxs-lookup"><span data-stu-id="9ea99-142">Liked</span></span>
- <span data-ttu-id="9ea99-143">Gepostet</span><span class="sxs-lookup"><span data-stu-id="9ea99-143">Posted</span></span>
- <span data-ttu-id="9ea99-144">Gelesen</span><span class="sxs-lookup"><span data-stu-id="9ea99-144">Read</span></span>
- <span data-ttu-id="9ea99-145">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="9ea99-145">Report Date</span></span>
- <span data-ttu-id="9ea99-146">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="9ea99-146">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="9ea99-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9ea99-147">Example</span></span>

#### <a name="request"></a><span data-ttu-id="9ea99-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9ea99-148">Request</span></span>

<span data-ttu-id="9ea99-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9ea99-149">The following is an example of making the request in ASP.NET that uses the TokenHelper file:</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerActivityUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="9ea99-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="9ea99-150">Response</span></span>

<span data-ttu-id="9ea99-151">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9ea99-151">Here is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="9ea99-152">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="9ea99-152">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Liked,Posted,Read,Report Date,Report Period
```
