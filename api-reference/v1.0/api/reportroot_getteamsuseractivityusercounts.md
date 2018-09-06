# <a name="reportroot-getteamsuseractivityusercounts"></a><span data-ttu-id="10c96-101">reportRoot: getTeamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="10c96-101">reportRoot: getTeamsUserActivityUserCounts</span></span>

<span data-ttu-id="10c96-102">Diese Methode ruft die Anzahl von Microsoft Teams-Benutzern nach Aktivitätstyp ab.</span><span class="sxs-lookup"><span data-stu-id="10c96-102">Get the number of Microsoft Teams users by activity type.</span></span> <span data-ttu-id="10c96-103">Die Aktivitätstypen geben die Anzahl von Chatnachrichten, privaten Chatnachrichten, Anrufen oder Besprechungen der Teams an.</span><span class="sxs-lookup"><span data-stu-id="10c96-103">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="10c96-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="10c96-104">Permissions</span></span>

<span data-ttu-id="10c96-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="10c96-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="10c96-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="10c96-107">Permission type</span></span>                        | <span data-ttu-id="10c96-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="10c96-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="10c96-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="10c96-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="10c96-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="10c96-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="10c96-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="10c96-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10c96-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="10c96-112">Not supported.</span></span>                           |
| <span data-ttu-id="10c96-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="10c96-113">Application</span></span>                            | <span data-ttu-id="10c96-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="10c96-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="10c96-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="10c96-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="10c96-116">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="10c96-116">Function parameters</span></span>

<span data-ttu-id="10c96-117">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="10c96-117">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="10c96-118">Parameter</span><span class="sxs-lookup"><span data-stu-id="10c96-118">Parameter</span></span> | <span data-ttu-id="10c96-119">Typ</span><span class="sxs-lookup"><span data-stu-id="10c96-119">Type</span></span>   | <span data-ttu-id="10c96-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="10c96-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="10c96-121">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="10c96-121">period</span></span>    | <span data-ttu-id="10c96-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="10c96-122">string</span></span> | <span data-ttu-id="10c96-123">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="10c96-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="10c96-124">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="10c96-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="10c96-125">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="10c96-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="10c96-126">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="10c96-126">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="10c96-127">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="10c96-127">Request headers</span></span>

| <span data-ttu-id="10c96-128">Name</span><span class="sxs-lookup"><span data-stu-id="10c96-128">Name</span></span>          | <span data-ttu-id="10c96-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="10c96-129">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="10c96-130">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="10c96-130">Authorization</span></span> | <span data-ttu-id="10c96-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="10c96-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="10c96-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="10c96-133">Response</span></span>

<span data-ttu-id="10c96-134">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="10c96-134">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="10c96-135">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="10c96-135">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="10c96-136">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="10c96-136">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="10c96-137">Die CSV-Datei verfügt über die folgenden Spaltenheader:</span><span class="sxs-lookup"><span data-stu-id="10c96-137">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="10c96-138">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="10c96-138">Report Refresh Date</span></span>
- <span data-ttu-id="10c96-139">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="10c96-139">Report Date</span></span>
- <span data-ttu-id="10c96-140">Team-Chatnachrichten</span><span class="sxs-lookup"><span data-stu-id="10c96-140">Team Chat Messages</span></span>
- <span data-ttu-id="10c96-141">Private Chatnachrichten</span><span class="sxs-lookup"><span data-stu-id="10c96-141">Private Chat Messages</span></span>
- <span data-ttu-id="10c96-142">Anrufe</span><span class="sxs-lookup"><span data-stu-id="10c96-142">Calls</span></span>
- <span data-ttu-id="10c96-143">Besprechungen</span><span class="sxs-lookup"><span data-stu-id="10c96-143">Meetings</span></span>
- <span data-ttu-id="10c96-144">Sonstige Aktionen</span><span class="sxs-lookup"><span data-stu-id="10c96-144">Other Actions</span></span>
- <span data-ttu-id="10c96-145">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="10c96-145">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="10c96-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="10c96-146">Example</span></span>

#### <a name="request"></a><span data-ttu-id="10c96-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="10c96-147">Request</span></span>

<span data-ttu-id="10c96-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="10c96-148">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getTeamsUserActivityUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="10c96-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="10c96-149">Response</span></span>

<span data-ttu-id="10c96-150">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="10c96-150">The following is an example of the response.</span></span>

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

<span data-ttu-id="10c96-151">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="10c96-151">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Team Chat Messages,Private Chat Messages,Calls,Meetings,Other Actions,Report Period
```
