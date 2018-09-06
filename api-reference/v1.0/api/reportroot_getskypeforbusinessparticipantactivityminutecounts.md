# <a name="reportroot-getskypeforbusinessparticipantactivityminutecounts"></a><span data-ttu-id="86c86-101">reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="86c86-101">reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts</span></span>

<span data-ttu-id="86c86-102">Erhalten Sie einen Überblick über die Dauer in Minuten und die Art von Konferenzsitzungen, an denen Benutzer aus Ihrer Organisation teilgenommen  haben.</span><span class="sxs-lookup"><span data-stu-id="86c86-102">Get usage trends on the length in minutes and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="86c86-103">Zu den Arten von Konferenzsitzungen gehören Audio/Video.</span><span class="sxs-lookup"><span data-stu-id="86c86-103">Types of conference sessions include audio/video.</span></span>

> <span data-ttu-id="86c86-104">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Skype for Business-Konferenzteilnehmeraktivität](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span><span class="sxs-lookup"><span data-stu-id="86c86-104">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="permissions"></a><span data-ttu-id="86c86-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="86c86-105">Permissions</span></span>

<span data-ttu-id="86c86-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="86c86-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="86c86-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="86c86-108">Permission type</span></span>                        | <span data-ttu-id="86c86-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="86c86-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="86c86-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="86c86-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="86c86-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="86c86-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="86c86-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="86c86-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86c86-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="86c86-113">Not supported.</span></span>                           |
| <span data-ttu-id="86c86-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="86c86-114">Application</span></span>                            | <span data-ttu-id="86c86-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="86c86-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="86c86-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="86c86-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessParticipantActivityMinuteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="86c86-117">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="86c86-117">Function parameters</span></span>

<span data-ttu-id="86c86-118">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="86c86-118">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="86c86-119">Parameter</span><span class="sxs-lookup"><span data-stu-id="86c86-119">Parameter</span></span> | <span data-ttu-id="86c86-120">Typ</span><span class="sxs-lookup"><span data-stu-id="86c86-120">Type</span></span>   | <span data-ttu-id="86c86-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="86c86-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="86c86-122">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="86c86-122">period</span></span>    | <span data-ttu-id="86c86-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="86c86-123">string</span></span> | <span data-ttu-id="86c86-124">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="86c86-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="86c86-125">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="86c86-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="86c86-126">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="86c86-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="86c86-127">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="86c86-127">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="86c86-128">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="86c86-128">Request headers</span></span>

| <span data-ttu-id="86c86-129">Name</span><span class="sxs-lookup"><span data-stu-id="86c86-129">Name</span></span>          | <span data-ttu-id="86c86-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="86c86-130">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="86c86-131">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="86c86-131">Authorization</span></span> | <span data-ttu-id="86c86-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="86c86-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="86c86-134">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="86c86-134">If-None-Match</span></span> | <span data-ttu-id="86c86-135">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="86c86-135">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="86c86-136">Optional.</span><span class="sxs-lookup"><span data-stu-id="86c86-136">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="86c86-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="86c86-137">Response</span></span>

<span data-ttu-id="86c86-138">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="86c86-138">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="86c86-139">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="86c86-139">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="86c86-140">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="86c86-140">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="86c86-141">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="86c86-141">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="86c86-142">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="86c86-142">Report Refresh Date</span></span>
- <span data-ttu-id="86c86-143">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="86c86-143">Report Date</span></span>
- <span data-ttu-id="86c86-144">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="86c86-144">Report Period</span></span>
- <span data-ttu-id="86c86-145">Audio/Video</span><span class="sxs-lookup"><span data-stu-id="86c86-145">Audio/Video</span></span>

## <a name="example"></a><span data-ttu-id="86c86-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="86c86-146">Example</span></span>

#### <a name="request"></a><span data-ttu-id="86c86-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="86c86-147">Request</span></span>

<span data-ttu-id="86c86-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="86c86-148">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessparticipantactivityminutecounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessParticipantActivityMinuteCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="86c86-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="86c86-149">Response</span></span>

<span data-ttu-id="86c86-150">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="86c86-150">The following is an example of the response.</span></span>

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

<span data-ttu-id="86c86-151">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="86c86-151">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Audio/Video
```
