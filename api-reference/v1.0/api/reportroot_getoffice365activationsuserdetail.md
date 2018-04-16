# <a name="reportroot-getoffice365activationsuserdetail"></a><span data-ttu-id="183d3-101">reportRoot: getOffice365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="183d3-101">reportRoot: getOffice365ActivationsUserDetail</span></span>

<span data-ttu-id="183d3-102">Erhalten Sie detaillierte Informationen über Benutzer, die Office 365 aktiviert haben.</span><span class="sxs-lookup"><span data-stu-id="183d3-102">Get details about users who have activated Office 365.</span></span>

> <span data-ttu-id="183d3-103">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Microsoft Office-Aktivierungen](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="183d3-103">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="183d3-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="183d3-104">Permissions</span></span>

<span data-ttu-id="183d3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="183d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="183d3-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="183d3-107">Permission type</span></span>                        | <span data-ttu-id="183d3-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="183d3-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="183d3-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="183d3-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="183d3-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="183d3-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="183d3-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="183d3-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="183d3-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="183d3-112">Not supported.</span></span>                           |
| <span data-ttu-id="183d3-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="183d3-113">Application</span></span>                            | <span data-ttu-id="183d3-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="183d3-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="183d3-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="183d3-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserDetail
```

## <a name="request-headers"></a><span data-ttu-id="183d3-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="183d3-116">Request headers</span></span>

| <span data-ttu-id="183d3-117">Name</span><span class="sxs-lookup"><span data-stu-id="183d3-117">Name</span></span>          | <span data-ttu-id="183d3-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="183d3-118">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="183d3-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="183d3-119">Authorization</span></span> | <span data-ttu-id="183d3-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="183d3-p102">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="183d3-122">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="183d3-122">If-None-Match</span></span> | <span data-ttu-id="183d3-123">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="183d3-123">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="183d3-124">Optional.</span><span class="sxs-lookup"><span data-stu-id="183d3-124">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="183d3-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="183d3-125">Response</span></span>

<span data-ttu-id="183d3-126">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="183d3-126">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="183d3-127">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="183d3-127">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="183d3-128">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="183d3-128">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="183d3-129">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="183d3-129">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="183d3-130">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="183d3-130">Report Refresh Date</span></span>
- <span data-ttu-id="183d3-131">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="183d3-131">User Principal Name</span></span>
- <span data-ttu-id="183d3-132">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="183d3-132">Display Name</span></span>
- <span data-ttu-id="183d3-133">Produkttyp</span><span class="sxs-lookup"><span data-stu-id="183d3-133">Product Type</span></span>
- <span data-ttu-id="183d3-134">Datum der letzten Aktivierung</span><span class="sxs-lookup"><span data-stu-id="183d3-134">Last Activated Date</span></span>
- <span data-ttu-id="183d3-135">Windows</span><span class="sxs-lookup"><span data-stu-id="183d3-135">Windows</span></span>
- <span data-ttu-id="183d3-136">Mac</span><span class="sxs-lookup"><span data-stu-id="183d3-136">Mac</span></span>
- <span data-ttu-id="183d3-137">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="183d3-137">Windows 10 Mobile</span></span>
- <span data-ttu-id="183d3-138">iOS</span><span class="sxs-lookup"><span data-stu-id="183d3-138">iOS</span></span>
- <span data-ttu-id="183d3-139">Android</span><span class="sxs-lookup"><span data-stu-id="183d3-139">Android</span></span>

## <a name="example"></a><span data-ttu-id="183d3-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="183d3-140">Example</span></span>

#### <a name="request"></a><span data-ttu-id="183d3-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="183d3-141">Request</span></span>

<span data-ttu-id="183d3-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="183d3-142">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationsuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationsUserDetail
```

#### <a name="response"></a><span data-ttu-id="183d3-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="183d3-143">Response</span></span>

<span data-ttu-id="183d3-144">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="183d3-144">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="183d3-145">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="183d3-145">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Product Type,Last Activated Date,Windows,Mac,Windows 10 Mobile,iOS,Android
```
