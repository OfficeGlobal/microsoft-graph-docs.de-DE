# <a name="reportroot-getskypeforbusinesspeertopeeractivityusercounts"></a><span data-ttu-id="c5600-101">reportRoot: getSkypeForBusinessPeerToPeerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="c5600-101">reportRoot: getSkypeForBusinessPeerToPeerActivityUserCounts</span></span>

<span data-ttu-id="c5600-102">Erhalten Sie Informationen über die Anzahl der eindeutigen Benutzer und die Art der in Ihrem Unternehmen gehaltenen Peer-to-Peer-Sitzungen.</span><span class="sxs-lookup"><span data-stu-id="c5600-102">Get usage trends on the number of unique users and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="c5600-103">Zu den Sitzungsarten gehören Chat, Audio, Video, Anwendungsfreigabe und Dateiübertragung in Peer-to-Peer-Sitzungen.</span><span class="sxs-lookup"><span data-stu-id="c5600-103">Types of sessions include IM, audio, video, application sharing, and file transfers in peer-to-peer sessions.</span></span>

> <span data-ttu-id="c5600-104">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Skype for Business-Peer-to-Peer-Aktivität](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span><span class="sxs-lookup"><span data-stu-id="c5600-104">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="permissions"></a><span data-ttu-id="c5600-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c5600-105">Permissions</span></span>

<span data-ttu-id="c5600-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c5600-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="c5600-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c5600-108">Permission type</span></span>                        | <span data-ttu-id="c5600-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c5600-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="c5600-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c5600-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c5600-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c5600-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="c5600-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c5600-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5600-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c5600-113">Not supported.</span></span>                           |
| <span data-ttu-id="c5600-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c5600-114">Application</span></span>                            | <span data-ttu-id="c5600-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c5600-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="c5600-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c5600-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessPeerToPeerActivityUserCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="c5600-117">Anforderungsparameter</span><span class="sxs-lookup"><span data-stu-id="c5600-117">Request parameters</span></span>

<span data-ttu-id="c5600-118">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="c5600-118">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="c5600-119">Parameter</span><span class="sxs-lookup"><span data-stu-id="c5600-119">Parameter</span></span> | <span data-ttu-id="c5600-120">Typ</span><span class="sxs-lookup"><span data-stu-id="c5600-120">Type</span></span>   | <span data-ttu-id="c5600-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c5600-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="c5600-122">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="c5600-122">period</span></span>    | <span data-ttu-id="c5600-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c5600-123">string</span></span> | <span data-ttu-id="c5600-124">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="c5600-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="c5600-125">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="c5600-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="c5600-126">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="c5600-126">These values follow the format D   where    represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="c5600-127">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="c5600-127">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="c5600-128">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c5600-128">Request headers</span></span>

| <span data-ttu-id="c5600-129">Name</span><span class="sxs-lookup"><span data-stu-id="c5600-129">Name</span></span>          | <span data-ttu-id="c5600-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c5600-130">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="c5600-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5600-131">Authorization</span></span> | <span data-ttu-id="c5600-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c5600-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="c5600-134">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="c5600-134">If-None-Match</span></span> | <span data-ttu-id="c5600-135">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c5600-135">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="c5600-136">Optional.</span><span class="sxs-lookup"><span data-stu-id="c5600-136">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="c5600-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="c5600-137">Response</span></span>

<span data-ttu-id="c5600-138">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="c5600-138">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="c5600-139">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c5600-139">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="c5600-140">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="c5600-140">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="c5600-141">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="c5600-141">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="c5600-142">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="c5600-142">Report Refresh Date</span></span>
- <span data-ttu-id="c5600-143">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="c5600-143">Report Date</span></span>
- <span data-ttu-id="c5600-144">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="c5600-144">Report Period</span></span>
- <span data-ttu-id="c5600-145">Chat</span><span class="sxs-lookup"><span data-stu-id="c5600-145">IM</span></span>
- <span data-ttu-id="c5600-146">Audio</span><span class="sxs-lookup"><span data-stu-id="c5600-146">Audio</span></span>
- <span data-ttu-id="c5600-147">Video</span><span class="sxs-lookup"><span data-stu-id="c5600-147">Video</span></span>
- <span data-ttu-id="c5600-148">Gemeinsame Nutzung von Anwendungen</span><span class="sxs-lookup"><span data-stu-id="c5600-148">App Sharing</span></span>
- <span data-ttu-id="c5600-149">Dateiübertragung</span><span class="sxs-lookup"><span data-stu-id="c5600-149">File Transfer</span></span>

## <a name="example"></a><span data-ttu-id="c5600-150">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c5600-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="c5600-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c5600-151">Request</span></span>

<span data-ttu-id="c5600-152">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c5600-152">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinesspeertopeeractivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessPeerToPeerActivityUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="c5600-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="c5600-153">Response</span></span>

<span data-ttu-id="c5600-154">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c5600-154">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="c5600-155">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="c5600-155">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio,Video,App Sharing,File Transfer
```
