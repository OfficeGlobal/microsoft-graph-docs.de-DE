# <a name="reportroot-getteamsuseractivityusercounts"></a><span data-ttu-id="c6ceb-101">reportRoot: getTeamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="c6ceb-101">reportRoot: getTeamsUserActivityUserCounts</span></span>

<span data-ttu-id="c6ceb-102">Diese Methode ruft die Anzahl von Microsoft Teams-Benutzern nach Aktivitätstyp ab.</span><span class="sxs-lookup"><span data-stu-id="c6ceb-102">Get the number of Microsoft Teams users by activity type.</span></span> <span data-ttu-id="c6ceb-103">Die Aktivitätstypen geben die Anzahl von Chatnachrichten, privaten Chatnachrichten, Anrufen oder Besprechungen der Teams an.</span><span class="sxs-lookup"><span data-stu-id="c6ceb-103">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="c6ceb-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c6ceb-104">Permissions</span></span>

<span data-ttu-id="c6ceb-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c6ceb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="c6ceb-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c6ceb-107">Permission type</span></span>                        | <span data-ttu-id="c6ceb-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c6ceb-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="c6ceb-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c6ceb-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="c6ceb-110">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c6ceb-110">Not supported.</span></span>                           |
| <span data-ttu-id="c6ceb-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c6ceb-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6ceb-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c6ceb-112">Not supported.</span></span>                           |
| <span data-ttu-id="c6ceb-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c6ceb-113">Application</span></span>                            | <span data-ttu-id="c6ceb-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c6ceb-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="c6ceb-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c6ceb-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="c6ceb-116">Anforderungsparameter</span><span class="sxs-lookup"><span data-stu-id="c6ceb-116">Request parameters</span></span>

<span data-ttu-id="c6ceb-117">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="c6ceb-117">In the request URL, provide the following query parameter with a valid value.</span></span>

| <span data-ttu-id="c6ceb-118">Parameter</span><span class="sxs-lookup"><span data-stu-id="c6ceb-118">Parameter</span></span> | <span data-ttu-id="c6ceb-119">Typ</span><span class="sxs-lookup"><span data-stu-id="c6ceb-119">Type</span></span>   | <span data-ttu-id="c6ceb-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c6ceb-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="c6ceb-121">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="c6ceb-121">period</span></span>    | <span data-ttu-id="c6ceb-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c6ceb-122">string</span></span> | <span data-ttu-id="c6ceb-123">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="c6ceb-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="c6ceb-124">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="c6ceb-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="c6ceb-125">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="c6ceb-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="c6ceb-126">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c6ceb-126">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="c6ceb-127">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c6ceb-127">Request headers</span></span>

| <span data-ttu-id="c6ceb-128">Name</span><span class="sxs-lookup"><span data-stu-id="c6ceb-128">Name</span></span>          | <span data-ttu-id="c6ceb-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c6ceb-129">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="c6ceb-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="c6ceb-130">Authorization</span></span> | <span data-ttu-id="c6ceb-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c6ceb-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="c6ceb-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="c6ceb-133">Response</span></span>

<span data-ttu-id="c6ceb-134">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="c6ceb-134">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="c6ceb-135">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c6ceb-135">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="c6ceb-136">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="c6ceb-136">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="c6ceb-137">Die CSV-Datei verfügt über die folgenden Spaltenheader:</span><span class="sxs-lookup"><span data-stu-id="c6ceb-137">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="c6ceb-138">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="c6ceb-138">Report Refresh Date</span></span>
- <span data-ttu-id="c6ceb-139">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="c6ceb-139">Report Date</span></span>
- <span data-ttu-id="c6ceb-140">Team-Chatnachrichten</span><span class="sxs-lookup"><span data-stu-id="c6ceb-140">Team Chat Messages</span></span>
- <span data-ttu-id="c6ceb-141">Private Chatnachrichten</span><span class="sxs-lookup"><span data-stu-id="c6ceb-141">Private Chat Messages</span></span>
- <span data-ttu-id="c6ceb-142">Anrufe</span><span class="sxs-lookup"><span data-stu-id="c6ceb-142">API Calls</span></span>
- <span data-ttu-id="c6ceb-143">Besprechungen</span><span class="sxs-lookup"><span data-stu-id="c6ceb-143">meetings</span></span>
- <span data-ttu-id="c6ceb-144">Sonstige Aktionen</span><span class="sxs-lookup"><span data-stu-id="c6ceb-144">Other Actions</span></span>
- <span data-ttu-id="c6ceb-145">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="c6ceb-145">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="c6ceb-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c6ceb-146">Example</span></span>

#### <a name="request"></a><span data-ttu-id="c6ceb-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c6ceb-147">Request</span></span>

<span data-ttu-id="c6ceb-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c6ceb-148">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getTeamsUserActivityUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="c6ceb-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="c6ceb-149">Response</span></span>

<span data-ttu-id="c6ceb-150">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c6ceb-150">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="c6ceb-151">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="c6ceb-151">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Team Chat Messages,Private Chat Messages,Calls,Meetings,Other Actions,Report Period
```
