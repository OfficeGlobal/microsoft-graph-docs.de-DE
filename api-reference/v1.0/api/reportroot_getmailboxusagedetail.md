# <a name="reportroot-getmailboxusagedetail"></a><span data-ttu-id="06b65-101">reportRoot: getMailboxUsageDetail</span><span class="sxs-lookup"><span data-stu-id="06b65-101">reportRoot: getMailboxUsageDetail</span></span>

<span data-ttu-id="06b65-102">Erhalten Sie detaillierte Informationen über die Postfachnutzung.</span><span class="sxs-lookup"><span data-stu-id="06b65-102">Get details about mailbox usage.</span></span>

> <span data-ttu-id="06b65-103">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Postfachnutzung](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="06b65-103">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="06b65-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="06b65-104">Permissions</span></span>

<span data-ttu-id="06b65-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="06b65-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="06b65-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="06b65-107">Permission type</span></span>                        | <span data-ttu-id="06b65-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="06b65-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="06b65-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="06b65-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="06b65-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="06b65-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="06b65-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="06b65-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06b65-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="06b65-112">Not supported.</span></span>                           |
| <span data-ttu-id="06b65-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="06b65-113">Application</span></span>                            | <span data-ttu-id="06b65-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="06b65-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="06b65-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="06b65-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageDetail(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="06b65-116">Anforderungsparameter</span><span class="sxs-lookup"><span data-stu-id="06b65-116">Request parameters</span></span>

<span data-ttu-id="06b65-117">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="06b65-117">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="06b65-118">Parameter</span><span class="sxs-lookup"><span data-stu-id="06b65-118">Parameter</span></span> | <span data-ttu-id="06b65-119">Typ</span><span class="sxs-lookup"><span data-stu-id="06b65-119">Type</span></span>   | <span data-ttu-id="06b65-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="06b65-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="06b65-121">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="06b65-121">period</span></span>    | <span data-ttu-id="06b65-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="06b65-122">string</span></span> | <span data-ttu-id="06b65-123">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="06b65-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="06b65-124">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="06b65-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="06b65-125">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="06b65-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="06b65-126">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="06b65-126">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="06b65-127">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="06b65-127">Request headers</span></span>

| <span data-ttu-id="06b65-128">Name</span><span class="sxs-lookup"><span data-stu-id="06b65-128">Name</span></span>          | <span data-ttu-id="06b65-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="06b65-129">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="06b65-130">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="06b65-130">Authorization</span></span> | <span data-ttu-id="06b65-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="06b65-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="06b65-133">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="06b65-133">If-None-Match</span></span> | <span data-ttu-id="06b65-134">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="06b65-134">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="06b65-135">Optional.</span><span class="sxs-lookup"><span data-stu-id="06b65-135">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="06b65-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="06b65-136">Response</span></span>

<span data-ttu-id="06b65-137">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="06b65-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="06b65-138">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="06b65-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="06b65-139">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="06b65-139">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="06b65-140">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="06b65-140">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="06b65-141">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="06b65-141">Report Refresh Date</span></span>
- <span data-ttu-id="06b65-142">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="06b65-142">User Principal Name</span></span>
- <span data-ttu-id="06b65-143">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="06b65-143">Display Name</span></span>
- <span data-ttu-id="06b65-144">Ist gelöscht</span><span class="sxs-lookup"><span data-stu-id="06b65-144">Is Deleted</span></span>
- <span data-ttu-id="06b65-145">Gelöscht am</span><span class="sxs-lookup"><span data-stu-id="06b65-145">Deleted Date</span></span>
- <span data-ttu-id="06b65-146">Erstellungsdatum</span><span class="sxs-lookup"><span data-stu-id="06b65-146">Created Date</span></span>
- <span data-ttu-id="06b65-147">Datum der letzten Aktivität</span><span class="sxs-lookup"><span data-stu-id="06b65-147">Last Activity Date</span></span>
- <span data-ttu-id="06b65-148">Elementanzahl</span><span class="sxs-lookup"><span data-stu-id="06b65-148">Item Count</span></span>
- <span data-ttu-id="06b65-149">Verwendeter Speicherplatz (Byte)</span><span class="sxs-lookup"><span data-stu-id="06b65-149">Storage Used (Byte)</span></span>
- <span data-ttu-id="06b65-150">Kontingent für Problemwarnung (Byte)</span><span class="sxs-lookup"><span data-stu-id="06b65-150">Issue Warning Quota (Byte)</span></span>
- <span data-ttu-id="06b65-151">Kontingent für Senden verbieten (Byte)</span><span class="sxs-lookup"><span data-stu-id="06b65-151">Prohibit Send Quota (Byte)</span></span>
- <span data-ttu-id="06b65-152">Kontingent für Senden/Empfangen verbieten (Byte)</span><span class="sxs-lookup"><span data-stu-id="06b65-152">Prohibit Send/Receive Quota (Byte)</span></span>
- <span data-ttu-id="06b65-153">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="06b65-153">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="06b65-154">Beispiel</span><span class="sxs-lookup"><span data-stu-id="06b65-154">Example</span></span>

#### <a name="request"></a><span data-ttu-id="06b65-155">Anforderung</span><span class="sxs-lookup"><span data-stu-id="06b65-155">Request</span></span>

<span data-ttu-id="06b65-156">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="06b65-156">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getmailboxusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getMailboxUsageDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="06b65-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="06b65-157">Response</span></span>

<span data-ttu-id="06b65-158">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="06b65-158">The following is an example of the response.</span></span>

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

<span data-ttu-id="06b65-159">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="06b65-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Created Date,Last Activity Date,Item Count,Storage Used (Byte),Issue Warning Quota (Byte),Prohibit Send Quota (Byte),Prohibit Send/Receive Quota (Byte),Report Period
```
