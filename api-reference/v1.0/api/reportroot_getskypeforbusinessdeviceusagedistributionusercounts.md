# <a name="reportroot-getskypeforbusinessdeviceusagedistributionusercounts"></a><span data-ttu-id="74de5-101">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="74de5-101">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span></span>

<span data-ttu-id="74de5-102">Rufen Sie die Anzahl der Benutzer ab, die eigene Geräte in Ihrer Organisation verwenden.</span><span class="sxs-lookup"><span data-stu-id="74de5-102">Get the number of users using unique devices in your organization.</span></span> <span data-ttu-id="74de5-103">Der Bericht enthält die Anzahl der Benutzer pro Gerät, einschließlich Windows, Windows Phone, Android-Smartphone, iPhone und iPad.</span><span class="sxs-lookup"><span data-stu-id="74de5-103">The report will show you the number of users per device including Windows, Windows phone, Android phone, iPhone, and iPad.</span></span>

> <span data-ttu-id="74de5-104">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Verwendete Skype for Business-Clients]((https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3)).</span><span class="sxs-lookup"><span data-stu-id="74de5-104">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used]((https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3)).</span></span>

## <a name="permissions"></a><span data-ttu-id="74de5-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="74de5-105">Permissions</span></span>

<span data-ttu-id="74de5-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="74de5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="74de5-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="74de5-108">Permission type</span></span>                        | <span data-ttu-id="74de5-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="74de5-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="74de5-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="74de5-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="74de5-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="74de5-111">Not supported.</span></span>                           |
| <span data-ttu-id="74de5-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="74de5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74de5-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="74de5-113">Not supported.</span></span>                           |
| <span data-ttu-id="74de5-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="74de5-114">Application</span></span>                            | <span data-ttu-id="74de5-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="74de5-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="74de5-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="74de5-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="74de5-117">Anforderungsparameter</span><span class="sxs-lookup"><span data-stu-id="74de5-117">Request parameters</span></span>

<span data-ttu-id="74de5-118">Stellen Sie in der URL der Anforderung die folgenden Abfrageparameter mit einem gültigen Wert bereit.</span><span class="sxs-lookup"><span data-stu-id="74de5-118">In the request URL, provide the following query parameter with a valid value.</span></span>

| <span data-ttu-id="74de5-119">Parameter</span><span class="sxs-lookup"><span data-stu-id="74de5-119">Parameter</span></span> | <span data-ttu-id="74de5-120">Typ</span><span class="sxs-lookup"><span data-stu-id="74de5-120">Type</span></span>   | <span data-ttu-id="74de5-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="74de5-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="74de5-122">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="74de5-122">Period</span></span>    | <span data-ttu-id="74de5-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="74de5-123">string</span></span> | <span data-ttu-id="74de5-124">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="74de5-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="74de5-125">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="74de5-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="74de5-126">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="74de5-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="74de5-127">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="74de5-127">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="74de5-128">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="74de5-128">Request headers</span></span>

| <span data-ttu-id="74de5-129">Name</span><span class="sxs-lookup"><span data-stu-id="74de5-129">Name</span></span>          | <span data-ttu-id="74de5-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="74de5-130">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="74de5-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="74de5-131">Authorization</span></span> | <span data-ttu-id="74de5-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="74de5-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="74de5-134">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="74de5-134">if-none-match</span></span> | <span data-ttu-id="74de5-135">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="74de5-135">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `304 Not Modified` response is returned.</span></span> <span data-ttu-id="74de5-136">Optional.</span><span class="sxs-lookup"><span data-stu-id="74de5-136">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="74de5-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="74de5-137">Response</span></span>

<span data-ttu-id="74de5-138">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="74de5-138">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="74de5-139">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="74de5-139">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="74de5-140">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="74de5-140">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

<span data-ttu-id="74de5-141">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="74de5-141">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="74de5-142">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="74de5-142">Report Refresh Date</span></span>
- <span data-ttu-id="74de5-143">Windows</span><span class="sxs-lookup"><span data-stu-id="74de5-143">Windows</span></span>
- <span data-ttu-id="74de5-144">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="74de5-144">Windows Phone</span></span>
- <span data-ttu-id="74de5-145">Android-Smartphone</span><span class="sxs-lookup"><span data-stu-id="74de5-145">Office for Android Phone</span></span>
- <span data-ttu-id="74de5-146">iPhone</span><span class="sxs-lookup"><span data-stu-id="74de5-146">iPhone</span></span>
- <span data-ttu-id="74de5-147">iPad</span><span class="sxs-lookup"><span data-stu-id="74de5-147">iPad</span></span>
- <span data-ttu-id="74de5-148">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="74de5-148">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="74de5-149">Beispiel</span><span class="sxs-lookup"><span data-stu-id="74de5-149">Example</span></span>

#### <a name="request"></a><span data-ttu-id="74de5-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="74de5-150">Request</span></span>

<span data-ttu-id="74de5-151">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="74de5-151">The following is an example of making the request in ASP.NET that uses the TokenHelper file:</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusagedistributionusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="74de5-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="74de5-152">Response</span></span>

<span data-ttu-id="74de5-153">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="74de5-153">Here is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="74de5-154">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="74de5-154">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Windows,Windows Phone,Android Phone,iPhone,iPad,Report Period
```
