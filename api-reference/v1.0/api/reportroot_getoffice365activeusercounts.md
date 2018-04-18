# <a name="reportroot-getoffice365activeusercounts"></a><span data-ttu-id="5b6ee-101">reportRoot: getOffice365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="5b6ee-101">reportRoot: getOffice365ActiveUserCounts</span></span>

<span data-ttu-id="5b6ee-102">Rufen Sie die Anzahl der im Berichtszeitraum täglich aktiven Benutzer nach Produkt ab.</span><span class="sxs-lookup"><span data-stu-id="5b6ee-102">Get the count of daily active users in the reporting period by product.</span></span>

> <span data-ttu-id="5b6ee-103">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Aktive Benutzer](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="5b6ee-103">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="5b6ee-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5b6ee-104">Permissions</span></span>

<span data-ttu-id="5b6ee-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5b6ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="5b6ee-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5b6ee-107">Permission type</span></span>                        | <span data-ttu-id="5b6ee-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5b6ee-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="5b6ee-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5b6ee-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="5b6ee-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b6ee-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="5b6ee-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5b6ee-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b6ee-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5b6ee-112">Not supported.</span></span>                           |
| <span data-ttu-id="5b6ee-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5b6ee-113">Application</span></span>                            | <span data-ttu-id="5b6ee-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b6ee-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="5b6ee-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5b6ee-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="5b6ee-116">Anforderungsparameter</span><span class="sxs-lookup"><span data-stu-id="5b6ee-116">Request parameters</span></span>

<span data-ttu-id="5b6ee-117">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="5b6ee-117">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="5b6ee-118">Parameter</span><span class="sxs-lookup"><span data-stu-id="5b6ee-118">Parameter</span></span> | <span data-ttu-id="5b6ee-119">Typ</span><span class="sxs-lookup"><span data-stu-id="5b6ee-119">Type</span></span>   | <span data-ttu-id="5b6ee-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5b6ee-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="5b6ee-121">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="5b6ee-121">period</span></span>    | <span data-ttu-id="5b6ee-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5b6ee-122">string</span></span> | <span data-ttu-id="5b6ee-123">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="5b6ee-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="5b6ee-124">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="5b6ee-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="5b6ee-125">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="5b6ee-125">These values follow the format D   where    represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="5b6ee-126">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="5b6ee-126">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="5b6ee-127">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5b6ee-127">Request headers</span></span>

| <span data-ttu-id="5b6ee-128">Name</span><span class="sxs-lookup"><span data-stu-id="5b6ee-128">Name</span></span>          | <span data-ttu-id="5b6ee-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5b6ee-129">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="5b6ee-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b6ee-130">Authorization</span></span> | <span data-ttu-id="5b6ee-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5b6ee-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="5b6ee-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="5b6ee-133">Response</span></span>

<span data-ttu-id="5b6ee-134">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="5b6ee-134">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="5b6ee-135">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5b6ee-135">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="5b6ee-136">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="5b6ee-136">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="5b6ee-137">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="5b6ee-137">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="5b6ee-138">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="5b6ee-138">Report Refresh Date</span></span>
- <span data-ttu-id="5b6ee-139">Office 365</span><span class="sxs-lookup"><span data-stu-id="5b6ee-139">Office 365</span></span>
- <span data-ttu-id="5b6ee-140">Exchange</span><span class="sxs-lookup"><span data-stu-id="5b6ee-140">Exchange</span></span>
- <span data-ttu-id="5b6ee-141">OneDrive</span><span class="sxs-lookup"><span data-stu-id="5b6ee-141">OneDrive</span></span>
- <span data-ttu-id="5b6ee-142">SharePoint</span><span class="sxs-lookup"><span data-stu-id="5b6ee-142">SharePoint</span></span>
- <span data-ttu-id="5b6ee-143">Skype for Business</span><span class="sxs-lookup"><span data-stu-id="5b6ee-143">Skype For Business</span></span> 
- <span data-ttu-id="5b6ee-144">Yammer</span><span class="sxs-lookup"><span data-stu-id="5b6ee-144">Yammer</span></span>
- <span data-ttu-id="5b6ee-145">Teams</span><span class="sxs-lookup"><span data-stu-id="5b6ee-145">Teams</span></span>
- <span data-ttu-id="5b6ee-146">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="5b6ee-146">Report Date</span></span>
- <span data-ttu-id="5b6ee-147">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="5b6ee-147">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="5b6ee-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5b6ee-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="5b6ee-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5b6ee-149">Request</span></span>

<span data-ttu-id="5b6ee-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5b6ee-150">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActiveUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="5b6ee-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="5b6ee-151">Response</span></span>

<span data-ttu-id="5b6ee-152">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5b6ee-152">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="5b6ee-153">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="5b6ee-153">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Office 365,Exchange,OneDrive,SharePoint,Skype For Business,Yammer,Teams,Report Date,Report Period
```
