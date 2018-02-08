# <a name="reportroot-getoffice365servicesusercounts"></a><span data-ttu-id="322d7-101">reportRoot: getOffice365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="322d7-101">reportRoot: getOffice365ServicesUserCounts</span></span>

<span data-ttu-id="322d7-102">Rufen Sie die Anzahl der Benutzer nach Aktivitätstyp und Dienst ab.</span><span class="sxs-lookup"><span data-stu-id="322d7-102">Get the count of users by activity type and service.</span></span>

> <span data-ttu-id="322d7-103">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Aktive Benutzer](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="322d7-103">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="322d7-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="322d7-104">Permissions</span></span>

<span data-ttu-id="322d7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="322d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="322d7-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="322d7-107">Permission type</span></span>                        | <span data-ttu-id="322d7-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="322d7-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="322d7-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="322d7-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="322d7-110">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="322d7-110">Not supported.</span></span>                           |
| <span data-ttu-id="322d7-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="322d7-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="322d7-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="322d7-112">Not supported.</span></span>                           |
| <span data-ttu-id="322d7-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="322d7-113">Application</span></span>                            | <span data-ttu-id="322d7-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="322d7-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="322d7-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="322d7-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ServicesUserCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="322d7-116">Anforderungsparameter</span><span class="sxs-lookup"><span data-stu-id="322d7-116">Request parameters</span></span>

<span data-ttu-id="322d7-117">Stellen Sie in der URL der Anforderung den folgenden Parameter mit einem gültigen Wert bereit.</span><span class="sxs-lookup"><span data-stu-id="322d7-117">In the request URL, provide the following query parameter with a valid value.</span></span>

| <span data-ttu-id="322d7-118">Parameter</span><span class="sxs-lookup"><span data-stu-id="322d7-118">Parameter</span></span> | <span data-ttu-id="322d7-119">Typ</span><span class="sxs-lookup"><span data-stu-id="322d7-119">Type</span></span>   | <span data-ttu-id="322d7-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="322d7-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="322d7-121">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="322d7-121">period</span></span>    | <span data-ttu-id="322d7-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="322d7-122">string</span></span> | <span data-ttu-id="322d7-123">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="322d7-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="322d7-124">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="322d7-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="322d7-125">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="322d7-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="322d7-126">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="322d7-126">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="322d7-127">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="322d7-127">Request headers</span></span>

| <span data-ttu-id="322d7-128">Name</span><span class="sxs-lookup"><span data-stu-id="322d7-128">Name</span></span>          | <span data-ttu-id="322d7-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="322d7-129">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="322d7-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="322d7-130">Authorization</span></span> | <span data-ttu-id="322d7-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="322d7-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="322d7-133">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="322d7-133">If-None-Match</span></span> | <span data-ttu-id="322d7-134">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="322d7-134">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="322d7-135">Optional.</span><span class="sxs-lookup"><span data-stu-id="322d7-135">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="322d7-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="322d7-136">Response</span></span>

<span data-ttu-id="322d7-137">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="322d7-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="322d7-138">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="322d7-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="322d7-139">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="322d7-139">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="322d7-140">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="322d7-140">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="322d7-141">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="322d7-141">Report Refresh Date</span></span>
- <span data-ttu-id="322d7-142">Exchange aktiv</span><span class="sxs-lookup"><span data-stu-id="322d7-142">Exchange Active</span></span>
- <span data-ttu-id="322d7-143">Exchange inaktiv</span><span class="sxs-lookup"><span data-stu-id="322d7-143">Exchange Inactive</span></span>
- <span data-ttu-id="322d7-144">OneDrive aktiv</span><span class="sxs-lookup"><span data-stu-id="322d7-144">OneDrive Active</span></span>
- <span data-ttu-id="322d7-145">OneDrive inaktiv</span><span class="sxs-lookup"><span data-stu-id="322d7-145">OneDrive Inactive</span></span>
- <span data-ttu-id="322d7-146">SharePoint aktiv</span><span class="sxs-lookup"><span data-stu-id="322d7-146">SharePoint Active</span></span>
- <span data-ttu-id="322d7-147">SharePoint inaktiv</span><span class="sxs-lookup"><span data-stu-id="322d7-147">SharePoint Inactive</span></span>
- <span data-ttu-id="322d7-148">Skype for Business aktiv</span><span class="sxs-lookup"><span data-stu-id="322d7-148">Skype For Business Active</span></span>
- <span data-ttu-id="322d7-149">Skype for Business inaktiv</span><span class="sxs-lookup"><span data-stu-id="322d7-149">Skype For Business Inactive</span></span>
- <span data-ttu-id="322d7-150">Yammer aktiv</span><span class="sxs-lookup"><span data-stu-id="322d7-150">Yammer Active</span></span>
- <span data-ttu-id="322d7-151">Yammer inaktiv</span><span class="sxs-lookup"><span data-stu-id="322d7-151">Yammer Inactive</span></span>
- <span data-ttu-id="322d7-152">Teams aktiv</span><span class="sxs-lookup"><span data-stu-id="322d7-152">Teams Active</span></span>
- <span data-ttu-id="322d7-153">Teams inaktiv</span><span class="sxs-lookup"><span data-stu-id="322d7-153">Teams Inactive</span></span>
- <span data-ttu-id="322d7-154">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="322d7-154">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="322d7-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="322d7-155">Example</span></span>

#### <a name="request"></a><span data-ttu-id="322d7-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="322d7-156">Request</span></span>

<span data-ttu-id="322d7-157">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="322d7-157">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365servicesusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ServicesUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="322d7-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="322d7-158">Response</span></span>

<span data-ttu-id="322d7-159">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="322d7-159">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="322d7-160">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="322d7-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Exchange Active,Exchange Inactive,OneDrive Active,OneDrive Inactive,SharePoint Active,SharePoint Inactive,Skype For Business Active,Skype For Business Inactive,Yammer Active,Yammer Inactive,Teams Active,Teams Inactive,Report Period
```
