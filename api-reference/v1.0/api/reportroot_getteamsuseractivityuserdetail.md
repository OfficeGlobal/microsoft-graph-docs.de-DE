# <a name="reportroot-getteamsuseractivityuserdetail"></a><span data-ttu-id="7bd83-101">reportRoot: getTeamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="7bd83-101">reportRoot: getTeamsUserActivityUserDetail</span></span>

<span data-ttu-id="7bd83-102">Abrufen von Details zur Microsoft Teams-Benutzeraktivität nach Benutzer.</span><span class="sxs-lookup"><span data-stu-id="7bd83-102">Get details about Microsoft Teams user activity by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="7bd83-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7bd83-103">Permissions</span></span>

<span data-ttu-id="7bd83-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7bd83-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="7bd83-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7bd83-106">Permission type</span></span>                        | <span data-ttu-id="7bd83-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7bd83-107">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="7bd83-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7bd83-108">Delegated (work or school account)</span></span>     | <span data-ttu-id="7bd83-109">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7bd83-109">Not supported.</span></span>                           |
| <span data-ttu-id="7bd83-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7bd83-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7bd83-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7bd83-111">Not supported.</span></span>                           |
| <span data-ttu-id="7bd83-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7bd83-112">Application</span></span>                            | <span data-ttu-id="7bd83-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7bd83-113">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="7bd83-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7bd83-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserDetail(period='{period_value}')
GET /reports/getTeamsUserActivityUserDetail(date={date_value})
```

## <a name="request-parameters"></a><span data-ttu-id="7bd83-115">Anforderungsparameter</span><span class="sxs-lookup"><span data-stu-id="7bd83-115">Request parameters</span></span>

<span data-ttu-id="7bd83-116">Geben Sie in der Anforderungs-URL einen der folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="7bd83-116">In the request URL, provide the following query parameter with a valid value.</span></span>

| <span data-ttu-id="7bd83-117">Parameter</span><span class="sxs-lookup"><span data-stu-id="7bd83-117">Parameter</span></span> | <span data-ttu-id="7bd83-118">Typ</span><span class="sxs-lookup"><span data-stu-id="7bd83-118">Type</span></span>   | <span data-ttu-id="7bd83-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7bd83-119">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="7bd83-120">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="7bd83-120">period</span></span>    | <span data-ttu-id="7bd83-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7bd83-121">string</span></span> | <span data-ttu-id="7bd83-122">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="7bd83-122">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="7bd83-123">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="7bd83-123">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="7bd83-124">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="7bd83-124">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="7bd83-125">date</span><span class="sxs-lookup"><span data-stu-id="7bd83-125">date</span></span>      | <span data-ttu-id="7bd83-126">Datum</span><span class="sxs-lookup"><span data-stu-id="7bd83-126">Date</span></span>   | <span data-ttu-id="7bd83-127">Gibt das Datum an, für das die Benutzer angezeigt werden sollen, die Aktivitäten durchgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="7bd83-127">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="7bd83-128">{date_value} muss im Format JJJJ-MM-TT vorliegen.</span><span class="sxs-lookup"><span data-stu-id="7bd83-128">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="7bd83-129">Da dieser Bericht nur für die letzten 30 Tage verfügbar ist, sollte {date_value} ein Datum aus diesem Zeitraum sein.</span><span class="sxs-lookup"><span data-stu-id="7bd83-129">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="7bd83-130">**Hinweis:** Sie müssen in der URL entweder einen Zeitraum oder ein Datum festlegen.</span><span class="sxs-lookup"><span data-stu-id="7bd83-130">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7bd83-131">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7bd83-131">Request headers</span></span>

| <span data-ttu-id="7bd83-132">Name</span><span class="sxs-lookup"><span data-stu-id="7bd83-132">Name</span></span>          | <span data-ttu-id="7bd83-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7bd83-133">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="7bd83-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="7bd83-134">Authorization</span></span> | <span data-ttu-id="7bd83-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7bd83-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="7bd83-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="7bd83-137">Response</span></span>

<span data-ttu-id="7bd83-138">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="7bd83-138">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="7bd83-139">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7bd83-139">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="7bd83-140">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="7bd83-140">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="7bd83-141">Die CSV-Datei verfügt über die folgenden Spaltenheader:</span><span class="sxs-lookup"><span data-stu-id="7bd83-141">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="7bd83-142">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="7bd83-142">Report Refresh Date</span></span>
- <span data-ttu-id="7bd83-143">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="7bd83-143">User Principal Name</span></span>
- <span data-ttu-id="7bd83-144">Datum der letzten Aktivität</span><span class="sxs-lookup"><span data-stu-id="7bd83-144">Last Activity Date</span></span>
- <span data-ttu-id="7bd83-145">Ist gelöscht</span><span class="sxs-lookup"><span data-stu-id="7bd83-145">Is Deleted</span></span>
- <span data-ttu-id="7bd83-146">Gelöscht am</span><span class="sxs-lookup"><span data-stu-id="7bd83-146">Deleted Date</span></span>
- <span data-ttu-id="7bd83-147">Zugewiesene Produkte</span><span class="sxs-lookup"><span data-stu-id="7bd83-147">Assigned Products</span></span>
- <span data-ttu-id="7bd83-148">Anzahl der Team-Chatnachrichten</span><span class="sxs-lookup"><span data-stu-id="7bd83-148">Team Chat Message Count</span></span>
- <span data-ttu-id="7bd83-149">Anzahl der privaten Chatnachrichten</span><span class="sxs-lookup"><span data-stu-id="7bd83-149">Private Chat Message Count</span></span>
- <span data-ttu-id="7bd83-150">Anzahl der Anrufe</span><span class="sxs-lookup"><span data-stu-id="7bd83-150">Call Count</span></span>
- <span data-ttu-id="7bd83-151">Anzahl der Besprechung</span><span class="sxs-lookup"><span data-stu-id="7bd83-151">Meeting Count</span></span>
- <span data-ttu-id="7bd83-152">Andere Aktion</span><span class="sxs-lookup"><span data-stu-id="7bd83-152">Has Other Action</span></span>
- <span data-ttu-id="7bd83-153">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="7bd83-153">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="7bd83-154">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7bd83-154">Example</span></span>

#### <a name="request"></a><span data-ttu-id="7bd83-155">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7bd83-155">Request</span></span>

<span data-ttu-id="7bd83-156">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7bd83-156">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getTeamsUserActivityUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="7bd83-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="7bd83-157">Response</span></span>

<span data-ttu-id="7bd83-158">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7bd83-158">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="7bd83-159">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="7bd83-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Is Deleted,Deleted Date,Assigned Products,Team Chat Message Count,Private Chat Message Count,Call Count,Meeting Count,Has Other Action,Report Period
```
