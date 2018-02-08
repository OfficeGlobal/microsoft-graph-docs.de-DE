# <a name="reportroot-getskypeforbusinesspeertopeeractivityminutecounts"></a><span data-ttu-id="53260-101">reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="53260-101">reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts</span></span>

<span data-ttu-id="53260-102">Erhalten Sie Informationen über die Dauer (in Minuten) und die Art der in Ihrem Unternehmen gehaltenen Peer-to-Peer-Sitzungen.</span><span class="sxs-lookup"><span data-stu-id="53260-102">Get usage trends on the length in minutes and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="53260-103">Zu den Sitzungsarten gehören Audio und Video.</span><span class="sxs-lookup"><span data-stu-id="53260-103">Types of sessions include audio and video.</span></span>

> <span data-ttu-id="53260-104">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Skype for Business-Peer-to-Peer-Aktivität](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span><span class="sxs-lookup"><span data-stu-id="53260-104">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="permissions"></a><span data-ttu-id="53260-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="53260-105">Permissions</span></span>

<span data-ttu-id="53260-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="53260-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="53260-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="53260-108">Permission type</span></span>                        | <span data-ttu-id="53260-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="53260-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="53260-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="53260-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="53260-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="53260-111">Not supported.</span></span>                           |
| <span data-ttu-id="53260-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="53260-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53260-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="53260-113">Not supported.</span></span>                           |
| <span data-ttu-id="53260-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="53260-114">Application</span></span>                            | <span data-ttu-id="53260-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="53260-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="53260-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="53260-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="53260-117">Anforderungsparameter</span><span class="sxs-lookup"><span data-stu-id="53260-117">Request parameters</span></span>

<span data-ttu-id="53260-118">Stellen Sie in der URL der Anforderung den folgenden Parameter mit einem gültigen Wert bereit.</span><span class="sxs-lookup"><span data-stu-id="53260-118">In the request URL, provide the following query parameter with a valid value.</span></span>

| <span data-ttu-id="53260-119">Parameter</span><span class="sxs-lookup"><span data-stu-id="53260-119">Parameter</span></span> | <span data-ttu-id="53260-120">Typ</span><span class="sxs-lookup"><span data-stu-id="53260-120">Type</span></span>   | <span data-ttu-id="53260-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="53260-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="53260-122">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="53260-122">period</span></span>    | <span data-ttu-id="53260-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="53260-123">string</span></span> | <span data-ttu-id="53260-124">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="53260-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="53260-125">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="53260-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="53260-126">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="53260-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="53260-127">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="53260-127">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="53260-128">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="53260-128">Request headers</span></span>

| <span data-ttu-id="53260-129">Name</span><span class="sxs-lookup"><span data-stu-id="53260-129">Name</span></span>          | <span data-ttu-id="53260-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="53260-130">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="53260-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="53260-131">Authorization</span></span> | <span data-ttu-id="53260-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="53260-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="53260-134">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="53260-134">If-None-Match</span></span> | <span data-ttu-id="53260-135">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="53260-135">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="53260-136">Optional.</span><span class="sxs-lookup"><span data-stu-id="53260-136">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="53260-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="53260-137">Response</span></span>

<span data-ttu-id="53260-138">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="53260-138">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="53260-139">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="53260-139">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="53260-140">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="53260-140">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="53260-141">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="53260-141">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="53260-142">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="53260-142">Report Refresh Date</span></span>
- <span data-ttu-id="53260-143">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="53260-143">Report Date</span></span>
- <span data-ttu-id="53260-144">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="53260-144">Report Period</span></span>
- <span data-ttu-id="53260-145">Audio</span><span class="sxs-lookup"><span data-stu-id="53260-145">Audio</span></span>
- <span data-ttu-id="53260-146">Video</span><span class="sxs-lookup"><span data-stu-id="53260-146">Video</span></span>

## <a name="example"></a><span data-ttu-id="53260-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="53260-147">Example</span></span>

#### <a name="request"></a><span data-ttu-id="53260-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="53260-148">Request</span></span>

<span data-ttu-id="53260-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="53260-149">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinesspeertopeeractivityminutecounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="53260-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="53260-150">Response</span></span>

<span data-ttu-id="53260-151">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="53260-151">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="53260-152">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="53260-152">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Audio,Video
```
