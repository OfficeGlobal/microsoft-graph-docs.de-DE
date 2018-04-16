# <a name="reportroot-getteamsdeviceusagedistributionusercounts"></a><span data-ttu-id="b4943-101">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="b4943-101">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span></span>

<span data-ttu-id="b4943-102">Abrufen der Anzahl der täglichen eindeutigen Benutzer des Microsoft Teams nach Gerätetyp im ausgewählten Zeitraum.</span><span class="sxs-lookup"><span data-stu-id="b4943-102">Get the number of Microsoft Teams unique users by device type over the selected time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="b4943-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b4943-103">Permissions</span></span>

<span data-ttu-id="b4943-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b4943-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="b4943-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b4943-106">Permission type</span></span>                        | <span data-ttu-id="b4943-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b4943-107">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b4943-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b4943-108">Delegated (work or school account)</span></span>     | <span data-ttu-id="b4943-109">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b4943-109">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b4943-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b4943-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4943-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b4943-111">Not supported.</span></span>                           |
| <span data-ttu-id="b4943-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b4943-112">Application</span></span>                            | <span data-ttu-id="b4943-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b4943-113">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="b4943-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b4943-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="b4943-115">Anforderungsparameter</span><span class="sxs-lookup"><span data-stu-id="b4943-115">Request parameters</span></span>

<span data-ttu-id="b4943-116">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="b4943-116">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="b4943-117">Parameter</span><span class="sxs-lookup"><span data-stu-id="b4943-117">Parameter</span></span> | <span data-ttu-id="b4943-118">Typ</span><span class="sxs-lookup"><span data-stu-id="b4943-118">Type</span></span>   | <span data-ttu-id="b4943-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b4943-119">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="b4943-120">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="b4943-120">period</span></span>    | <span data-ttu-id="b4943-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4943-121">string</span></span> | <span data-ttu-id="b4943-122">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="b4943-122">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="b4943-123">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="b4943-123">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="b4943-124">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="b4943-124">These values follow the format D   where    represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="b4943-125">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="b4943-125">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="b4943-126">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b4943-126">Request headers</span></span>

| <span data-ttu-id="b4943-127">Name</span><span class="sxs-lookup"><span data-stu-id="b4943-127">Name</span></span>          | <span data-ttu-id="b4943-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b4943-128">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="b4943-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4943-129">Authorization</span></span> | <span data-ttu-id="b4943-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b4943-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="b4943-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="b4943-132">Response</span></span>

<span data-ttu-id="b4943-133">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="b4943-133">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b4943-134">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b4943-134">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b4943-135">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="b4943-135">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b4943-136">Die CSV-Datei verfügt über die folgenden Spaltenheader:</span><span class="sxs-lookup"><span data-stu-id="b4943-136">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="b4943-137">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="b4943-137">Report Refresh Date</span></span>
- <span data-ttu-id="b4943-138">Web</span><span class="sxs-lookup"><span data-stu-id="b4943-138">Web</span></span>
- <span data-ttu-id="b4943-139">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="b4943-139">Windows Phone</span></span>
- <span data-ttu-id="b4943-140">Android-Smartphone</span><span class="sxs-lookup"><span data-stu-id="b4943-140">Android Phone</span></span>
- <span data-ttu-id="b4943-141">iOS</span><span class="sxs-lookup"><span data-stu-id="b4943-141">iOS</span></span>
- <span data-ttu-id="b4943-142">Mac</span><span class="sxs-lookup"><span data-stu-id="b4943-142">Mac</span></span>
- <span data-ttu-id="b4943-143">Windows</span><span class="sxs-lookup"><span data-stu-id="b4943-143">Windows</span></span>
- <span data-ttu-id="b4943-144">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="b4943-144">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="b4943-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b4943-145">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b4943-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b4943-146">Request</span></span>

<span data-ttu-id="b4943-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b4943-147">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="b4943-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="b4943-148">Response</span></span>

<span data-ttu-id="b4943-149">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b4943-149">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="b4943-150">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="b4943-150">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iOS,Mac,Windows,Report Period
```
