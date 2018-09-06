# <a name="reportroot-getyammerdeviceusagedistributionusercounts"></a><span data-ttu-id="d22d4-101">reportRoot: getYammerDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="d22d4-101">reportRoot: getYammerDeviceUsageDistributionUserCounts</span></span>

<span data-ttu-id="d22d4-102">Erhalten Sie die Anzahl der Benutzer nach Gerätetyp.</span><span class="sxs-lookup"><span data-stu-id="d22d4-102">Get the number of users by device type.</span></span>

> <span data-ttu-id="d22d4-103">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Yammer-Gerätenutzung](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="d22d4-103">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="d22d4-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d22d4-104">Permissions</span></span>

<span data-ttu-id="d22d4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d22d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="d22d4-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d22d4-107">Permission type</span></span>                        | <span data-ttu-id="d22d4-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d22d4-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="d22d4-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d22d4-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="d22d4-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d22d4-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="d22d4-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d22d4-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d22d4-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d22d4-112">Not supported.</span></span>                           |
| <span data-ttu-id="d22d4-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d22d4-113">Application</span></span>                            | <span data-ttu-id="d22d4-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d22d4-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="d22d4-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d22d4-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="d22d4-116">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="d22d4-116">Function parameters</span></span>

<span data-ttu-id="d22d4-117">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="d22d4-117">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="d22d4-118">Parameter</span><span class="sxs-lookup"><span data-stu-id="d22d4-118">Parameter</span></span> | <span data-ttu-id="d22d4-119">Typ</span><span class="sxs-lookup"><span data-stu-id="d22d4-119">Type</span></span>   | <span data-ttu-id="d22d4-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d22d4-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="d22d4-121">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="d22d4-121">period</span></span>    | <span data-ttu-id="d22d4-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d22d4-122">string</span></span> | <span data-ttu-id="d22d4-123">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="d22d4-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="d22d4-124">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="d22d4-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="d22d4-125">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="d22d4-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="d22d4-126">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d22d4-126">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="d22d4-127">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d22d4-127">Request headers</span></span>

| <span data-ttu-id="d22d4-128">Name</span><span class="sxs-lookup"><span data-stu-id="d22d4-128">Name</span></span>          | <span data-ttu-id="d22d4-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d22d4-129">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="d22d4-130">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="d22d4-130">Authorization</span></span> | <span data-ttu-id="d22d4-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d22d4-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="d22d4-133">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="d22d4-133">If-None-Match</span></span> | <span data-ttu-id="d22d4-134">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d22d4-134">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="d22d4-135">Optional.</span><span class="sxs-lookup"><span data-stu-id="d22d4-135">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="d22d4-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="d22d4-136">Response</span></span>

<span data-ttu-id="d22d4-137">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="d22d4-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="d22d4-138">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d22d4-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="d22d4-139">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="d22d4-139">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="d22d4-140">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="d22d4-140">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="d22d4-141">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="d22d4-141">Report Refresh Date</span></span>
- <span data-ttu-id="d22d4-142">Web</span><span class="sxs-lookup"><span data-stu-id="d22d4-142">Web</span></span>
- <span data-ttu-id="d22d4-143">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="d22d4-143">Windows Phone</span></span>
- <span data-ttu-id="d22d4-144">Android-Smartphone</span><span class="sxs-lookup"><span data-stu-id="d22d4-144">Android Phone</span></span>
- <span data-ttu-id="d22d4-145">iPhone</span><span class="sxs-lookup"><span data-stu-id="d22d4-145">iPhone</span></span>
- <span data-ttu-id="d22d4-146">iPad</span><span class="sxs-lookup"><span data-stu-id="d22d4-146">iPad</span></span>
- <span data-ttu-id="d22d4-147">Sonstiges</span><span class="sxs-lookup"><span data-stu-id="d22d4-147">Other</span></span>
- <span data-ttu-id="d22d4-148">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="d22d4-148">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="d22d4-149">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d22d4-149">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d22d4-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d22d4-150">Request</span></span>

<span data-ttu-id="d22d4-151">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d22d4-151">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammerdeviceusagedistributionusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerDeviceUsageDistributionUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="d22d4-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="d22d4-152">Response</span></span>

<span data-ttu-id="d22d4-153">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d22d4-153">The following is an example of the response.</span></span>

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

<span data-ttu-id="d22d4-154">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="d22d4-154">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iPhone,iPad,Other,Report Period
```
