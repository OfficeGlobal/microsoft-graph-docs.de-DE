# <a name="reportroot-getskypeforbusinessdeviceusageusercounts"></a><span data-ttu-id="38b39-101">reportRoot: getSkypeForBusinessDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="38b39-101">reportRoot: getSkypeForBusinessDeviceUsageUserCounts</span></span>

<span data-ttu-id="38b39-102">Erfahren Sie mehr über Auslastungstrends, indem Sie sich ansehen, wie viele Benutzer in Ihrer Organisation sich über die Skype for Business-App verbunden haben.</span><span class="sxs-lookup"><span data-stu-id="38b39-102">Get the usage trends on how many users in your organization have connected using the Skype for Business app.</span></span> <span data-ttu-id="38b39-103">Außerdem erhalten Sie eine Auflistung des Gerätetyps (Windows, Windows Phone, Android-Smartphone, iPhone oder iPad) auf dem die Skype for Business-Client-App installiert und in Ihrer Organisation verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="38b39-103">You will also get a breakdown by the type of device (Windows, Windows phone, Android phone, iPhone, or iPad) on which the Skype for Business client app is installed and used across your organization.</span></span>

> <span data-ttu-id="38b39-104">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Verwendete Skype for Business-Clients](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span><span class="sxs-lookup"><span data-stu-id="38b39-104">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="38b39-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="38b39-105">Permissions</span></span>

<span data-ttu-id="38b39-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="38b39-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="38b39-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="38b39-108">Permission type</span></span>                        | <span data-ttu-id="38b39-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="38b39-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="38b39-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="38b39-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="38b39-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="38b39-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="38b39-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="38b39-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38b39-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="38b39-113">Not supported.</span></span>                           |
| <span data-ttu-id="38b39-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="38b39-114">Application</span></span>                            | <span data-ttu-id="38b39-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="38b39-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="38b39-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="38b39-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="38b39-117">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="38b39-117">Function parameters</span></span>

<span data-ttu-id="38b39-118">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="38b39-118">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="38b39-119">Parameter</span><span class="sxs-lookup"><span data-stu-id="38b39-119">Parameter</span></span> | <span data-ttu-id="38b39-120">Typ</span><span class="sxs-lookup"><span data-stu-id="38b39-120">Type</span></span>   | <span data-ttu-id="38b39-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="38b39-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="38b39-122">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="38b39-122">period</span></span>    | <span data-ttu-id="38b39-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="38b39-123">string</span></span> | <span data-ttu-id="38b39-124">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="38b39-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="38b39-125">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="38b39-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="38b39-126">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="38b39-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="38b39-127">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="38b39-127">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="38b39-128">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="38b39-128">Request headers</span></span>

| <span data-ttu-id="38b39-129">Name</span><span class="sxs-lookup"><span data-stu-id="38b39-129">Name</span></span>          | <span data-ttu-id="38b39-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="38b39-130">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="38b39-131">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="38b39-131">Authorization</span></span> | <span data-ttu-id="38b39-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="38b39-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="38b39-134">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="38b39-134">If-None-Match</span></span> | <span data-ttu-id="38b39-135">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="38b39-135">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="38b39-136">Optional.</span><span class="sxs-lookup"><span data-stu-id="38b39-136">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="38b39-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="38b39-137">Response</span></span>

<span data-ttu-id="38b39-138">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="38b39-138">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="38b39-139">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="38b39-139">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="38b39-140">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="38b39-140">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="38b39-141">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="38b39-141">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="38b39-142">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="38b39-142">Report Refresh Date</span></span>
- <span data-ttu-id="38b39-143">Windows</span><span class="sxs-lookup"><span data-stu-id="38b39-143">Windows</span></span>
- <span data-ttu-id="38b39-144">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="38b39-144">Windows Phone</span></span>
- <span data-ttu-id="38b39-145">Android-Smartphone</span><span class="sxs-lookup"><span data-stu-id="38b39-145">Android Phone</span></span>
- <span data-ttu-id="38b39-146">iPhone</span><span class="sxs-lookup"><span data-stu-id="38b39-146">iPhone</span></span>
- <span data-ttu-id="38b39-147">iPad</span><span class="sxs-lookup"><span data-stu-id="38b39-147">iPad</span></span>
- <span data-ttu-id="38b39-148">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="38b39-148">Report Date</span></span>
- <span data-ttu-id="38b39-149">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="38b39-149">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="38b39-150">Beispiel</span><span class="sxs-lookup"><span data-stu-id="38b39-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="38b39-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="38b39-151">Request</span></span>

<span data-ttu-id="38b39-152">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="38b39-152">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessdeviceusageusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessDeviceUsageUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="38b39-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="38b39-153">Response</span></span>

<span data-ttu-id="38b39-154">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="38b39-154">The following is an example of the response.</span></span>

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

<span data-ttu-id="38b39-155">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="38b39-155">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Windows,Windows Phone,Android Phone,iPhone,iPad,Report Date,Report Period
```
