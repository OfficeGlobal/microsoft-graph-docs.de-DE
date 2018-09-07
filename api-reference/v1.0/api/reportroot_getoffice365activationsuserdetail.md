# <a name="reportroot-getoffice365activationsuserdetail"></a><span data-ttu-id="fed6e-101">reportRoot: getOffice365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="fed6e-101">reportRoot: getOffice365ActivationsUserDetail</span></span>

<span data-ttu-id="fed6e-102">Erhalten Sie detaillierte Informationen über Benutzer, die Office 365 aktiviert haben.</span><span class="sxs-lookup"><span data-stu-id="fed6e-102">Get details about users who have activated Office 365.</span></span>

> <span data-ttu-id="fed6e-103">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Microsoft Office-Aktivierungen](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="fed6e-103">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="fed6e-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="fed6e-104">Permissions</span></span>

<span data-ttu-id="fed6e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fed6e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="fed6e-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fed6e-107">Permission type</span></span>                        | <span data-ttu-id="fed6e-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fed6e-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="fed6e-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fed6e-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="fed6e-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fed6e-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="fed6e-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fed6e-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fed6e-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fed6e-112">Not supported.</span></span>                           |
| <span data-ttu-id="fed6e-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fed6e-113">Application</span></span>                            | <span data-ttu-id="fed6e-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fed6e-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="fed6e-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fed6e-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserDetail
```

## <a name="request-headers"></a><span data-ttu-id="fed6e-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fed6e-116">Request headers</span></span>

| <span data-ttu-id="fed6e-117">Name</span><span class="sxs-lookup"><span data-stu-id="fed6e-117">Name</span></span>          | <span data-ttu-id="fed6e-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fed6e-118">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="fed6e-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="fed6e-119">Authorization</span></span> | <span data-ttu-id="fed6e-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fed6e-p102">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="fed6e-122">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="fed6e-122">If-None-Match</span></span> | <span data-ttu-id="fed6e-123">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fed6e-123">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="fed6e-124">Optional.</span><span class="sxs-lookup"><span data-stu-id="fed6e-124">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="fed6e-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="fed6e-125">Response</span></span>

<span data-ttu-id="fed6e-126">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="fed6e-126">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="fed6e-127">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="fed6e-127">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="fed6e-128">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="fed6e-128">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="fed6e-129">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="fed6e-129">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="fed6e-130">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="fed6e-130">Report Refresh Date</span></span>
- <span data-ttu-id="fed6e-131">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="fed6e-131">User Principal Name</span></span>
- <span data-ttu-id="fed6e-132">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="fed6e-132">Display Name</span></span>
- <span data-ttu-id="fed6e-133">Produkttyp</span><span class="sxs-lookup"><span data-stu-id="fed6e-133">Product Type</span></span>
- <span data-ttu-id="fed6e-134">Datum der letzten Aktivierung</span><span class="sxs-lookup"><span data-stu-id="fed6e-134">Last Activated Date</span></span>
- <span data-ttu-id="fed6e-135">Windows</span><span class="sxs-lookup"><span data-stu-id="fed6e-135">Windows</span></span>
- <span data-ttu-id="fed6e-136">Mac</span><span class="sxs-lookup"><span data-stu-id="fed6e-136">Mac</span></span>
- <span data-ttu-id="fed6e-137">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="fed6e-137">Windows 10 Mobile</span></span>
- <span data-ttu-id="fed6e-138">iOS</span><span class="sxs-lookup"><span data-stu-id="fed6e-138">iOS</span></span>
- <span data-ttu-id="fed6e-139">Android</span><span class="sxs-lookup"><span data-stu-id="fed6e-139">Android</span></span>
- <span data-ttu-id="fed6e-140">Gemeinsam genutzter Computer aktiviert</span><span class="sxs-lookup"><span data-stu-id="fed6e-140">Activated On Shared Computer</span></span>

## <a name="example"></a><span data-ttu-id="fed6e-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fed6e-141">Example</span></span>

#### <a name="request"></a><span data-ttu-id="fed6e-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fed6e-142">Request</span></span>

<span data-ttu-id="fed6e-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fed6e-143">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activationsuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationsUserDetail
```

#### <a name="response"></a><span data-ttu-id="fed6e-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="fed6e-144">Response</span></span>

<span data-ttu-id="fed6e-145">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="fed6e-145">The following is an example of the response.</span></span>

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

<span data-ttu-id="fed6e-146">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="fed6e-146">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Product Type,Last Activated Date,Windows,Mac,Windows 10 Mobile,iOS,Android,Activated On Shared Computer
```
