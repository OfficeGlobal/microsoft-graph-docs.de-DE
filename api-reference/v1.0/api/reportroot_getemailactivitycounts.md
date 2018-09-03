# <a name="reportroot-getemailactivitycounts"></a><span data-ttu-id="046af-101">reportRoot: getEmailActivityCounts</span><span class="sxs-lookup"><span data-stu-id="046af-101">reportRoot: getEmailActivityCounts</span></span>

<span data-ttu-id="046af-102">Ermöglicht es Ihnen, einen Überblick über die E-Mail-Aktivitäten (z. B. wie viele E-Mails versendet, gelesen und empfangen wurden) in Ihrer Organisation zu gewinnen.</span><span class="sxs-lookup"><span data-stu-id="046af-102">Enables you to understand the trends of email activity (like how many were sent, read, and received) in your organization.</span></span>

> <span data-ttu-id="046af-103">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – E-Mail-Aktivität](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span><span class="sxs-lookup"><span data-stu-id="046af-103">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="permissions"></a><span data-ttu-id="046af-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="046af-104">Permissions</span></span>

<span data-ttu-id="046af-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="046af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="046af-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="046af-107">Permission type</span></span>                        | <span data-ttu-id="046af-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="046af-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="046af-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="046af-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="046af-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="046af-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="046af-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="046af-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="046af-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="046af-112">Not supported.</span></span>                           |
| <span data-ttu-id="046af-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="046af-113">Application</span></span>                            | <span data-ttu-id="046af-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="046af-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="046af-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="046af-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="046af-116">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="046af-116">Function parameters</span></span>

<span data-ttu-id="046af-117">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="046af-117">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="046af-118">Parameter</span><span class="sxs-lookup"><span data-stu-id="046af-118">Parameter</span></span> | <span data-ttu-id="046af-119">Typ</span><span class="sxs-lookup"><span data-stu-id="046af-119">Type</span></span>   | <span data-ttu-id="046af-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="046af-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="046af-121">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="046af-121">period</span></span>    | <span data-ttu-id="046af-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="046af-122">string</span></span> | <span data-ttu-id="046af-123">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="046af-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="046af-124">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="046af-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="046af-125">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="046af-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="046af-126">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="046af-126">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="046af-127">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="046af-127">Request headers</span></span>

| <span data-ttu-id="046af-128">Name</span><span class="sxs-lookup"><span data-stu-id="046af-128">Name</span></span>          | <span data-ttu-id="046af-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="046af-129">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="046af-130">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="046af-130">Authorization</span></span> | <span data-ttu-id="046af-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="046af-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="046af-133">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="046af-133">If-None-Match</span></span> | <span data-ttu-id="046af-134">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="046af-134">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="046af-135">Optional.</span><span class="sxs-lookup"><span data-stu-id="046af-135">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="046af-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="046af-136">Response</span></span>

<span data-ttu-id="046af-137">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="046af-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="046af-138">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="046af-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="046af-139">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="046af-139">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="046af-140">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="046af-140">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="046af-141">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="046af-141">Report Refresh Date</span></span>
- <span data-ttu-id="046af-142">Senden</span><span class="sxs-lookup"><span data-stu-id="046af-142">Send</span></span>
- <span data-ttu-id="046af-143">Empfangen</span><span class="sxs-lookup"><span data-stu-id="046af-143">Receive</span></span>
- <span data-ttu-id="046af-144">Lesen</span><span class="sxs-lookup"><span data-stu-id="046af-144">Read</span></span>
- <span data-ttu-id="046af-145">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="046af-145">Report Date</span></span>
- <span data-ttu-id="046af-146">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="046af-146">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="046af-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="046af-147">Example</span></span>

#### <a name="request"></a><span data-ttu-id="046af-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="046af-148">Request</span></span>

<span data-ttu-id="046af-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="046af-149">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getemailactivitycounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getEmailActivityCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="046af-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="046af-150">Response</span></span>

<span data-ttu-id="046af-151">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="046af-151">The following is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.report" } --> 

```http
HTTP/1.1 302 Found
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="046af-152">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="046af-152">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "ignored"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Send,Receive,Read,Report Date,Report Period
```
