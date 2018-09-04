# <a name="reportroot-getteamsuseractivitycounts"></a><span data-ttu-id="32025-101">reportRoot: getTeamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="32025-101">reportRoot: getTeamsUserActivityCounts</span></span>

<span data-ttu-id="32025-102">Diese Methode ruft die Anzahl von Microsoft Teams-Aktivitäten nach Aktivitätstyp ab.</span><span class="sxs-lookup"><span data-stu-id="32025-102">Get the number of Microsoft Teams activities by activity type.</span></span> <span data-ttu-id="32025-103">Die Aktivitätstypen sind Chatnachricht, private Chatnachricht, Anruf und Besprechung.</span><span class="sxs-lookup"><span data-stu-id="32025-103">The activity types are team chat messages, private chat messages, calls, and meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="32025-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="32025-104">Permissions</span></span>

<span data-ttu-id="32025-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="32025-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="32025-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="32025-107">Permission type</span></span>                        | <span data-ttu-id="32025-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="32025-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="32025-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="32025-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="32025-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="32025-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="32025-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="32025-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32025-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="32025-112">Not supported.</span></span>                           |
| <span data-ttu-id="32025-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="32025-113">Application</span></span>                            | <span data-ttu-id="32025-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="32025-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="32025-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="32025-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="32025-116">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="32025-116">Function parameters</span></span>

<span data-ttu-id="32025-117">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="32025-117">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="32025-118">Parameter</span><span class="sxs-lookup"><span data-stu-id="32025-118">Parameter</span></span> | <span data-ttu-id="32025-119">Typ</span><span class="sxs-lookup"><span data-stu-id="32025-119">Type</span></span>   | <span data-ttu-id="32025-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="32025-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="32025-121">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="32025-121">period</span></span>    | <span data-ttu-id="32025-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="32025-122">string</span></span> | <span data-ttu-id="32025-123">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="32025-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="32025-124">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="32025-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="32025-125">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="32025-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="32025-126">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="32025-126">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="32025-127">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="32025-127">Request headers</span></span>

| <span data-ttu-id="32025-128">Name</span><span class="sxs-lookup"><span data-stu-id="32025-128">Name</span></span>          | <span data-ttu-id="32025-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="32025-129">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="32025-130">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="32025-130">Authorization</span></span> | <span data-ttu-id="32025-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="32025-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="32025-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="32025-133">Response</span></span>

<span data-ttu-id="32025-134">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="32025-134">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="32025-135">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="32025-135">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="32025-136">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="32025-136">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="32025-137">Die CSV-Datei verfügt über die folgenden Spaltenheader:</span><span class="sxs-lookup"><span data-stu-id="32025-137">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="32025-138">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="32025-138">Report Refresh Date</span></span>
- <span data-ttu-id="32025-139">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="32025-139">Report Date</span></span>
- <span data-ttu-id="32025-140">Team-Chatnachrichten</span><span class="sxs-lookup"><span data-stu-id="32025-140">Team Chat Messages</span></span>
- <span data-ttu-id="32025-141">Private Chatnachrichten</span><span class="sxs-lookup"><span data-stu-id="32025-141">Private Chat Messages</span></span>
- <span data-ttu-id="32025-142">Anrufe</span><span class="sxs-lookup"><span data-stu-id="32025-142">Calls</span></span>
- <span data-ttu-id="32025-143">Besprechungen</span><span class="sxs-lookup"><span data-stu-id="32025-143">Meetings</span></span>
- <span data-ttu-id="32025-144">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="32025-144">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="32025-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="32025-145">Example</span></span>

#### <a name="request"></a><span data-ttu-id="32025-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="32025-146">Request</span></span>

<span data-ttu-id="32025-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="32025-147">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivitycounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getTeamsUserActivityCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="32025-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="32025-148">Response</span></span>

<span data-ttu-id="32025-149">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="32025-149">The following is an example of the response.</span></span>

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
<span data-ttu-id="32025-150">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="32025-150">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Team Chat Messages,Private Chat Messages,Calls,Meetings,Report Period
```
