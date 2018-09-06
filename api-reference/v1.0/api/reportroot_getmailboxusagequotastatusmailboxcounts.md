# <a name="reportroot-getmailboxusagequotastatusmailboxcounts"></a><span data-ttu-id="eaa8b-101">reportRoot: getMailboxUsageQuotaStatusMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="eaa8b-101">reportRoot: getMailboxUsageQuotaStatusMailboxCounts</span></span>

<span data-ttu-id="eaa8b-102">Rufen Sie die Anzahl der Benutzerpostfächer in jeder Kontingentkategorie ab.</span><span class="sxs-lookup"><span data-stu-id="eaa8b-102">Get the count of user mailboxes in each quota category.</span></span>

> <span data-ttu-id="eaa8b-103">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Postfachnutzung](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="eaa8b-103">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="eaa8b-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="eaa8b-104">Permissions</span></span>

<span data-ttu-id="eaa8b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="eaa8b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="eaa8b-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="eaa8b-107">Permission type</span></span>                        | <span data-ttu-id="eaa8b-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="eaa8b-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="eaa8b-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="eaa8b-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="eaa8b-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="eaa8b-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="eaa8b-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="eaa8b-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eaa8b-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eaa8b-112">Not supported.</span></span>                           |
| <span data-ttu-id="eaa8b-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="eaa8b-113">Application</span></span>                            | <span data-ttu-id="eaa8b-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="eaa8b-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="eaa8b-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="eaa8b-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageQuotaStatusMailboxCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="eaa8b-116">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="eaa8b-116">Function parameters</span></span>

<span data-ttu-id="eaa8b-117">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="eaa8b-117">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="eaa8b-118">Parameter</span><span class="sxs-lookup"><span data-stu-id="eaa8b-118">Parameter</span></span> | <span data-ttu-id="eaa8b-119">Typ</span><span class="sxs-lookup"><span data-stu-id="eaa8b-119">Type</span></span>   | <span data-ttu-id="eaa8b-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="eaa8b-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="eaa8b-121">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="eaa8b-121">period</span></span>    | <span data-ttu-id="eaa8b-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="eaa8b-122">string</span></span> | <span data-ttu-id="eaa8b-123">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="eaa8b-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="eaa8b-124">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="eaa8b-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="eaa8b-125">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="eaa8b-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="eaa8b-126">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="eaa8b-126">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="eaa8b-127">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="eaa8b-127">Request headers</span></span>

| <span data-ttu-id="eaa8b-128">Name</span><span class="sxs-lookup"><span data-stu-id="eaa8b-128">Name</span></span>          | <span data-ttu-id="eaa8b-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="eaa8b-129">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="eaa8b-130">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="eaa8b-130">Authorization</span></span> | <span data-ttu-id="eaa8b-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="eaa8b-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="eaa8b-133">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="eaa8b-133">If-None-Match</span></span> | <span data-ttu-id="eaa8b-134">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="eaa8b-134">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="eaa8b-135">Optional.</span><span class="sxs-lookup"><span data-stu-id="eaa8b-135">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="eaa8b-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="eaa8b-136">Response</span></span>

<span data-ttu-id="eaa8b-137">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="eaa8b-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="eaa8b-138">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="eaa8b-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="eaa8b-139">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="eaa8b-139">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="eaa8b-140">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="eaa8b-140">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="eaa8b-141">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="eaa8b-141">Report Refresh Date</span></span>
- <span data-ttu-id="eaa8b-142">Unter Grenzwert</span><span class="sxs-lookup"><span data-stu-id="eaa8b-142">Under Limit</span></span>
- <span data-ttu-id="eaa8b-143">Warnung ausgegeben</span><span class="sxs-lookup"><span data-stu-id="eaa8b-143">Warning Issued</span></span>
- <span data-ttu-id="eaa8b-144">Senden unzulässig</span><span class="sxs-lookup"><span data-stu-id="eaa8b-144">Send Prohibited</span></span>
- <span data-ttu-id="eaa8b-145">Senden/Empfangen unzulässig</span><span class="sxs-lookup"><span data-stu-id="eaa8b-145">Send/Receive Prohibited</span></span>
- <span data-ttu-id="eaa8b-146">Unbestimmt</span><span class="sxs-lookup"><span data-stu-id="eaa8b-146">Indeterminate</span></span>
- <span data-ttu-id="eaa8b-147">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="eaa8b-147">Report Date</span></span>
- <span data-ttu-id="eaa8b-148">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="eaa8b-148">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="eaa8b-149">Beispiel</span><span class="sxs-lookup"><span data-stu-id="eaa8b-149">Example</span></span>

#### <a name="request"></a><span data-ttu-id="eaa8b-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="eaa8b-150">Request</span></span>

<span data-ttu-id="eaa8b-151">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="eaa8b-151">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getmailboxusagequotastatusmailboxcounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getMailboxUsageQuotaStatusMailboxCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="eaa8b-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="eaa8b-152">Response</span></span>

<span data-ttu-id="eaa8b-153">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="eaa8b-153">The following is an example of the response.</span></span>

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

<span data-ttu-id="eaa8b-154">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="eaa8b-154">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Under Limit,Warning Issued,Send Prohibited,Send/Receive Prohibited,Indeterminate,Report Date,Report Period
```
