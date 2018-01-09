# <a name="reportroot-getoffice365activationsusercounts"></a><span data-ttu-id="71358-101">reportRoot: getOffice365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="71358-101">reportRoot: getOffice365ActivationsUserCounts</span></span>

<span data-ttu-id="71358-102">Rufen Sie die Anzahl der aktivierten Benutzer ab und erfahren Sie, wie viele Benutzer das Office-Abonnement auf dem Desktop oder einem Gerät aktiviert haben.</span><span class="sxs-lookup"><span data-stu-id="71358-102">Get the count of users that are enabled and those that have activated the Office subscription on desktop or devices.</span></span>

> <span data-ttu-id="71358-103">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Microsoft Office-Aktivierungen]((https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)).</span><span class="sxs-lookup"><span data-stu-id="71358-103">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations]((https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)).</span></span>

## <a name="permissions"></a><span data-ttu-id="71358-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="71358-104">Permissions</span></span>

<span data-ttu-id="71358-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="71358-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="71358-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="71358-107">Permission type</span></span>                        | <span data-ttu-id="71358-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="71358-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="71358-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="71358-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="71358-110">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="71358-110">Not supported.</span></span>                           |
| <span data-ttu-id="71358-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="71358-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71358-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="71358-112">Not supported.</span></span>                           |
| <span data-ttu-id="71358-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="71358-113">Application</span></span>                            | <span data-ttu-id="71358-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="71358-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="71358-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="71358-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserCounts
```

## <a name="request-headers"></a><span data-ttu-id="71358-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="71358-116">Request headers</span></span>

| <span data-ttu-id="71358-117">Name</span><span class="sxs-lookup"><span data-stu-id="71358-117">Name</span></span>          | <span data-ttu-id="71358-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="71358-118">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="71358-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="71358-119">Authorization</span></span> | <span data-ttu-id="71358-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="71358-p102">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="71358-122">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="71358-122">if-none-match</span></span> | <span data-ttu-id="71358-123">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="71358-123">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `304 Not Modified` response is returned.</span></span> <span data-ttu-id="71358-124">Optional.</span><span class="sxs-lookup"><span data-stu-id="71358-124">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="71358-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="71358-125">Response</span></span>

<span data-ttu-id="71358-126">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="71358-126">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="71358-127">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="71358-127">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="71358-128">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="71358-128">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

<span data-ttu-id="71358-129">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="71358-129">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="71358-130">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="71358-130">Report Refresh Date</span></span>
- <span data-ttu-id="71358-131">Produkttyp</span><span class="sxs-lookup"><span data-stu-id="71358-131">Product External Content Type</span></span>
- <span data-ttu-id="71358-132">Zugewiesen</span><span class="sxs-lookup"><span data-stu-id="71358-132">Assigned</span></span>
- <span data-ttu-id="71358-133">Aktiviert</span><span class="sxs-lookup"><span data-stu-id="71358-133">Activated</span></span>

## <a name="example"></a><span data-ttu-id="71358-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="71358-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="71358-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="71358-135">Request</span></span>

<span data-ttu-id="71358-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="71358-136">The following is an example of making the request in ASP.NET that uses the TokenHelper file:</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationsusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationsUserCounts
```

#### <a name="response"></a><span data-ttu-id="71358-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="71358-137">Response</span></span>

<span data-ttu-id="71358-138">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="71358-138">Here is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="71358-139">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="71358-139">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Product Type,Assigned,Activated
```
